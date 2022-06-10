---
title: 'Enhanced PDF to HTML, PDF to Excel Conversion and Better Compatibility with COM Interop with Aspose.PDF for .NET 9.4.0'
date: Mon, 21 Jul 2014 00:04:36 +0000
draft: false
url: /2014/07/21/enhanced-pdf-to-html-better-compatibility-with-com-interop-and-stable-pdf-to-excel-file-conversion-with-aspose.pdf-for-.net-9.4.0/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'C# .NET PDF API', 'Convert PDF document to HTML', 'PDF to Excel XLS XLSX']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net_100.png" alt="Aspose.Pdf for .NET logo">}}


At Aspose, we always strive to provide enhanced versions of our APIs, stable and optimized as compared to earlier versions. In the recent versions of Aspose.PDF for .NET, our focus has been improving file format conversion including PDF to HTML, SVG to PDF, PDF to Excel, PDF to DOC, image to PDF and PDF to image format. In fact, PDF files to HTML rendering are one of the most demanded features because it provides the ability to convert any PDF file to raw HTML format and the output HTML can be viewed on any platform using any web browser. This makes our customers' work a lot easier and enables them to use our API in distributed web applications as well as cloud-based systems. It helps their customers view PDF files on various platforms, without being worried about the PDF viewing application. This feature is used a lot in applications developed by our sister company named [GroupDocs][1]. In latest release of [Aspose.PDF for .NET 9.4.0][2] , we have introduced a feature that extracts fonts independently of HTML, SVG and other resources. The following code snippet shows the steps to perform this feature.

1.  Performs fonts extraction from the document (with new FontAbsorber class).
2.  Saves fonts into cache folder (with Font.Save method).
3.  Passes the cached fonts into HTML conversion procedure (with htmlOptions.FontSources).
4.  Splits the document into separate pages.
5.  Performs HTML conversion of each page in parallel threads.
6.  All the threads use single fonts set.
7.  If the fonts are passed as a font sources the fonts are not extracted, decoded and processed, they are just passed into the resources saving callback in corresponding format.

