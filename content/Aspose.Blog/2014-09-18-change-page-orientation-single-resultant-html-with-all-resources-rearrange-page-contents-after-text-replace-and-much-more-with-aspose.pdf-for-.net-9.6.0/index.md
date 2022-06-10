---
title: 'Change Page Orientation, Single Output HTML with All Resources, Rearrange Page Contents After Replacing Text and More in Aspose.PDF for .NET 9.6.0'
date: Thu, 18 Sep 2014 11:51:37 +0000
draft: false
url: /2014/09/18/change-page-orientation-single-resultant-html-with-all-resources-rearrange-page-contents-after-text-replace-and-much-more-with-aspose.pdf-for-.net-9.6.0/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net_100.png" alt="Aspose.Pdf for .NET logo">}}


We are very much excited to announce the release of [Aspose.PDF for .NET 9.6.0][1] which provides some great new features like changing page orientation from landscape to portrait and vice versa. In order to accomplish this requirement, set the page's MediaBox by using following code snippet.

## Change Page Orientation

The following code sample shows how to change page orientation in C#.

```
Document doc = new Document("PdfWithText.pdf");
foreach (Page page in doc.Pages)
{
    Rectangle r = page.MediaBox;
    double newHeight = r.Width;
    double newWidth = r.Height;
    double newLLX = r.LLX;
    //  We must to move page upper in order to compensate changing page size 
    // (lower edge of the page is 0,0 and information is usually placed from the 
    //  top of the page. That's why we move lover edge upper on difference between 
    //  old and new height.
    double newLLY = r.LLY + (r.Height - newHeight);
    page.MediaBox = new Rectangle(newLLX, newLLY, newLLX + newWidth, newLLY + newHeight);
    // Sometimes we also need to set CropBox (if it was set in original file)
    page.CropBox = new Rectangle(newLLX, newLLY, newLLX + newWidth, newLLY + newHeight);
}
doc.Save("36115.pdf"); 
```

Please note that when using the above code snippet, some of the document's content might be cut because the page height is decreased. To avoid this, increase width proportionally and leave the height intact. Example of calculations:

```
Rectangle r = page.MediaBox;
// New height the same
double newHeight = r.Height;
// New width is expanded proportionally to make orientation landscape 
// (we assume that previous orientation is portrait)
double newWidth = r.Height * r.Height / r.Width;
```

Besides the above approach, consider using the PdfPageEditor facade (it can apply zoom to page contents)

```
// Load source PDF file
Document doc = new Document("PdfWithText.pdf");
// Get rectangular region of first page of PDF
Aspose.Pdf.Rectangle rect = doc.Pages[1].Rect;
// Instantiate PdfPageEditor instance
PdfPageEditor ppe = new PdfPageEditor();
// Bind source PDF
ppe.BindPdf("PdfWithText.pdf");
// Set zoom coefficient 
ppe.Zoom = (float)(rect.Width / rect.Height);
// Update page size
ppe.PageSize = new Aspose.Pdf.PageSize((float)rect.Height, (float)rect.Width);
// Save resultant PDF
ppe.Save("36115-1.pdf");
```

## PDF to HTML as a Single HTML with All Resources Embedded

One of the features in this release is conversion of a PDF to a single HTML file with all resources embedded. Prior to this release, when converting PDF files to HTML format, the resources (that is, images, fonts, CSS) used inside PDF are saved in separate folder in same directory that the HTML file was saved to. Recently we received a requirement to convert PDF file to HTML format where all the resources should be embedded in the HTML file. The implementation is according to the [data URI scheme][2]. In order to accomplish this requirement, a new value EmbedAllIntoHtml is introduced to the HtmlSaveOptions.PartsEmbeddingModes enumeration. Please try the following code snippet.

```
// Load source PDF file
Document doc = new Document(@"F:\ExternalTestsData\36608.pdf");
// Instantiate HTML Save options object
HtmlSaveOptions newOptions = new HtmlSaveOptions();

// Enable option to embed all resources inside the HTML
newOptions.PartsEmbeddingMode = HtmlSaveOptions.PartsEmbeddingModes.EmbedAllIntoHtml;

// This is just optimization for IE and can be omitted 
newOptions.LettersPositioningMethod = HtmlSaveOptions.LettersPositioningMethods.UseEmUnitsAndCompensationOfRoundingErrorsInCss;
newOptions.RasterImagesSavingMode = HtmlSaveOptions.RasterImagesSavingModes.AsEmbeddedPartsOfPngPageBackground;
newOptions.FontSavingMode = HtmlSaveOptions.FontSavingModes.SaveInAllFormats;
// Output file path 
string outHtmlFile = @"F:\ExternalTestsData\36340.html";
doc.Save(outHtmlFile, newOptions);
```

In case the requirement is to only embed CSS inside the output HTML, use the EmbedCssOnly value of the HtmlSaveOptions.PartsEmbeddingModes enumeration.

## Retrieve RadioHoriz Property for RadioButton Field

The RadioHoriz property is required to control how radio button items are added: if RadioHoriz is true items are added horizontally, if it is false they are added vertically. This property is specific to the FormEditor class and just defines the most used scenario of creating radio buttons. Usually it does not make any sense to read the RadioHoriz property for radio button field and you can access RadioButtonField sub-items and read their coordinates, instead of trying to read the RadioHoriz property. The following example illustrates the RadioHoriz property behavior, how to create radio button items with arbitrary positions and how to read positions of the radio button items.

