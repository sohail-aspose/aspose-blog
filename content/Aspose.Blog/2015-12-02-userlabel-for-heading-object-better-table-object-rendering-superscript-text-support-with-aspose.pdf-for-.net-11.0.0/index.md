---
title: 'UserLabel for Heading object, better Table object rendering, SuperScript text support with Aspose.Pdf for .NET 11.0.0'
date: Wed, 02 Dec 2015 18:44:41 +0000
draft: false
url: /2015/12/02/userlabel-for-heading-object-better-table-object-rendering-superscript-text-support-with-aspose.pdf-for-.net-11.0.0/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz']
categories: ['Aspose.PDF Product Family']
---

[![Aspose.Pdf for .NET logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/06/aspose-Pdf-for-net_100.png)A new release of [Aspose.Pdf for .NET 11.0.0][2] has been published and is available in download section. This version has some unique improvements which have been recently requested by our customers. Among those new features and enhancements, we also have made significant progress in terms bug fixing and a huge number of issues reported against earlier release versions have been fixed in this new release. The following sections describe some details regarding these newly added features/enhancements.

## Support UserLabel property for Heading instance

The legacy Aspose.Pdf.Generator approach provided the capabilities to Use System Defined Bullets while creating PDF documents from scratch, where user can define its own custom labels for heading instances. Recently we received a similar requirement to support similar capabilities in new DOM of Aspose.Pdf namespace. The bullet style can be any value as specified in image below.

```
Document doc = new Document();
doc.Pages.Add();
Aspose.Pdf.Heading heading = new Aspose.Pdf.Heading(1);
heading.Style = NumberingStyle.NumeralsArabic;
heading.Text = "Heading ";
heading.UserLabel= "Bullet1";
doc.Pages[1].Paragraphs.Add(heading);
doc.Save("c:/pdftest/Headingtest.pdf");
```

## Move whole table to the next page when page breaks

In previous release versions, when a table reaches bottom margin of page and all the rows of table cannot be rendered over same page, the table started to break. However recently we received a requirement that if table reaches page bottom margin, instead breaking the table rows, the complete table should be rendered in subsequent page. So when executing following code snippet with this new release, the complete second table will be rendered on second page, instead of displaying its few rows on first page and some rows on second page.

```
 Document doc = new Document();
Page page = doc.Pages.Add();

//create text fragment
TextFragment textFragment = new TextFragment("main text");
//textFragment.setPosition(new com.aspose.pdf.Position(100, 600));

//set text properties
textFragment.TextState.Font = (FontRepository.FindFont("Verdana"));
textFragment.TextState.FontSize = (14);
textFragment.TextState.ForegroundColor = (Color.Black);
textFragment.TextState.BackgroundColor = (Color.Blue);

page.PageInfo.Height = (PageSize.A4.Height);
page.PageInfo.Width = (PageSize.A3.Width);
page.PageInfo.Margin.Top = (72);
page.PageInfo.Margin.Bottom = (72);
page.PageInfo.Margin.Left = (72);
page.PageInfo.Margin.Right = (72);

TextFragment t4 = new TextFragment("");
page.Paragraphs.Add(t4);
page.Paragraphs.Add(t4);
TextFragment t5 = new TextFragment("CO Acknowledgement:");
t5.TextState.Font = (FontRepository.FindFont("Arial"));
t5.TextState.FontSize = (10);
t5.TextState.FontStyle = (FontStyles.Bold);
t5.TextState.HorizontalAlignment = (HorizontalAlignment.Left);
t5.TextState.ForegroundColor = (Color.Black);
t5.TextState.Underline = (true);

page.Paragraphs.Add(t5);


page.Paragraphs.Add(t4);

//System.out.println(page.getParagraphs().get_Item(63).isKeptWithNext());

Image selectImg = new Image();
selectImg.HorizontalAlignment = (HorizontalAlignment.Right);
selectImg.File = (myDir + "Radio_Checked.png");

Image unselectImg = new Image();
unselectImg.HorizontalAlignment = (HorizontalAlignment.Right);
unselectImg.File = (myDir + "Radio_Checked.png");

Table table = new Table();
// Add the table in paragraphs collection of the desired section
page.Paragraphs.Add(table);
// Set with column widths of the table
table.ColumnWidths = ("18% 66,5% 15,5%");
// Set default cell border using BorderInfo object
table.DefaultCellBorder = (new BorderInfo(BorderSide.All, 0.1F, Color.Black));
// Set table border using another customized BorderInfo object
table.Border = (new BorderInfo(BorderSide.All, 0.1F, Color.Black));
table.Border = (new BorderInfo(BorderSide.Bottom, 0.1F, Color.White));
// Create MarginInfo object and set its left, bottom, right and top margins
MarginInfo margin = new MarginInfo();
margin.Left = (0.5f);
margin.Right = (0.5f);
margin.Top = (0.5f);
margin.Bottom = (0.5f);
// Set the default cell padding to the MarginInfo object

TextState celltext = new TextState("Arial", 8);
table.DefaultCellPadding = (margin);

table.DefaultCellTextState = (celltext);
//table.setInNewPage(true);
//table.setBroken(false);

//table.setBroken(TableBroken.VerticalInSamePage);

Console.Out.WriteLine(table.Broken);


TextState celltext1 = new TextState("Arial", 8);
celltext1.ForegroundColor = (Color.White);

Table table2 = new Table();
table2.ColumnWidths = ("16% 17% 16% 17% 16% 17%");
table2.DefaultCellTextState = (celltext);
//table2.setBroken(false);
//table2.setBroken(TableBroken.);
Row row7 = table2.Rows.Add();
//row7.getCells().add();


Cell icon = row7.Cells.Add();
icon.Paragraphs.Add(selectImg);
row7.Cells.Add("Yes");
Cell icon2 = row7.Cells.Add();
icon2.Paragraphs.Add(unselectImg);
row7.Cells.Add("No");

// Create rows in the table and then cells in the rows
Row row1 = table.Rows.Add();
row1.IsRowBroken = (false);
row1.Cells.Add("Client Owner EWR Acknowledgement").RowSpan = (3);
row1.Cells[0].Alignment = (HorizontalAlignment.Center);
row1.Cells[0].BackgroundColor = (Color.Blue);
row1.Cells[0].DefaultCellTextState = (celltext1);
row1.Cells.Add("row1 string asdasdasdsadas");
Cell icon1 = row1.Cells.Add();

icon1.Paragraphs.Add(table2);


//second row
Row row2 = table.Rows.Add();
row2.IsRowBroken = (false);
row2.Cells.Add("Choose a  type ");
if (true)
{
    row2.Cells.Add("2nd Rowasdasd ").Alignment = (HorizontalAlignment.Center);
}
else
{
    row2.Cells.Add("");
}

//third row
Row row3 = table.Rows.Add();

row3.Cells.Add("Summary Comments: dasasdasdas");
row3.Cells[0].ColSpan = (2);
row3.IsRowBroken = (false);

//forth row
Row row4 = table.Rows.Add();
row4.Cells.Add("").Border = (new BorderInfo(BorderSide.All, 0.7F, Color.FromArgb(255, 255, 255)));
row4.Cells.Add("").Border = (new BorderInfo(BorderSide.All, 0.7F, Color.FromArgb(255, 255, 255)));
row4.Cells.Add("").Border = (new BorderInfo(BorderSide.All, 0.7F, Color.FromArgb(255, 255, 255)));
row4.IsRowBroken = (false);


page.Paragraphs.Add(new TextFragment("")); page.Paragraphs.Add(new TextFragment(""));
page.Paragraphs.Add(new TextFragment("")); page.Paragraphs.Add(new TextFragment(""));
page.Paragraphs.Add(new TextFragment("")); page.Paragraphs.Add(new TextFragment(""));
page.Paragraphs.Add(new TextFragment("")); page.Paragraphs.Add(new TextFragment(""));
page.Paragraphs.Add(new TextFragment("")); page.Paragraphs.Add(new TextFragment(""));
page.Paragraphs.Add(new TextFragment("")); page.Paragraphs.Add(new TextFragment(""));
page.Paragraphs.Add(new TextFragment("")); page.Paragraphs.Add(new TextFragment(""));
page.Paragraphs.Add(new TextFragment("")); page.Paragraphs.Add(new TextFragment(""));
page.Paragraphs.Add(new TextFragment("")); page.Paragraphs.Add(new TextFragment(""));
page.Paragraphs.Add(new TextFragment("")); page.Paragraphs.Add(new TextFragment(""));
page.Paragraphs.Add(new TextFragment("")); page.Paragraphs.Add(new TextFragment(""));
page.Paragraphs.Add(new TextFragment("")); page.Paragraphs.Add(new TextFragment(""));
page.Paragraphs.Add(new TextFragment("")); page.Paragraphs.Add(new TextFragment(""));
page.Paragraphs.Add(new TextFragment("")); page.Paragraphs.Add(new TextFragment(""));

page.Paragraphs.Add(new TextFragment("")); page.Paragraphs.Add(new TextFragment(""));
page.Paragraphs.Add(new TextFragment("")); page.Paragraphs.Add(new TextFragment(""));
page.Paragraphs.Add(new TextFragment("")); page.Paragraphs.Add(new TextFragment(""));
page.Paragraphs.Add(new TextFragment("")); page.Paragraphs.Add(new TextFragment(""));
page.Paragraphs.Add(new TextFragment("")); page.Paragraphs.Add(new TextFragment(""));
page.Paragraphs.Add(new TextFragment("")); page.Paragraphs.Add(new TextFragment(""));
page.Paragraphs.Add(new TextFragment("")); page.Paragraphs.Add(new TextFragment(""));
page.Paragraphs.Add(new TextFragment(""));
page.Paragraphs.Add(new TextFragment("")); page.Paragraphs.Add(new TextFragment(""));
page.Paragraphs.Add(new TextFragment(""));
page.Paragraphs.Add(new TextFragment("")); page.Paragraphs.Add(new TextFragment(""));
page.Paragraphs.Add(new TextFragment("")); page.Paragraphs.Add(new TextFragment(""));
page.Paragraphs.Add(new TextFragment("")); page.Paragraphs.Add(new TextFragment(""));
page.Paragraphs.Add(new TextFragment("")); page.Paragraphs.Add(new TextFragment(""));
page.Paragraphs.Add(new TextFragment("")); page.Paragraphs.Add(new TextFragment(""));
page.Paragraphs.Add(new TextFragment(""));
page.Paragraphs.Add(new TextFragment(""));
page.Paragraphs.Add(table);


// save updated PDF file
doc.Save(myDir + "Row_Span_Issue_Text_Added_1090_net_test.pdf");
```

## Support of superscript in TextState

In order to accomplish this requirement, you may consider using TextState.Superscript and TextState.Subscript properties of TextSegment and TextFragment objects. Please take a look over following code snippet.

```
Document document = new Document();
Page page = document.Pages.Add();

//Superscript example
TextFragment fragment1 = new TextFragment();
TextSegment seg11 = new TextSegment("8");
fragment1.Segments.Add(seg11);
TextSegment seg12 = new TextSegment("th");
fragment1.Segments.Add(seg12);
seg12.TextState.Superscript = true;
TextSegment seg13 = new TextSegment(" M");
fragment1.Segments.Add(seg13);
TextSegment seg14 = new TextSegment("lle");
fragment1.Segments.Add(seg14);
seg14.TextState.Superscript = true;
TextSegment seg15 = new TextSegment(" Blip");
fragment1.Segments.Add(seg15);
TextSegment seg16 = new TextSegment("42");
seg16.TextState.Superscript = true;
fragment1.Segments.Add(seg16);
TextSegment seg17 = new TextSegment(" x");
fragment1.Segments.Add(seg17);
TextSegment seg18 = new TextSegment("2n");
seg18.TextState.Superscript = true;
fragment1.Segments.Add(seg18);
page.Paragraphs.Add(fragment1);

//Subscript example
TextFragment fragment2 = new TextFragment();
TextSegment seg21 = new TextSegment("C");
fragment2.Segments.Add(seg21);
TextSegment seg22 = new TextSegment("2");
fragment2.Segments.Add(seg22);
seg22.TextState.Subscript = true;
TextSegment seg23 = new TextSegment("H");
fragment2.Segments.Add(seg23);
TextSegment seg24 = new TextSegment("5");
fragment2.Segments.Add(seg24);
seg24.TextState.Subscript = true;
TextSegment seg25 = new TextSegment("OH + 3O");
fragment2.Segments.Add(seg25);
TextSegment seg26 = new TextSegment("2");
seg26.TextState.Subscript = true;
fragment2.Segments.Add(seg26);
TextSegment seg27 = new TextSegment(" —> 2CO");
fragment2.Segments.Add(seg27);
TextSegment seg28 = new TextSegment("2");
seg28.TextState.Subscript = true;
fragment2.Segments.Add(seg28);
TextSegment seg29 = new TextSegment(" + 3H");
fragment2.Segments.Add(seg29);
TextSegment seg210 = new TextSegment("2");
seg210.TextState.Subscript = true;
fragment2.Segments.Add(seg210);
TextSegment seg211 = new TextSegment("O;");
fragment2.Segments.Add(seg211);
page.Paragraphs.Add(fragment2);

document.Save(outFile);
```You can set TextState.FontSize and TextState.LineSpacing for TextSegment or TextFragment objects as normal when setting Superscript property. However if you need to set specific font (e.g. Arial) and superscript, please try using following code snippet

```
TextFragment fragment1 = new TextFragment();
TextSegment seg11 = new TextSegment("8");
seg11.TextState.Font = FontRepository.FindFont("Arial");
fragment1.Segments.Add(seg11);
TextSegment seg12 = new TextSegment("th");
seg12.TextState.Font = FontRepository.FindFont("Arial");
seg12.TextState.Superscript = true;
fragment1.Segments.Add(seg12);
```

In above specified code snippet, the font information is set for TextSegement object because setting the font for TextFragment leads to unification of text segments properties, and individual properties of segments will be lost. So following code snippet cannot be used.

```
TextFragment fragment1 = new TextFragment();
fragment1.TextState.Font = FontRepository.FindFont("Arial");
```

Also please note that we use following values for glyph transformation: **superscript/subscript size 58.3%, subscript position -33.3%, superscript position +33.3%**. These values match to [default values of Adobe products.][3] However if you have a requirement to modify these glyph transformation parameters, please feel free to contact and we may consider implementing as separate enhancement.

## Miscellaneous fixes

As well as the enhancements and features discussed above, there have been specific improvement for PDF to HTML and HTML to PDF conversion features with better support for HTML5. Among these fixes, the PCL to PDF, SVG to PDF, PDF to Excel, PDF to DOC, PDF to TIFF and TIFF to PDF conversion, PDF to XPS, ePUB to PDF, XML to PDF, conversion of PDF to PDF/A compliant documents, text replacement, Filling of signature field with an image, flattening of PDF, FloatingBox rendering, Footnote, EndNote and rendering of non-English (specifically Arabic) contents are also improved. Please download and try the latest release of [Aspose.Pdf for .NET 11.0.0][4].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/06/aspose-Pdf-for-net_100.png "Aspose.Pdf for .NET logo"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.pdf-for-.net/entry669037.aspx
[3]: https://en.wikipedia.org/wiki/Subscript_and_superscript#Desktop_publishing
[4]: http://www.aspose.com/community/files/51/.net-components/aspose.pdf-for-.net/entry669037.aspx




