---
title: 'Specify Character Spacing for Text in PDF using C#'
date: Mon, 23 Feb 2015 13:28:38 +0000
draft: false
url: /2015/02/23/specify-character-spacing-for-text-in-pdf-using-csharp-asp.net/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'Specify Character Spacing for Text in PDF']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net_100.png" alt="Aspose.Pdf for .NET logo">}}


The new release version of [Aspose.PDF for .NET 10.1.0][1] has been released with new features. With every new release, the demanding features from our customers are made available and keeping the tradition alive, we have introduced some useful features, as well as fixes for issues reported in earlier release versions.

## Specify Character Spacing for Text in PDF

A text can be added inside paragraphs collection of PDF files using **TextFragment** instance or by using **TextParagraph** object and even you can stamp the text inside PDF by using **TextStamp** class. While adding the text, we may have a requirement to specify character spacing for the text. In order to accomplish this requirement, a new property named **CharacterSpacing** has been introduced. Please take a look over the following approaches to fulfill this requirement. For more information, please visit How to specify character Spacing when adding Text.

### Using TextBuilder and TextFragment

{{< gist aspose-pdf 7e1330795d76012fcb04248bb81d45b3 "Examples-CSharp-AsposePDF-Text-SpecifyCharacterSpacing-UsingTextBuilderAndFragment.cs" >}}

### Using TextParagraph

{{< gist aspose-pdf 7e1330795d76012fcb04248bb81d45b3 "Examples-CSharp-AsposePDF-Text-SpecifyCharacterSpacing-UsingTextBuilderAndParagraph.cs" >}}

### Using TextStamp

{{< gist aspose-pdf 7e1330795d76012fcb04248bb81d45b3 "Examples-CSharp-AsposePDF-Text-SpecifyCharacterSpacing-UsingTextStamp.cs" >}}

### Using Aspose.Pdf.Generator Object

The **TextInfo** object already supports the feature to specify characters spacing using **CharSpace** property and this requirement can be accomplished by using the following code snippet but we still recommend using a new Document Object Model of Aspose.Pdf namespace as all the enhancements and updates are being made in new DOM approach.

```
Aspose.Pdf.Generator.Pdf pdf1 = new Aspose.Pdf.Generator.Pdf();

//Create a new section in the Pdf object
Aspose.Pdf.Generator.Section sec1 = pdf1.Sections.Add();

//Add 1st paragraph (inheriting the text format settings from the section)
//to the section 
sec1.Paragraphs.Add(new Aspose.Pdf.Generator.Text(sec1, "This is generator text paragraph with default character spacing"));

Aspose.Pdf.Generator.Section sec2 = pdf1.Sections.Add();

//Create 2nd paragraph (inheriting the text format settings from the section) 
Aspose.Pdf.Generator.Text t2 = new Aspose.Pdf.Generator.Text(sec1);

//Create a segment "seg1" in the paragraph "t2"
Aspose.Pdf.Generator.Segment seg1 = new Aspose.Pdf.Generator.Segment(t2);
//Assign some content to the segment
seg1.Content = "This is generator text paragraph with increased character spacing";
//Set character spacing of the segment to 2.0
seg1.TextInfo.CharSpace = 2.0f;

//Add segment (with character spacing) to the paragraph
t2.Segments.Add(seg1);
//Add 2nd text paragraph to the section with overridden text format settings
sec1.Paragraphs.Add(t2);

//save the document
pdf1.Save(outFile);
```

## Determine License Initialization

When using the API in trial mode, you get the limitations to manipulate/add a certain number of elements inside a PDF file. The limitation includes adding/removing the number of pages from PDF file, adding/manipulating Attachments or Annotations inside PDF file, conversion of only the first 4 pages to Image format and so on. Also when using the API in trial mode (without using the license), a watermark text is added in the resultant file and you also come across an error message stating that API is being used in evaluation mode. So before performing any operation, we can also check the license initialization and for this purpose, a static read-only property named IsLicensed is added in Document class.

```
// determine if the API is licensed
if (Document.IsLicensed)
{
    // print message that license is applied
    Console.WriteLine("Licensed");
}
```

We generate the PDF files on the fly and during PDF file creation, we may come across the requirement (creating Table Of Contents, etc) to get page count of PDF file without saving the file over system or stream. So in order to cater to this requirement, a method ProcessParagraphs(...) has been introduced in Document class. Please take a look over the following code snippet which shows the steps to get page count without saving the document. For further information, please visit [Get Number of Pages in a PDF File][2]

## TextStamp Rotation

Adding text stamps inside PDF file is one of the salient features of our API and while adding Text Stamp, we may have a requirement to rotate the text stamp. In order to accomplish this requirement, a property named **RotateAngle** is present inside the TextStamp class. You can pass any angle value which can be applied to rotate Stamp instance. Please take a look over the following code snippet which illustrates the steps to rotate TextStamp at 45-degree angle when placing it inside PDF file.

```
//open document
Document pdfDocument = new Document();
pdfDocument.Pages.Add();
//create text stamp
TextStamp textStamp = new TextStamp("Sample Stamp");
//set whether stamp is background
textStamp.Background = (true);
//set origin
textStamp.XIndent = (100);
textStamp.YIndent = (100);
//rotate stamp at 45 degree
textStamp.RotateAngle = 45;
//set text properties
textStamp.TextState.Font = FontRepository.FindFont("Arial");
textStamp.TextState.FontSize = (14.0F);
textStamp.TextState.FontStyle = (FontStyles.Bold);
textStamp.TextState.FontStyle = (FontStyles.Italic);
textStamp.TextState.ForegroundColor = (Aspose.Pdf.Color.Green);
//add stamp to particular page
pdfDocument.Pages[1].AddStamp(textStamp);
//save output document
pdfDocument.Save("TextStamp_output.pdf");
```

## PDF to DOC - Paragraph Break after Each Paragraph

Recently one of the customers reported an issue where paragraph break was being added at the end of each line instead of adding it at the end of the paragraph. In order to cater this requirement, a new property named **AddReturnToLineEnd** is added in DocSaveOptions class. Please take a look at the following code snippet.

```
// load input PDF
Aspose.Pdf.Document document = new Document("source.pdf");
// instantiate DocSave instance to save output in MS Word format
Aspose.Pdf.DocSaveOptions saveOptions = new Aspose.Pdf.DocSaveOptions();
// specify output format as DOCX
saveOptions.Format = DocSaveOptions.DocFormat.DocX;
// set the mode of contents as Flow
saveOptions.Mode = Aspose.Pdf.DocSaveOptions.RecognitionMode.Flow;
// donot add paragraph break at end of each line
saveOptions.AddReturnToLineEnd = false;
// save output as DOCX format
document.Save("Resultant.docx", SaveFormat.DocX);
```

As well as the enhancements and features discussed above, there has been a specific improvement for PDF to HTML and HTML to PDF conversion features. Among these fixes, the PCL to PDF, SVG to PDF, PDF to Excel, PDF to TIFF and TIFF to PDF conversion, conversion of PDF to PDF/A compliant documents, text replacement, rendering PDF files to XPS format are also improved. Please download and try the latest release of [Aspose.PDF for .NET 10.1.0][3].




[1]: https://downloads.aspose.com/pdf/net
[2]: https://docs.aspose.com/display/pdfnet/Get+and+Set+Page+Properties
[3]: https://downloads.aspose.com/pdf/net