```
public void PDFNEWNET_36524_cacheFonts_Sample()
{
Helper.SetLicense();

string inFile = TestSettings.GetInputFile("36524.pdf");

HTMLMultithreadingTester_FontCache_Sample tester = new HTMLMultithreadingTester_FontCache_Sample(inFile);
tester.Run();
}

class HTMLMultithreadingTester_FontCache_Sample
{
public HTMLMultithreadingTester_FontCache_Sample(string inputFile)
{
    inFile = inputFile;
    fileNameOnly = Path.GetFileNameWithoutExtension(inFile);
    testOut = Path.Combine(TestSettings.TestOutput, fileNameOnly);

    // Delete previous output directories
    if (Directory.Exists(testOut))
    {
        string[] files = Directory.GetFiles(testOut, "*.*", SearchOption.AllDirectories);
        foreach (string file in files)
        {
            File.Delete(file);
        }
        string[] directories = Directory.GetDirectories(testOut, "*.*", SearchOption.AllDirectories);
        foreach (string dir in directories)
        {
            Directory.Delete(dir);
        }
    }
    Directory.CreateDirectory(testOut);
}

string inFile;
string testOut;
string fileNameOnly;

public Dictionary outFileNames = new Dictionary();

public void Run()
{
    Helper.SetLicense();

    // Folder that contains pre-generated cached fonts 
    // All the fonts of the document will be placed to this folder and will be passed to each page conversion procedure
    string fontCacheFolder = Path.Combine(testOut, fileNameOnly + "_fonts_preSaved\\");
    string cacheFontFileTemplate = Path.Combine(fontCacheFolder, "font{0}.ttf");

    // Folder that will contain fonts as a result of the conversion procedure
    string fontOutFolder = Path.GetFullPath(Path.Combine(testOut, fileNameOnly + "_fonts\\"));

    // Create our folders
    Directory.CreateDirectory(fontCacheFolder);
    Directory.CreateDirectory(fontOutFolder);

    System.Diagnostics.Stopwatch sw = System.Diagnostics.Stopwatch.StartNew();

    Aspose.Pdf.Document document = new Aspose.Pdf.Document(inFile);
    int pageCount = document.Pages.Count;

    // Find all the fonts of the document
    FontAbsorber fa = new FontAbsorber();
    fa.Visit(document);

    FontCollection fc = fa.Fonts;
    List fontFiles = new List();

    // Save all the fonts in the cache folder
    int fontNum = 0;
    foreach (Pdf.Text.Font font in fc)
    {
        string cacheFontFile = string.Format(cacheFontFileTemplate, fontNum++);

        using (Stream fileStream = File.OpenWrite(cacheFontFile))
        {
            font.Save(fileStream);
        }
        fontFiles.Add(cacheFontFile);
    }

    int pageNumber = 0;
    // Split the document to separate pages to convert them in parallel
    foreach (Page pdfPage in document.Pages)
    {
        using (Document newDocument = new Document())
        {
            newDocument.Pages.Add(pdfPage);
            newDocument.Save(Path.Combine(testOut, String.Format(fileNameOnly + "_page{0}.pdf", pageNumber)));
        }
        pageNumber++;
    }
    document.Dispose();

    // Run conversion threads
    Thread[] threads = new Thread[pageCount];
    ThreadParam[] threadParams = new ThreadParam[pageCount];

    for (int i = 0; i < pageCount; i++)
    {
        threads[i] = new Thread(new ParameterizedThreadStart(Worker));
        threadParams[i] = new ThreadParam(i);
        threadParams[i].fontFiles = fontFiles;
        threads[i].Start(threadParams[i]);
    }

    // Wait threads to finish
    for (int i = 0; i < pageCount; i++)
    {
        threads[i].Join();
    }

    sw.Stop();
    Console.WriteLine(sw.Elapsed.TotalSeconds);
}

private void Worker(Object param)
{
    ThreadParam threadParam = (ThreadParam)param;
    Console.Out.WriteLine("started: " + threadParam.PageNum);

    try
    {
        using (Aspose.Pdf.Document pdfPageDocument = new Aspose.Pdf.Document(Path.Combine(testOut, String.Format(fileNameOnly + "_page{0}.pdf", threadParam.PageNum))))
        {
            Aspose.Pdf.HtmlSaveOptions htmlOptions = new Aspose.Pdf.HtmlSaveOptions();
            htmlOptions.SplitIntoPages = false;
            htmlOptions.FixedLayout = true;
            htmlOptions.FontSavingMode = HtmlSaveOptions.FontSavingModes.AlwaysSaveAsTTF;
            htmlOptions.CompressSvgGraphicsIfAny = false;
            htmlOptions.CustomResourceSavingStrategy = new HtmlSaveOptions.ResourceSavingStrategy(CacheFontsStrategy);

            // addtthe cached fonts as a font sources
            foreach (string fontFile in threadParam.fontFiles)
            {
                htmlOptions.FontSources.Add(new FileFontSource(fontFile));
            }
            htmlOptions.RasterImagesSavingMode = Aspose.Pdf.HtmlSaveOptions.RasterImagesSavingModes.AsExternalPngFilesReferencedViaSvg;

            string outputFileName = Path.GetFullPath(Path.Combine(testOut, String.Format(fileNameOnly + "_page{0}.html", threadParam.PageNum)));
            pdfPageDocument.Save(outputFileName, htmlOptions);

            outFileNames[threadParam.PageNum] = outputFileName;
        }
    }
    catch (Exception ex)
    {
        threadParam.isSuccess = false;
        Console.Out.WriteLine(ex.ToString());
    }
}

class ThreadParam
{
    public ThreadParam(int pageNum)
    {
        this.PageNum = pageNum;
        this.isSuccess = true;
    }
    public int PageNum;
    public List fontFiles;
    public bool isSuccess;
}

static object resourceSavingSync = new object();

/// 
/// Resource saving callback that saves fonts into output folder and builds css links to the fonts
/// 
private string CacheFontsStrategy(SaveOptions.ResourceSavingInfo resourceSavingInfo)
{
    // The callback is performed in parallel threads, so synchronization must be implemented
    lock (resourceSavingSync)
    {
        string fontsFolder = Path.GetFullPath(Path.Combine(testOut, fileNameOnly + "_fonts\\"));
        if (!Directory.Exists(fontsFolder))
            Directory.CreateDirectory(fontsFolder);

        // First path of this method is for saving of font
        if (resourceSavingInfo.ResourceType == SaveOptions.NodeLevelResourceType.Font)
        {
            string outFontFile = fontsFolder + Path.GetFileName(resourceSavingInfo.SupposedFileName);
            System.IO.BinaryReader fontBinaryReader = new BinaryReader(resourceSavingInfo.ContentStream);
            System.IO.File.WriteAllBytes(outFontFile,
                fontBinaryReader.ReadBytes((int)resourceSavingInfo.ContentStream.Length));
            string fontUrl = "../" + fileNameOnly + "_fonts/" + resourceSavingInfo.SupposedFileName;
            return fontUrl;
        }
        resourceSavingInfo.CustomProcessingCancelled = true;
        return null;
    }
}
} 
```

