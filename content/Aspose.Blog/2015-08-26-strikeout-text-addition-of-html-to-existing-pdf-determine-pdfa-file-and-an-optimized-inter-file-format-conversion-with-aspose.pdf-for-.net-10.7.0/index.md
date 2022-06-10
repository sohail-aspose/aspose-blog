---
title: 'Strikeout Text, addition of HTML to existing PDF, determine PDF/A file and an optimized inter file format conversion with Aspose.PDF for .NET 10.7.0'
date: Wed, 26 Aug 2015 21:17:58 +0000
draft: false
url: /2015/08/26/strikeout-text-addition-of-html-to-existing-pdf-determine-pdfa-file-and-an-optimized-inter-file-format-conversion-with-aspose.pdf-for-.net-10.7.0/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'Add HTML to PDF in Csharp', 'Strikeout text in PDF documents .net', 'Strikeout text in PDF documents programmatically', 'Validate PDF/A compliant document']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net_100.png" alt="PDF API for .NET">}}


A new release of [Aspose.PDF for .NET 10.7.0][1] has been published with new features and enhancements which were requested in earlier release versions. Likewise previous versions, this new release also contains fixes for issues reported against previous releases. The following are some details regarding features introduced in this new release.

## Strikeout feature in TextState class

The TextState class provides the capabilities to set formatting for TextFragments being placed inside PDF document. You can use this class to set text formatting as Bold, Italic, Underline and starting this release, the API has provided the capabilities to mark text formatting as Strikeout. Please try using following code snippet to add TextFragment with Strikeout formatting. Meanwhile you may consider visiting following link for further details on [Add Text in existing PDF file][2]

```
//open document
Document pdfDocument = new Document();
//get particular page
Page pdfPage = (Page)pdfDocument.Pages.Add();

//create text fragment
TextFragment textFragment = new TextFragment("main text");
textFragment.Position = new Position(100, 600);

//set text properties
textFragment.TextState.FontSize = 12;
textFragment.TextState.Font = FontRepository.FindFont("TimesNewRoman");
textFragment.TextState.BackgroundColor = Aspose.Pdf.Color.LightGray;
textFragment.TextState.ForegroundColor = Aspose.Pdf.Color.Red;
//set StrikeOut property
textFragment.TextState.StrikeOut = true;
// mark text as Bold
textFragment.TextState.FontStyle = FontStyles.Bold;

// create TextBuilder object
TextBuilder textBuilder = new TextBuilder(pdfPage);
// append the text fragment to the PDF page
textBuilder.AppendText(textFragment);
//save document
pdfDocument.Save(outFile);
```

## Add HTML contents to existing PDF document

Aspose.Pdf for .NET provides the capabilities to [Convert HTML to PDF Format][3], as well as the feature to [Add Text in an Existing PDF File][4]. However with this release, we have also introduced the feature to add HTML contents inside PDF document where HTML tags will be rendered accordingly, instead they appear as static HTML tags.

```
//open document
Document pdfDocument = new Document();
string outFile = "33851.pdf";
// create HTML Fragment object to speicfy the HTML contents which need to be added
HtmlFragment t = new HtmlFragment(" < body style='line-height: 100px;'>First line of textSecond Line of Text
```

*   First
*   Second
*   Third
*   Fourth
*   Fifth

```
Text after the list.Next lineLast line ");
// add page to pages collection of Document instance
Page page = pdfDocument.Pages.Add();
// add HTML fragment to paragraphs collection of page
page.Paragraphs.Add(t);
// save output file
pdfDocument.Save(outFile);
```

## Determine of the document is PDF/A file

Aspose.Pdf for .NET provides the feature to [convert PDF file to PDF/A format][5], [convert PDF/A file to PDF format][6] and the feature to [Validate if PDF document is PDF/A compliant][7]. It also offers the capabilities to determine if loaded document is a valid PDF and also if its encrypted or not. In order to further extend the capabilities of Document class, **IsPdfaCompliant** property is added to determine if input file is PDF/A compliant and a property named **PdfaFormat** to identify the PDF/A format are introduced.

## [Footnote enhancement in DOM approach][8]

In earlier release versions, the Footnote support has been provided but it was only applicable to TextFragment object. However now you can also add Footnote to other objects inside PDF document such as Table, Cells etc. The following code snippet shows the steps to add Footnote to TextFragment object and then add table to paragraphs collection of Footnote section.

