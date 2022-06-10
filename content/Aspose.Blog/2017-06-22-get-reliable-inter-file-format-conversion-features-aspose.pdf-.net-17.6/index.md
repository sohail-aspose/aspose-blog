---
title: 'Get Reliable Inter File Format Conversion using Aspose.PDF for .NET'
date: Thu, 22 Jun 2017 12:44:30 +0000
draft: false
url: /2017/06/22/get-reliable-inter-file-format-conversion-features-aspose.pdf-.net-17.6/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose_pdf-for-net.jpg" alt="">}}


Get better inter-document conversion features with the new [Aspose.PDF for .NET][1] 17.6 release. This release mainly focuses on fixing the issues reported in earlier release versions and like always recommended, we encourage our customers to try using latest release versions as they contain recent enhancements and improvements in terms of problems resolution.

## Rotate Text inside Table Cell

Table is one of the widely used element inside PDF document to represent data and sometimes we have a requirement to rotate the text inside the table cell. The following code snippet shows the steps to rotate text with 90 degrees and render it in table cell.

```
 // create Document instance
Document doc = new Document();
// add page to pages collection of Document instance
Page pg = doc.Pages.Add();
// create table instance
Table tab = new Table();
tab.DefaultCellTextState.FontSize = 7;
tab.DefaultCellPadding = new MarginInfo(7, 7, 7, 7);
tab.DefaultCellBorder = new BorderInfo(BorderSide.All, 0.1f);

Aspose.Pdf.Text.TextFragment verticalTextFragment = new Aspose.Pdf.Text.TextFragment("Gradient");
verticalTextFragment.TextState.Rotation = 90;
tab.ColumnWidths = (verticalTextFragment.Rectangle.Width + 5).ToString(System.Globalization.CultureInfo.InvariantCulture) + " " + (verticalTextFragment.Rectangle.Width + 5).ToString(System.Globalization.CultureInfo.InvariantCulture);
Row r1 = tab.Rows.Add();
Cell c1 = r1.Cells.Add();
c1.RowSpan = 3;
r1.Cells.Add("A");

Row r2 = tab.Rows.Add();
r2.Cells.Add("B");

Row r3 = tab.Rows.Add();
r3.Cells.Add("C");
// add Vertical Text to paragraphs collection of Cell instance
c1.Paragraphs.Add(verticalTextFragment);
// add table to paragraphs collection of Page instance
pg.Paragraphs.Add(tab);

Table tab1 = new Table();
tab1.Margin.Top = 50;
tab1.DefaultCellTextState.FontSize = 7;
tab1.DefaultCellPadding = new MarginInfo(7, 7, 7, 7);
tab1.DefaultCellBorder = new BorderInfo(BorderSide.All, 0.1f);

Aspose.Pdf.Text.TextFragment verticalTextFragment1 = new Aspose.Pdf.Text.TextFragment("Gradient");
// set rotation angle for Text as 90 degrees
verticalTextFragment.TextState.Rotation = 90;
//After rotation height of the text will be width of particular column. 
tab1.ColumnWidths = (verticalTextFragment.Rectangle.Height + 5).ToString(System.Globalization.CultureInfo.InvariantCulture) + " " + (verticalTextFragment.Rectangle.Width + 5).ToString(System.Globalization.CultureInfo.InvariantCulture);
Row r11 = tab1.Rows.Add();
Cell c11 = r11.Cells.Add();
c11.RowSpan = 3;
r11.Cells.Add("A");

Row r22 = tab1.Rows.Add();
r22.Cells.Add("B");

Row r33 = tab1.Rows.Add();
r33.Cells.Add("C");
// add vertical text with 90 degress to paragraphs collection of Cell instance
c11.Paragraphs.Add(verticalTextFragment);
// add second table to paragraphs collection of Page instance
pg.Paragraphs.Add(tab1);
// save the resultant PDF document
doc.Save(@"c:/pdftest/RotateText.pdf"); 
```



{{< figure align=center src="images/Rotated_Text_inside_TableCell.png" alt="">}}


## Miscellaneous fixes

Apart from the above-mentioned improvements, the PDF to PDF/A, PDF to DOC/DOCX, PDF to PPT/PPTX conversion features are specifically improved in this release. These features have been greatly tested under various scenarios while using different input files. The PDF/A validation feature is also tuned to produce more reliable results. Furthermore, the EPUB to PDF, Text manipulation, PDF to Image conversion, Text extraction are among the improvement areas. It is always recommended to use latest release of our API's, so we suggest you to please download the latest release of [Aspose.Pdf for .NET 17.6][2] and check [Release Notes][3] section for list of issues fixed in Aspose.Pdf for .NET 17.6

*   [Home page for Aspose.PDF for .NET][4]
*   [Download Aspose.PDF for .NET][5]
*   [Aspose.PDF product family forum][6]– Post your technical questions and queries, or any other problem you faced while running Aspose.Pdf APIs.
*   [Aspose.PDF for .NET online documentation][7] – help documentation and API reference documents.
*   [Enable Blog Subscription][8]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.PDF APIs, new features, fixes, and other API related topics by subscribing to Aspose.PDF blog.
*   [Aspose.PDF for .NET Examples][9]– We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://products.aspose.com/pdf/net
[2]: https://downloads.aspose.com/pdf/net/new-releases/aspose.pdf-for-.net-17.6/
[3]: https://docs.aspose.com/pdf/net/aspose-pdf-for-net-17-6-release-notes/
[4]: https://products.aspose.com/pdf/net/
[5]: https://downloads.aspose.com/pdf/net
[6]: https://forums.aspose.com/c/pdf
[7]: https://docs.aspose.com/pdf/net/
[8]: https://blog.aspose.com/category/aspose-products/aspose-pdf-product-family/
[9]: https://github.com/aspose-pdf/Aspose.Pdf-for-.NET




