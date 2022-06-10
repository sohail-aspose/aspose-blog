---
title: 'Reference an Image Multiple Times and Add Text Inside a Graph in PDF using C#'
date: Tue, 17 Jan 2017 03:13:32 +0000
draft: false
url: /2017/01/17/reference-an-image-multiple-times-and-add-text-inside-a-graph-in-pdf-using-csharp/
author: Tilal Ahmad
summary: ''
tags: ['Add Text Inside a Graph in PDF', 'Reference an Image Multiple Times in PDF']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose_pdf-for-net.jpg" alt="">}}


We are pleased to announce the release of [Aspose.PDF for .NET 17.1.0][1]. This month's release introduces some new features. Some of these are to add reference of an image multiple times, break text for a table broken across the pages, and to set different TabLeaderType for different TOC levels along with an enhancement to add text inside the Graph Object. This release also contains the fixes of bugs reported in previous versions by our valued customers that improve the API functionality. Please check the detailed release notes of [Aspose.PDF for .NET 17.1.0][2], in order to get an idea about the new features/enhancements and fixes made in this release of Aspose.Pdf for .NET API.

Furthermore, If you are planning to upgrade the API from any previous version, we strongly recommend you to check the [Public API Changes section][3] of current release and other intermediate releases from release notes pages, to know what has been changed since your current revision of the API.

The following sections describe some details regarding these newly added features/enhancements.

## Reference an Image Multiple Times in PDF using C#

Some of our customers have a requirement to use the same image reference for multiple times in a PDF, it helps to reduce the PDF document file size. We have introduced XImageCollection.Add(Ximage) method in this release. It helps to refer existing image instance in the PDF document instead new Image.

```
Aspose.Pdf.Rectangle imageRectangle = new Aspose.Pdf.Rectangle(0, 0, 30, 15);
using (Aspose.Pdf.Document document = new Aspose.Pdf.Document("input.pdf"))
{
    using (var imageStream = File.Open("icon.png", FileMode.Open))
    {
        XImage image = null;
        foreach (Page page in document.Pages)
        {
            WatermarkAnnotation annotation = new WatermarkAnnotation(page, page.Rect);
            XForm form = annotation.Appearance["N"];
            form.BBox = page.Rect;

            string name;
            if (image == null)
            {
                name = form.Resources.Images.Add(imageStream);
                image = form.Resources.Images[name];
            }
            else
            {
                name = form.Resources.Images.Add(image);
            }

            form.Contents.Add(new Operator.GSave());
            form.Contents.Add(new Operator.ConcatenateMatrix(new Aspose.Pdf.Matrix(imageRectangle.Width, 0, 0, imageRectangle.Height, 0, 0)));
            form.Contents.Add(new Operator.Do(name));
            form.Contents.Add(new Operator.GRestore());

            page.Annotations.Add(annotation, false);
            imageRectangle = new Aspose.Pdf.Rectangle(0, 0, imageRectangle.Width * 1.01, imageRectangle.Height * 1.01);
        }
    }

    document.Save("output.pdf");
}
```

Read more about this feature [here][4].

## Set Different TabLeaderTypes for Different TOC Levels

Previously, we have to use a single TabLeaderType for all the TOC entries. With the release of current version, now we can set different TabLeaderType for different TOC Levels. For this functionality, we can set LineDash property of TOC Level with required value of TabLeaderType enum. Please check the following sample code for details:

```
string outFile = "TOC.pdf";
Aspose.Pdf.Document doc = new Aspose.Pdf.Document();
Page tocPage = doc.Pages.Add();
TocInfo tocInfo = new TocInfo();
//set LeaderType
tocInfo.LineDash = TabLeaderType.Solid;
TextFragment title = new TextFragment("Table Of Contents");
title.TextState.FontSize = 30;
tocInfo.Title = title;
//Add the list section to the sections collection of the Pdf document
tocPage.TocInfo = tocInfo;
//Define the format of the four levels list by setting the left margins
//and
//text format settings of each level
tocInfo.FormatArrayLength = 4;
tocInfo.FormatArray[0].Margin.Left = 0;
tocInfo.FormatArray[0].Margin.Right = 30;
tocInfo.FormatArray[0].LineDash = TabLeaderType.Dot;
tocInfo.FormatArray[0].TextState.FontStyle = FontStyles.Bold | FontStyles.Italic;
tocInfo.FormatArray[1].Margin.Left = 10;
tocInfo.FormatArray[1].Margin.Right = 30;
tocInfo.FormatArray[1].LineDash = TabLeaderType.None;
tocInfo.FormatArray[1].TextState.FontSize = 10;
tocInfo.FormatArray[2].Margin.Left = 20;
tocInfo.FormatArray[2].Margin.Right = 30;
tocInfo.FormatArray[2].TextState.FontStyle = FontStyles.Bold;
tocInfo.FormatArray[3].LineDash = TabLeaderType.Solid;
tocInfo.FormatArray[3].Margin.Left = 30;
tocInfo.FormatArray[3].Margin.Right = 30;
tocInfo.FormatArray[3].TextState.FontStyle = FontStyles.Bold;
//Create a section in the Pdf document
Page page = doc.Pages.Add();
//Add four headings in the section
for (int Level = 1; Level <= 4; Level++)

{ Aspose.Pdf.Heading heading2 = new Aspose.Pdf.Heading(Level);
    TextSegment segment2 = new TextSegment();
    heading2.Segments.Add(segment2);
    heading2.IsAutoSequence = true;
    heading2.TocPage = tocPage;
    segment2.Text = "Sample Heading" + Level;
    heading2.TextState.Font = FontRepository.FindFont("Arial Unicode MS");
    //Add the heading into Table Of Contents. 
    heading2.IsInList = true; 
    page.Paragraphs.Add(heading2); 
}
// save the Pdf 
doc.Save(outFile);
```

