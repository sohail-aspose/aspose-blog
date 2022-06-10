---
title: 'Insert Page Break, Set User Agent String, Stream Parameter in PDF to HTML Conversion with Aspose.PDF for .NET 10.0.0'
date: Fri, 30 Jan 2015 12:32:24 +0000
draft: false
url: /2015/01/30/insert-page-break-in-existing-pdf-setting-user-agent-string-support-of-stream-parameter-in-pdf-to-html-conversion-with-aspose.pdf-for-.net-10.0.0/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'Convert HTML to PDF with user-agent', 'Insert page breaks in PDF documents in Csharp', 'Use Stream Parameter in PDF to HTML']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net_100.png" alt="Aspose.Pdf for .NET logo">}}


The latest release of [Aspose.PDF for .NET 10.0.0][1] has hit the download section. This new release provides some great features like insertion of Page Break inside an existing PDF file, Setting of User-agent string, Setting Header and Footer once for the newly created PDF document or enhancement for CutomeHtmlSavingStrategy to support Stream instance as in earlier release, this property has not been supported.

## Page Break in Existing PDF

As a default layout, the contents inside PDF files are added in Top-Left to Bottom-Right layout. Once the contents exceed beyond page bottom margin, the page break occurs. However, you may come across a requirement to insert page break depending upon the requirement. In order to accomplish this requirement, a method named AddPageBreak(...) method is added in the PdfFileEditor class to accomplish this requirement. For further details, please visit [Page Break in Existing PDF][2].

```
// instantiate Document instance
Document doc = new Document("source.pdf");
// instantiate blank Document instance
Document dest = new Document();
// create PdfFileEditor object
PdfFileEditor fileEditor = new PdfFileEditor();
fileEditor.AddPageBreak(doc, dest, new PdfFileEditor.PageBreak\[\] 
{ 
    new PdfFileEditor.PageBreak(1, 450) 
});
// save resultant file
dest.Save("dest.pdf");

```

## Convert HTML to PDF - Setting User-Agent string

When converting HTML files to PDF format, we may come across a scenario where we may have a dynamic page that generates an image based on the information provided in the query string and in order to properly add images in resultant PDF, the source website requires user agent string for images. In order to accomplish this requirement, **UserAgentNameOfFileWebRequests** is added to Aspose.Pdf.Generator.Pdf class.

```
internal  static void OnWebRequestIssuedHandler(Pdf.WebFileRequestCreatedEventInfo eventInfo)
{
    if (eventInfo.PreparedRequest is System.Net.HttpWebRequest)
    {
        System.Net.HttpWebRequest asHttpRequest = (System.Net.HttpWebRequest)eventInfo.PreparedRequest;
        Console.WriteLine("Issued request to '" + eventInfo.PreparedRequest.RequestUri + "'");
        Console.WriteLine("Used user agent string is '" + asHttpRequest.UserAgent + "'");
            //Assert.AreEqual(asHttpRequest.UserAgent, "Test user agent Aspose.Pdf.9.9");
    }
}

static void RunTest() {
    string html = string.Format(@"

    
        < h1>Image load test
        < p>Following image NOT loading:
```
```
        < img src='http://staging.programworkshop.com/itdversions/8.6.0.0/itdmedia.aspx?data=40&AUC=1&programid=40&language=ENU&urid=07064/ETS\_MFT\_4C\_sm2.gif' />
        < p>Following image loading:
```
```
        < img src='http://upload.wikimedia.org/wikipedia/commons/thumb/4/44/PIA16934-RoverDistances-20130515.jpg/355px-PIA16934-RoverDistances-20130515.jpg' />
    
");

Pdf pdf = new Pdf();
Section section = pdf.Sections.Add();

Text text2 = new Text(section, html);
text2.IsHtmlTagSupported = true;
section.Paragraphs.Add(text2);

Pdf.UserAgentNameOfFileWebRequests = "Test user agent Aspose.Pdf 10.0";
Pdf.WebFileRequestCreatedDelegate handler = new Pdf.WebFileRequestCreatedDelegate(OnWebRequestIssuedHandler);
Pdf.WebFileRequestCreated += handler;

MemoryStream outstream = new MemoryStream();
pdf.Save(outstream);

Console.ReadLine(); 

```

## PDF to HTML - Support Stream Parameter in CustomeHtmlSavingStrategy

The earlier release versions of Aspose.Pdf for .NET provide the feature to use a static stream variable for stream passage from caller object and return, however, one of the customers requested the possibility to pass a ref stream as an argument to the function SavingToStream(HtmlSaveOptions.HtmlPageMarkupSavingInfo htmlSavingInfo). Please note that the method specified below cannot be changed; just to add some additional parameters since the delegate of this method must be passed to _CustomHtmlSavingStrategy_.

