---
title: 'Convert PDF to HTML with Customized Image Resolution in C#'
date: Mon, 02 Apr 2018 21:08:04 +0000
draft: false
url: /2018/04/02/improved-image-quality-in-pdf-to-html-conversion-and-repeating-column-in-table/
author: Asad Ali
summary: ''
tags: ['Asad Ali', 'Convert PDF to HTML Csharp']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net.png" alt="">}}


The regular monthly update [Aspose.PDF for .NET 18.3][1] has been published and available for download. Like every new release, [Aspose.PDF for .NET 18.3][2] includes fixes for issues reported in earlier release version(s) and in this release, we have also added some attractive and exciting features, in order to cater to the various scenarios. Since we always have been striving to provide a robust, stable and feature-rich release version, Aspose.PDF for .NET 18.3 includes new functionalities and enhancements. An overview of improvements and changes in this version of the API is given in the [release notes][3] section of API documentation.

## Convert PDF to HTML with Improved Image Quality

In order to produce a better quality of images, when generating HTML from PDF document, you can use [HtmlSaveOptions.ImageResolution][4] property to the resolution of output images. This way the output HTML will contain better image quality.

Following code snippet shows usage of ImageResolution property while converting PDF to HTML:

```
Document document = new Document(myDir + "input.pdf");
string workingDir = Directory.GetCurrentDirectory();
string outputFilePath = Path.Combine(myDir, "output.html");
HtmlSaveOptions options = new HtmlSaveOptions();
options.ImageResolution = 300; 
options.PartsEmbeddingMode = 
HtmlSaveOptions.PartsEmbeddingModes.EmbedAllIntoHtml;
options.RasterImagesSavingMode = 
HtmlSaveOptions.RasterImagesSavingModes.AsEmbeddedPartsOfPngPageBackground;
options.LettersPositioningMethod = 
HtmlSaveOptions.LettersPositioningMethods.UseEmUnitsAndCompensationOfRoundingErrorsInCss;
document.Save(outputFilePath, options);
```

## Add Repeating Column in Table in PDF

In earlier version(s) of the API, you have been using adding repeating rows feature by setting [RepeatingRowsCount][5] property of [Aspose.Pdf.Table][6] Class. We have implemented adding repeating column functionality in Aspose.PDF for .NET 18.3. [RepeatingColumnsCount][7] property has been added to **Aspose.Pdf.Table** Class, in order to repeat the columns in tables, which are too wide to fit on a single page. You can check the following code snippet for an example of using **RepeatingColumnsCount** property:

```
string outFile = GetOutputPath("40515.pdf");
// Added document
// Added document
Document doc = new Document();
Aspose.Pdf.Page page = doc.Pages.Add();

//Instantiate an outer table that takes up the entire page
Aspose.Pdf.Table outerTable = new Aspose.Pdf.Table();
outerTable.ColumnWidths = "100%";
outerTable.HorizontalAlignment = HorizontalAlignment.Left;

//Instantiate a table object that will be nested inside 
//outerTable that will break
//inside the same page
Aspose.Pdf.Table mytable = new Aspose.Pdf.Table();
mytable.Broken = TableBroken.VerticalInSamePage;
mytable.ColumnAdjustment = ColumnAdjustment.AutoFitToContent;

//Add the outerTable to the page paragraphs
//Add mytable to outerTable
page.Paragraphs.Add(outerTable);
var bodyRow = outerTable.Rows.Add();
var bodyCell = bodyRow.Cells.Add();
bodyCell.Paragraphs.Add(mytable);
mytable.RepeatingColumnsCount = 5;
//comment out this or the top section to test if the table renders
//page.Paragraphs.Add(mytable);

//Add header Row
Aspose.Pdf.Row row = mytable.Rows.Add();
row.Cells.Add("header 1");
row.Cells.Add("header 2");
row.Cells.Add("header 3");
row.Cells.Add("header 4");
row.Cells.Add("header 5");
row.Cells.Add("header 6");
row.Cells.Add("header 7");
row.Cells.Add("header 11");
row.Cells.Add("header 12");
row.Cells.Add("header 13");
row.Cells.Add("header 14");
row.Cells.Add("header 15");
row.Cells.Add("header 16");
row.Cells.Add("header 17");

for (int RowCounter = 0; RowCounter <= 5; RowCounter++)
{
 //Create rows in the table and then cells in the rows
 Aspose.Pdf.Row row1 = mytable.Rows.Add();
 row1.Cells.Add("col " + RowCounter.ToString() + ", 1");
 row1.Cells.Add("col " + RowCounter.ToString() + ", 2");
 row1.Cells.Add("col " + RowCounter.ToString() + ", 3");
 row1.Cells.Add("col " + RowCounter.ToString() + ", 4");
 row1.Cells.Add("col " + RowCounter.ToString() + ", 5");
 row1.Cells.Add("col " + RowCounter.ToString() + ", 6");
 row1.Cells.Add("col " + RowCounter.ToString() + ", 7");
 row1.Cells.Add("col " + RowCounter.ToString() + ", 11");
 row1.Cells.Add("col " + RowCounter.ToString() + ", 12");
 row1.Cells.Add("col " + RowCounter.ToString() + ", 13");
 row1.Cells.Add("col " + RowCounter.ToString() + ", 14");
 row1.Cells.Add("col " + RowCounter.ToString() + ", 15");
 row1.Cells.Add("col " + RowCounter.ToString() + ", 16");
 row1.Cells.Add("col " + RowCounter.ToString() + ", 17");
}
doc.Save(outFile);
```

## Miscellaneous

As it is always recommended to use the latest release of our API’s, so we suggest you please download the latest release [Aspose.PDF for .NET 18.3][8] and check following resources which will help you working with API:

*   [Home page for Aspose.PDF for .NET][9]
*   [Download Aspose.PDF for .NET 18.3][10]
*   [Aspose.PDF product family forum][11] – Post your technical questions and queries, or any other problem you faced while running Aspose.PDF APIs.
*   [Aspose.PDF for .NET online documentation][12] – help documentation and API reference documents.
*   [Enable Blog Subscription][13] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.PDF APIs, new features, fixes and other API related topics by subscribing to Aspose.PDF blog.
*   [Aspose.PDF for .NET Examples][14] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Pdf/18.3.0
[2]: https://www.nuget.org/packages/Aspose.Pdf/18.3.0
[3]: https://docs.aspose.com/display/pdfnet/Aspose.PDF+for+.NET+18.3+Release+Notes
[4]: https://apireference.aspose.com/net/pdf/aspose.pdf/htmlsaveoptions/properties/imageresolution
[5]: https://apireference.aspose.com/net/pdf/aspose.pdf/table/properties/repeatingrowscount
[6]: https://apireference.aspose.com/net/pdf/aspose.pdf/table/
[7]: https://apireference.aspose.com/net/pdf/aspose.pdf/table/properties/repeatingcolumnscount
[8]: https://www.nuget.org/packages/Aspose.Pdf/18.3.0
[9]: https://products.aspose.com/pdf/net
[10]: https://www.nuget.org/packages/Aspose.Pdf/18.3.0
[11]: https://forums.aspose.com/c/pdf
[12]: https://docs.aspose.com/display/pdfnet/Home
[13]: https://blog.aspose.com/category/aspose-products/aspose-pdf-product-family/
[14]: https://github.com/aspose-pdf/Aspose.PDF-for-.NET




