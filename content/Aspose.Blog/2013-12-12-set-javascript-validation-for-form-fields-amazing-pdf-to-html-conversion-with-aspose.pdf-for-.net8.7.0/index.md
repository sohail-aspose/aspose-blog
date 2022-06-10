---
title: 'JavaScript Validation for Form Fields &amp; Improved PDF to HTML Conversion'
date: Thu, 12 Dec 2013 19:56:56 +0000
draft: false
url: /2013/12/12/set-javascript-validation-for-form-fields-amazing-pdf-to-html-conversion-with-aspose.pdf-for-.net8.7.0/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net_100.png" alt="Aspose.Pdf for .NET logo">}}


We have introduced a new feature in Aspose.Pdf for .NET which allows developers to ensure that only numeric values are entered in form fields. The properties OnModifyCharacter and OnFormat properties have been added to Field.Actions. To validate a user entry, the AFNumber\_Keystroke and AFNumber\_Format Java script functions may be used. Please take a look over following code snippet.

```
// Load input PDF file
Document doc = new Document("c:/pdftest/ABFillablewfields.pdf");
TextBoxField field = (TextBoxField)doc.Form\["husband name"\];
// http://www.adobe.com/content/dam/Adobe/en/devnet/acrobat/pdfs/FormsAPIReference.pdf
// 2 digits after point
// No separator
// Neg style = minus
// No currency
field.Actions.OnModifyCharacter = new JavascriptAction("AFNumber\_Keystroke(2, 1, 1, 0, \\"\\", true)");
field.Actions.OnFormat = new JavascriptAction("AFNumber\_Format(2, 1, 1, 0, \\"\\", true)");
// Set initial field value
field.Value = "123";
// Save resultant PDF
doc.Save("c:/pdftest/Restricted\_out.pdf");

```

## Saving Images in Raster Format when Converting to HTML

Aspose.Pdf for .NET has great features for converting PDF files to DOC, DOCX, image, HTML and various other formats. During the PDF to HTML conversion process, images in PDF files are saved with SVG compression but you might want to save them in raster format - PNG or JPEG - instead to reduce image size.

```
// Source PDF file
Document doc = new Document("c:/input.pdf");
// Create HtmlSaveOption with tested feature
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
saveOptions.FixedLayout = true;
saveOptions.SplitIntoPages = false;
saveOptions.RasterImagesSavingMode = HtmlSaveOptions.RasterImagesSavingModes.AsExternalPngFilesReferencedViaSvg;

string outFile = "c:/ResultantFile.pdf";
// Save the output in HTML format
doc.Save(outFile, saveOptions);

```

## Split CSS to Pages During PDF to HTML Conversion

The HtmlSaveOptions class has a property, SplitIntoPages, which lets you split an HTML file to pages when generating the output. Recently, a customer had the requirement to split the CSS file based on individual pages instead of generating a single CSS file. To accomplish this requirement, we have introduced a new flag, SplitCssIntoPages, in the HtmlSaveOptions class. When the value of this property is set to true, the converter splits the CSS into parts/pages based on the individual HTML page created. Please take a look at the following code snippet.

```
//1) Clean-up target folders
string htmlFile = Path.GetFullPath("c:/pdftest/ResultantFile\_files/" + "resultant.html");
string imagesDir = Path.GetDirectoryName(htmlFile) + @"\\35942\_files";
string cssDir = Path.GetDirectoryName(htmlFile) + @"\\35942\_css\_files";
if (Directory.Exists(imagesDir)) { Directory.Delete(imagesDir, true); };
if (Directory.Exists(cssDir)) { Directory.Delete(cssDir, true); };

//2) Create document for conversion
Document pdfDocument = new Document("c:/pdftest/antrag.pdf");

//3) Tune conversion options
HtmlSaveOptions options = new HtmlSaveOptions();
options.RasterImagesSavingMode = HtmlSaveOptions.RasterImagesSavingModes.AsPngImagesEmbeddedIntoSvg;//<- to get compatibility with previous behavior and therefore same result of tests
// Split HTML output into pages
options.SplitIntoPages = true;
// Split CSS into pages
options.SplitCssIntoPages = true;
options.CustomCssSavingStrategy = new HtmlSaveOptions.CssSavingStrategy(Strategy\_4\_CSS\_MULTIPAGE\_SAVING\_RIGHT\_WAY);
options.CustomStrategyOfCssUrlCreation = new HtmlSaveOptions.CssUrlMakingStrategy(Strategy\_5\_CSS\_MAKING\_CUSTOM\_URL\_FOR\_MULTIPAGING);
//3) Convert
pdfDocument.Save(htmlFile, options);

private static void Strategy\_4\_CSS\_MULTIPAGE\_SAVING\_RIGHT\_WAY(HtmlSaveOptions.CssSavingInfo partSavingInfo)
{
    string cssOutFolder = @"c:\\pdftest\\ResultantFile\_files\\";
    if (!Directory.Exists(cssOutFolder))
    {
        Directory.CreateDirectory(cssOutFolder);
    }

    string outPath = cssOutFolder + "style\_xyz\_page" + partSavingInfo.HtmlPageNumber.ToString() + ".css";
    System.IO.BinaryReader reader = new BinaryReader(partSavingInfo.ContentStream);
    System.IO.File.WriteAllBytes(outPath, reader.ReadBytes((int)partSavingInfo.ContentStream.Length));
}
private static string Strategy\_5\_CSS\_MAKING\_CUSTOM\_URL\_FOR\_MULTIPAGING(HtmlSaveOptions.CssUrlRequestInfo requestInfo)
{
    return "/document-viewer/GetCss?cssId=4544554445\_page{0}";
}

```

## Determine Field Properties

During PDF form creation, some fields are marked as mandatory and we might need to determine if a particular field is marked as such. Please try using the following code snippet to find out if a field is marked as required.

```
// Load source PDF file
Document pdf = new Document(@"c:\\pdftest\\RequiredField\_output.pdf");
// Instantiate Form object
Aspose.Pdf.Facades.Form pdfForm = new Aspose.Pdf.Facades.Form(pdf);
// Iterate through each field inside PDF form
foreach (Field field in pdf.Form.Fields)
{
    // Determine if the field is marked as required or not
    bool isRequired = pdfForm.IsRequiredField(field.FullName);
    if (isRequired)
    {
        // Print either the field is marked as required or not
        Console.WriteLine("The field named " + field.FullName + " is required");
    }
}

```

## Enhancements

We have enhanced numerous features. The following section highlights some of the enhancements introduced in this release

*   PDF to HTML conversion - Extract images, fonts and CSS in separate folders and create aliases.
*   PDF to HTML conversion - Convert non-vector SVG elements to PNG/JPG.
*   PDF to HTML conversion - Shorten font names.
*   Add JavaScript to push button using Aspose.Pdf.Generator.
*   Mark the Producer and Creator properties of DocumentInfo to read only.
*   PDF generation time is optimized compared to previous releases.
*   Better PDF to XPS and image rendering.

Explore the new features in [Aspose.Pdf for .NET 8.7.0][1].




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.pdf-for-.net/entry512052.aspx