When the above-stated code is executed, the fonts are created only once, independent of output HTML files.

## Specify Image Format During PDF to HTML Export

Recently, we introduced a feature that allows developers to specify the image file format when exporting a PDF file to HTML format. In order to accomplish this feature, we added a new class named HtmlSaveOptions.RasterImagesSavingModes. The following code snippet shows how to select the target graphic format.

```
Aspose.Pdf.Document doc = new Document(@"c:\pdftest\36009.pdf");

HtmlSaveOptions options = new HtmlSaveOptions();
options.RasterImagesSavingMode = HtmlSaveOptions.RasterImagesSavingModes.AsEmbeddedPartsOfPngPageBackground;
// Next line is just to make view best for max amount of browsers
// You can coment it out if You will
options.FontSavingMode = HtmlSaveOptions.FontSavingModes.SaveInAllFormats;
doc.Save(@"c:\pdftest\36009.html", options);
```

When the above code is executed, the output folder will not contain any SVG files but only PNG files are generated (one PNG per page).

## PDF to Excel - Export All Pages to a Single Sheet

By default, when exporting PDF file to Excel format, each PDF page is converted to an individual Excel worksheet. However, we recently received a requirement for exporting all PDF pages to single worksheet in an Excel file. To accomplish this requirement, the following code snippet can be used

```
Document doc = new Document("Original.pdf");
ExcelSaveOptions options = new ExcelSaveOptions();
// Set this property to true
options.MinimizeTheNumberOfWorksheets = true;
doc.Save("output.xls", options);
```

## Set Table Columns Width as Per its Contents

Tables are one of the main objects when creating or manipulating PDF files. While creating a table object, we need to specify the columns width information using the Table.ColumnWidths property. However, we may want to auto-adjust the table columns width to fit the contents. In order to cater to this requirement, a new enumeration named ColumnAdjustment has been introduced. It contains the value AutoFitToContent. Please take a look at the following code snippet to accomplish this requirement.

```
string outFile = "36916.pdf";
// Added document
Document doc = new Document();
Page page = doc.Pages.Add();
// Create a table object and add it to the paragraphs collection of the section 
Table tab1 = new Table();
page.Paragraphs.Add(tab1);
// Set the column widths and default cell border of the table
tab1.ColumnAdjustment = ColumnAdjustment.AutoFitToContent;
tab1.ColumnWidths = "50 50 50";
tab1.DefaultCellBorder = new BorderInfo(BorderSide.All, 1F);
// Prepare an array of string values to be added to table
string[] data = new string[] { "Sample Text", "8.4", "Its test to set column width as per contnents" };
// Import the contents of the array created in above step
tab1.ImportArray(data, 0, 0, true);
// Save the resultant PDF
doc.Save(outFile);
```

## Create InkAnnotation with Stroke Ends as Rounded

By default, the stroke ends of InkAnnotation are square. However, recently we received a requirement to create InkAnnotation with rounded corners. In order to accomplish this requirement, the CapStyle property has been added to the InkAnnotation class. The CapStyle enumeration contains two values: CapStyle.Rectangular and CapStyle.Rounded. By default, InkAnnotation.CapStyle is set to CapStyle.Rectangular. To create rounded corner annotation, please use the following code snippet.

```
Document doc = new Document("PdfWithText.pdf");
Page pdfPage = doc.Pages[1];
System.Drawing.Rectangle drect = new System.Drawing.Rectangle();
drect.Height = (int)pdfPage.Rect.Height;
drect.Width = (int)pdfPage.Rect.Width;
drect.X = 0;
drect.Y = 0;
Aspose.Pdf.Rectangle arect = Aspose.Pdf.Rectangle.FromRect(drect);
ArrayList inkList = new ArrayList();
Aspose.Pdf.Point[] arrpt = new Aspose.Pdf.Point[3];
inkList.Add(arrpt);
arrpt[0] = new Point(100, 800);
arrpt[1] = new Point(200, 800);
arrpt[2] = new Point(200, 700);
InkAnnotation ia = new InkAnnotation(pdfPage, arect, inkList);
ia.Title = "XXX";
ia.Color = Aspose.Pdf.Color.LightBlue; // (GetColorFromString(stroke.InkColor));
ia.CapStyle = CapStyle.Rounded;
Border border = new Border(ia);
border.Width = 25;
ia.Opacity = 0.5;
pdfPage.Annotations.Add(ia);
doc.Save("37071.pdf");
```