```
string outXml = TestSettings.GetOutputFile("38614.xml");
string inFile = TestSettings.GetInputFile("..//new_Logo.bmp");
string outFile = TestSettings.GetOutputFile("38614.pdf");
Document doc = new Document();
Page page = doc.Pages.Add();
TextFragment text = new TextFragment("some text");
Aspose.Pdf.Image image = new Aspose.Pdf.Image();
image.File = inFile;
image.FixHeight = 20;
page.Paragraphs.Add(text);

text.FootNote = new Note();
text.FootNote.Paragraphs.Add(image);
TextFragment footNote = new TextFragment("footnote text");
footNote.TextState.FontSize = 20;
footNote.IsInLineParagraph = true;
text.FootNote.Paragraphs.Add(footNote);
Aspose.Pdf.Table table = new Aspose.Pdf.Table();
table.Rows.Add().Cells.Add().Paragraphs.Add(new TextFragment("Row 1 Cell 1"));
text.FootNote.Paragraphs.Add(table);
doc.SaveXml(outXml);
doc = new Document();
doc.BindXml(outXml);
doc.Save(outFile); 
```

## TabStops for Text objects using DOM

A Tab Stop is a stopping point for tabbing. In word processing, each line contains a number of tab stops placed at regular intervals (for example, every half inch). They can be changed, however, as most word processors allow you to set tab stops wherever you want. When you press the Tab key, the cursor or insertion point jumps to the next tab stop, which itself is invisible. Although tab stops do not exist in the text file, the word processor keeps track of them so that it can react correctly to the Tab key. For further details, please visit [Working with Custom Tab stops][9]

```
Document _pdfdocument = new Document();
Page page = _pdfdocument.Pages.Add();

Aspose.Pdf.Text.TabStops ts = new Aspose.Pdf.Text.TabStops();
Aspose.Pdf.Text.TabStop ts1 = ts.Add(100);
ts1.AlignmentType = TabAlignmentType.Right;
ts1.LeaderType = TabLeaderType.Solid;
Aspose.Pdf.Text.TabStop ts2 = ts.Add(200);
ts2.AlignmentType = TabAlignmentType.Center;
ts2.LeaderType = TabLeaderType.Dash;
Aspose.Pdf.Text.TabStop ts3 = ts.Add(300);
ts3.AlignmentType = TabAlignmentType.Left;
ts3.LeaderType = TabLeaderType.Dot;

TextFragment header = new TextFragment("This is a example of forming table with TAB stops", ts);
TextFragment text0 = new TextFragment("#$TABHead1 #$TABHead2 #$TABHead3", ts);
text0.TextState.FontStyle = FontStyles.Bold;
TextFragment text1 = new TextFragment("#$TABdata11 #$TABdata12 #$TABdata13", ts);
TextFragment text2 = new TextFragment("#$TABdata21 ", ts);
text2.Segments.Add(new TextSegment("#$TAB"));
text2.Segments.Add(new TextSegment("data22 "));
text2.Segments.Add(new TextSegment("#$TAB"));
text2.Segments.Add(new TextSegment("data23"));

page.Paragraphs.Add(header);
page.Paragraphs.Add(text0);
page.Paragraphs.Add(text1);
page.Paragraphs.Add(text2);

_pdfdocument.Save(outFile); 
```

## Miscellaneous fixes

As well as the enhancements and features discussed above, there has been a specific improvement for PDF to HTML and HTML to PDF conversion features with better support for HTML5. Among these fixes, the PCL to PDF, SVG to PDF, PDF to Excel, PDF to DOC, PDF to TIFF and TIFF to PDF conversion, conversion of PDF to PDF/A compliant documents, text replacement, Filling of signature field with an image, flattening of PDF and rendering of PDF to XPS format, FloatingBox rendering, Footnote, EndNote and rendering of non-English (specifically Arabic) contents are also improved. Please download and try the latest release of [Aspose.PDF for .NET 10.7.0][10].




[1]: https://downloads.aspose.com/pdf/net
[2]: http://docs.aspose.com/display/pdfnet/Add+Text+in+an+Existing+PDF+File
[3]: http://docs.aspose.com/display/pdfnet/Convert+HTML+to+PDF+Format
[4]: http://docs.aspose.com/display/pdfnet/Add+Text+in+an+Existing+PDF+File
[5]: http://docs.aspose.com/display/pdfnet/Convert+PDF+File+to+PDF-A
[6]: https://docs.aspose.com/display/pdfnet/Convert+PDF-A+to+PDF
[7]: https://docs.aspose.com/display/pdfnet/Manipulate+PDF+Document#ManipulatePDFDocument-ValidatePDFDocumentforPDFAStandard(A1AandA1B)
[8]: https://docs.aspose.com/display/pdfnet/Add+Text+to+a+PDF+file#AddTexttoaPDFfile-FootNotesandEndNotes(DOM)
[9]: https://docs.aspose.com/display/pdfnet/Add+Text+to+a+PDF+file#AddTexttoaPDFfile-WorkingwithcustomTabStops
[10]: https://downloads.aspose.com/pdf/net