Read more about this feature [here][5].

## Add Break Text for Table Broken in Two Pages

In legacy generator(Aspose.Pdf.Generator), we supported table break text to set some text string at the end of the page for the Table broken in two pages. In this release, we have implemented the same feature in a new generator(Aspsoe.Pdf).

```
string outFile = "Table.pdf";
Aspose.Pdf.Document doc = new Aspose.Pdf.Document();
Page page = doc.Pages.Add();
Aspose.Pdf.Table tab = new Aspose.Pdf.Table();
tab.Alignment = HorizontalAlignment.Center;
tab.DefaultCellBorder = new Aspose.Pdf.BorderInfo(Aspose.Pdf.BorderSide.All, 0.1f);
tab.Margin.Top = 10;

for (int i = 1; i <= 200; i++)

{ Aspose.Pdf.Row row1 = tab.Rows.Add(); row1.Cells.Add("row - " + i); }
tab.BreakText = new TextFragment("To be continued on next page");
tab.RepeatingRowsCount = 1;
page.Paragraphs.Add(tab);
doc.Save(outFile);
```

## Add Text Inside Graph Object

A customer requested an enhancement to add text inside a Graph object, for his business need. We have added a text property in Graph object to add text inside the shape. The following code shows how we can add text inside a Rectangle shape.

```
// Open document
string outFile = "Graph.pdf";
Aspose.Pdf.Document pdfDoc = new Aspose.Pdf.Document();
Aspose.Pdf.Page pdfPage = pdfDoc.Pages.Add();
Aspose.Pdf.Drawing.Graph graph = new Aspose.Pdf.Drawing.Graph(500, 100);
pdfPage.Paragraphs.Add(graph);

//1st rectangle
Aspose.Pdf.Drawing.Rectangle rect = new Aspose.Pdf.Drawing.Rectangle(0, 30, 50, 40);
rect.GraphInfo.LineWidth = 1f;
rect.GraphInfo.Color = Aspose.Pdf.Color.Black;
rect.Text = new TextFragment("Rectangle");
graph.Shapes.Add(rect);
pdfDoc.Save(outFile);
```

Read more about this feature [here][6].

## Aspose.PDF for .NET Resources

The following resources will help you work with Aspose.PDF for .NET:

*   [Home page for Aspose.PDF for .NET][7]
*   [Download Aspose.PDF for .NET][8]
*   [PDF product family forum][9]– Post your technical questions and queries, or any other problem you faced while running Aspose.PDF APIs.
*   [PDF for .NET online documentation][10]– help documentation.
*   [PDF for .NET online API reference][11] - API reference documents.
*   [Enable Blog Subscription][12]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.PDF, APIs, new features, fixes and other API related topics by subscribing to Aspose.PDF blog.
*   [PDF for .NET Examples][13]– We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/pdf/net/new-releases/aspose.pdf-for-.net-17.1.0/
[2]: https://docs.aspose.com/display/pdfnet/Aspose.Pdf+for+.NET+17.1.0+Release+Notes
[3]: https://docs.aspose.com/display/pdfnet/Aspose.Pdf+for+.NET+17.1.0+Release+Notes
[4]: https://docs.aspose.com/display/pdfnet/Manipulate+Images#ManipulateImages-AddReferenceofasingleImagemultipletimesinaPDFDocument
[5]: https://docs.aspose.com/display/pdfnet/Manipulate+PDF+Document#ManipulatePDFDocument-SetdifferentTabLeaderTypefordifferentTOCLevels
[6]: https://docs.aspose.com/display/pdfnet/Working+with+Graphs#WorkingwithGraphs-AddtextinsideGraphObject
[7]: http://www.aspose.com/products/pdf/net
[8]: http://www.aspose.com/downloads/pdf/net
[9]: http://forum.aspose.com
[10]: http://docs.aspose.com/display/pdfnet/Home
[11]: https://apireference.aspose.com/pdf/net
[12]: https://blog.aspose.com/
[13]: https://github.com/aspose-pdf/Aspose.Pdf-for-.NET