### Example 1: Create new document and add radio button with 3 items (DOM approach)```
// Create a new document
Document doc = new Document();
Page page = doc.Pages.Add();
// Add radio button field
RadioButtonField field = new Aspose.Pdf.InteractiveFeatures.Forms.RadioButtonField(page);
field.Rect = new Aspose.Pdf.Rectangle(40, 650, 100, 720);
field.PartialName = "NewField";

// Add radio button options. please note that these options are situated 
// neither horizontally nor vertically. 
// You can try to set any coordinates (and even size) for them. 
RadioButtonOptionField opt1 = new RadioButtonOptionField();
opt1.Rect = new Aspose.Pdf.Rectangle(40, 650, 60, 670);
opt1.OptionName = "Item1";
opt1.Border = new Border(opt1);
opt1.Border.Width = 1;
opt1.Characteristics.Border = System.Drawing.Color.Black;

RadioButtonOptionField opt2 = new RadioButtonOptionField();
opt2.Rect = new Aspose.Pdf.Rectangle(60, 670, 80, 690);
opt2.OptionName = "Item2";
opt2.Border = new Border(opt2);
opt2.Border.Width = 1;
opt2.Characteristics.Border = System.Drawing.Color.Black;

RadioButtonOptionField opt3 = new RadioButtonOptionField();
opt3.Rect = new Aspose.Pdf.Rectangle(80, 690, 100, 710);
opt3.OptionName = "Item3";
opt3.Border = new Border(opt3);
opt3.Border.Width = 1;
opt3.Characteristics.Border = System.Drawing.Color.Black;
field.Add(opt1);
field.Add(opt2);
field.Add(opt3);
doc.Form.Add(field);
doc.Save("37337-1.pdf");
```

### Example 2: Adding horizontally and vertically situated radio buttons with FormEditor.```
// Load previously saved document
FormEditor formEditor = new FormEditor();
formEditor.BindPdf("37337-1.pdf");
// RadioGap is distance between two radio button options. 
formEditor.RadioGap = 4;
// Add horizontal radio button
formEditor.RadioHoriz = true;
// RadioButtonItemSize if size of radio button item.
formEditor.RadioButtonItemSize = 20;
formEditor.Facade.BorderWidth = 1;
formEditor.Facade.BorderColor = System.Drawing.Color.Black;
formEditor.Items = new string[] { "First", "Second", "Third" };
formEditor.AddField(FieldType.Radio, "NewField1", 1, 40, 600, 120, 620);

// Add other radio button situated vertically
formEditor.RadioHoriz = false;
formEditor.Items = new string[] { "First", "Second", "Third" };
formEditor.AddField(FieldType.Radio, "NewField2", 1, 40, 500, 60, 550);
formEditor.Save("37337-2.pdf");
```

### Example 3: How to get RadioButton items coordinates.```
// Load output document 
Document doc1 = new Document("37337-2.pdf");
// Find added fields
RadioButtonField field0 = doc1.Form["NewField"] as RadioButtonField;
RadioButtonField field1 = doc1.Form["NewField1"] as RadioButtonField;
RadioButtonField field2 = doc1.Form["NewField2"] as RadioButtonField;

// And show positions of sub items for each of them. 
foreach (RadioButtonOptionField option in field0)
{
    Console.WriteLine(option.Rect);
}
foreach (RadioButtonOptionField option in field1)
{
    Console.WriteLine(option.Rect);
}

foreach (RadioButtonOptionField option in field2)
{
    Console.WriteLine(option.Rect);
}
```

## Text Replacement should Automatically Re-arrange Page Contents

We recently received a requirement that once text in a PDF document is replaced, the contents should be re-arranged. If text is replaced with smaller contents, for example, no extra space should be displayed. If it's replace with a longer string, words should not overlap existing contents. To cater for these requirements, we enhanced the API and no such issue appears when replacing text inside PDF.

```
// Load source PDF file
Document doc = new Document("29860.pdf");
// Create TextFragment Absorber object with regular expression
TextFragmentAbsorber textFragmentAbsorber = new TextFragmentAbsorber("[Cname,companyname,Textbox,50]");
doc.Pages.Accept(textFragmentAbsorber);
// Replace each TextFragment
foreach (TextFragment textFragment in textFragmentAbsorber.TextFragments)
{
    // Set font of text fragment being replaced
    textFragment.TextState.Font = FontRepository.FindFont("Arial");
    // Set font size
    textFragment.TextState.FontSize = 12;
    textFragment.TextState.ForegroundColor = Aspose.Pdf.Color.Navy;
    // Replace the text with larger string than placeholder
    textFragment.Text = "This is a Larger String for the Testing of this issue";
}
// Save resultant PDF
doc.Save("29860_out_large_NoHyphenation.pdf");
```

You also can specify the ReplaceAdjustment.WholeWordsHyphenation option to wrap text on the next or current line if the current line becomes too long or short after replacement: textFragmentAbsorber.TextReplaceOptions.ReplaceAdjustmentAction = TextReplaceOptions.ReplaceAdjustment.WholeWordsHyphenation;

As well as the features explored above, there are numerous enhancements and fixes for issues reported in the earlier version. PDF to DOC conversion, text replacement, XPS to PDF conversion, PDF to image conversion, HTML to PDF conversion, PNG to PDF conversion, XSL-FO to PDF conversion, PDF to PDF/A, PDF to Excel, SVG to PDF, etc. are key improvement areas. Please go ahead, download and start exploring the new release of [Aspose.PDF for .NET 9.6.0.][3]




[1]: https://downloads.aspose.com/pdf/net
[2]: http://en.wikipedia.org/wiki/Data_URI_scheme
[3]: https://downloads.aspose.com/pdf/net