```
private static void SavingToStream(HtmlSaveOptions.HtmlPageMarkupSavingInfo htmlSavingInfo)
{
}
```

However, the goal (saving of several output documents to same static output stream) can easily be achieved with the following code snippet where we only need to change a bit custom handler of output saving. Please take a look over the following code snippet.

```
// it can be any writable stream, file stream used only as example    
static Stream \_staticOutStream = File.OpenWrite(@"F:\\ExternalTestsData\\static\_stream\_out.html");

public static void PDFtoStaticHTMLStream\_37952()
{
    Document doc = new Document(@"F:\\ExternalTestsData\\HelloWorld.pdf");

    // tune conversion params for first saving
    HtmlSaveOptions newOptions = new HtmlSaveOptions();
    newOptions.RasterImagesSavingMode = HtmlSaveOptions.RasterImagesSavingModes.AsEmbeddedPartsOfPngPageBackground;
    newOptions.FontSavingMode = HtmlSaveOptions.FontSavingModes.SaveInAllFormats;
    newOptions.PartsEmbeddingMode = HtmlSaveOptions.PartsEmbeddingModes.EmbedAllIntoHtml;
    newOptions.LettersPositioningMethod = HtmlSaveOptions.LettersPositioningMethods.UseEmUnitsAndCompensationOfRoundingErrorsInCss;
    newOptions.SplitIntoPages = false;// force write HTMLs of all pages into one output document
    newOptions.CustomHtmlSavingStrategy = new HtmlSaveOptions.HtmlPageMarkupSavingStrategy(SavingToStaticStream);

    //we can use some non-existing puth as result file name - all real saving will be done
    //in our custom method SavingToStream() (it's follows this one)
    string outHtmlFile = @"Z:\\SomeNonExistingFolder\\HelloWorld.html";
    doc.Save(outHtmlFile, newOptions);

    // 2) saving one more document in same stream(saving will really take place in SavingToStaticStream() method)
    Document doc\_2 = new Document(@"F:\\ExternalTestsData\\Test1.pdf");

    // 2.1)tune conversion params
    HtmlSaveOptions newOptions2 = new HtmlSaveOptions();
    newOptions2.RasterImagesSavingMode = HtmlSaveOptions.RasterImagesSavingModes.AsEmbeddedPartsOfPngPageBackground;
    newOptions2.FontSavingMode = HtmlSaveOptions.FontSavingModes.SaveInAllFormats;
    newOptions2.PartsEmbeddingMode = HtmlSaveOptions.PartsEmbeddingModes.EmbedAllIntoHtml;
    newOptions2.LettersPositioningMethod = HtmlSaveOptions.LettersPositioningMethods.UseEmUnitsAndCompensationOfRoundingErrorsInCss;
    newOptions2.SplitIntoPages = false;// force write HTMLs of all pages into one output document
    newOptions2.CustomHtmlSavingStrategy = new HtmlSaveOptions.HtmlPageMarkupSavingStrategy(SavingToStaticStream);
            
    // 2.2)start saving itself
    outHtmlFile=@"Z:\\SomeNonExistingFolder\\Test1.html";
    doc\_2.Save(outHtmlFile, newOptions);

    // 
    Console.ReadKey();
}

private static void SavingToStaticStream(HtmlSaveOptions.HtmlPageMarkupSavingInfo htmlSavingInfo)
{
    Console.WriteLine("Starting saving to static stream of output HTML document '" +htmlSavingInfo.SupposedFileName + "' ...");

    byte\[\] resultHtmlAsBytes = new byte\[htmlSavingInfo.ContentStream.Length\];
    htmlSavingInfo.ContentStream.Read(resultHtmlAsBytes, 0, resultHtmlAsBytes.Length);

    // locking allows to ensure that saving to static stream 
    // goes from one thread a time and allows avoid interference 
    // between different threads(if any) during saving to same output thread

    lock (\_staticOutStream)
    {
        \_staticOutStream.Write(resultHtmlAsBytes, 0, resultHtmlAsBytes.Length);
    }
    Console.WriteLine("Output HTML document '" + htmlSavingInfo.SupposedFileName + "' has been successfully saved to static stream.");
}
```

As well as the enhancements and features discussed above, there has been a specific improvement for PDF to HTML and HTML conversion feature. Among these fixes, the PCL to PDF, PDF to TIFF conversion, conversion of PDF to PDF/A compliant documents, text replacement, rendering PDF files to XPS format is also improved. Please download and try the latest release of [Aspose.PDF for .NET 10.0.0][3].




[1]: https://downloads.aspose.com/pdf/net
[2]: https://docs.aspose.com/display/pdfnet/Working+with+Document+-+Facades#WorkingwithDocument-Facades-PageBreakinexistingPDF
[3]: https://downloads.aspose.com/pdf/net