## Show Note on Mouseover Event

Recently one of our customers wanted to create an annotation that would appear when a user moused over some text or image. To accomplish this, some enhancements have been made to the API. Now you can make popup window notes which appear on mouseover or other events you need. Please try using the following code snippet:

```
/*Declaring of parameters*/
// Unique name of annotation
string name = "IMDB0145487";
// Title of popup window
string title = "Spider-Man";
// Description that be in popup window
string comment = "Movie produced in 2002; run length: 121";
// Path to image for that popup window will appeared on mouse over
string imagePath = (TestSettings.GetInputFile("36228.jpg"));
// Position of image on page of document
Aspose.Pdf.Rectangle imageRect = new Aspose.Pdf.Rectangle(2, 700, 97, 840);
// Position of popup on page of document
Aspose.Pdf.Rectangle popupRect = new Aspose.Pdf.Rectangle(90, 610, 235, 710);

/*Document creating*/
Document doc = new Document();
doc.Pages.Add();
// Page for adding of image
Page page = doc.Pages[1];

/*Add image on page*/
// Load image into stream
FileStream imageStream = new FileStream(imagePath, FileMode.Open);
// Add image to Images collection of Page Resources
page.Resources.Images.Add(imageStream);
// Using GSave operator: this operator saves current graphics state
page.Contents.Add(new Operator.GSave());
// Create Rectangle and Matrix objects
Aspose.Pdf.DOM.Matrix matrix =
    new Aspose.Pdf.DOM.Matrix(new double[]
    {
        imageRect.URX - imageRect.LLX, 0, 0, imageRect.URY - imageRect.LLY, imageRect.LLX, imageRect.LLY
    });
// Using ConcatenateMatrix (concatenate matrix) operator: defines how image must be placed
page.Contents.Add(new Operator.ConcatenateMatrix(matrix));
XImage ximage = page.Resources.Images[page.Resources.Images.Count];
// Using Do operator: this operator draws image
page.Contents.Add(new Operator.Do(ximage.Name));
// Using GRestore operator: this operator restores graphics state
page.Contents.Add(new Operator.GRestore());

/*Add text annotation*/
TextAnnotation text = new TextAnnotation(page, imageRect);
text.Name = name;
text.Title = title;
text.Contents = comment;
// This flags must be raised to suppress showing of annotation icon
text.Flags = AnnotationFlags.NoView|AnnotationFlags.ReadOnly;
page.Annotations.Add(text);

/*Add popup annotation*/
PopupAnnotation popup = new PopupAnnotation(page, popupRect);
page.Annotations.Add(popup);

/*Link text and popup annotations*/
text.Popup = popup;
popup.Parent = text;

/*Add button*/
Field field = new ButtonField(page, imageRect);
doc.Form.Add(field);

/*Set ButtonField actions*/
string fieldName = field.PartialName;
string openScript =
    "var t = this.getAnnot(this.pageNum, '" + name + "'); t.popupOpen = true; var w = this.getField('" + fieldName + "'); w.setFocus();";
string closeScript = "var t = this.getAnnot(this.pageNum, '" + name + "'); t.popupOpen = false;";
field.Actions.OnEnter = new JavascriptAction(openScript);
field.Actions.OnExit = new JavascriptAction(closeScript);

/*Save document*/
doc.Save(TestSettings.GetOutputFile("36228.pdf")); 
```

As well as the above features, there have been numerous enhancements in the recent release of Aspose.PDF for .NET. One of the enhancements include adding a default value to the PageLayout enumeration. To do this, the PageLayout.Default value has been added. Various improvements related to XPS to PDF conversion, PDF to XPS conversion, PDF file optimization, concatenation of PDF file, HTML to PDF conversion, PDF to DOC conversion, PDF to HTML, PDF to image, SVG to PDF, CGM to PDF conversion, image and text manipulation, addition of TOC and much more. In short, this release includes fixes for around 90 issues and is a major release. Please go ahead, download and start exploring the new release of [Aspose.PDF for .NET 9.4.0.][3]




[1]: http://groupdocs.com/apps
[2]: https://downloads.aspose.com/pdf/net
[3]: https://downloads.aspose.com/pdf/net




