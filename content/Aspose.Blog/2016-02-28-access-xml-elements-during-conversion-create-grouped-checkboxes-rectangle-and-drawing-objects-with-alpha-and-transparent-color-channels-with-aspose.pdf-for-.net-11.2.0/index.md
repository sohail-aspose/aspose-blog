---
title: 'Access XML Elements during PDF Conversion using Aspose.PDF for .NET 11.2.0'
date: Sun, 28 Feb 2016 19:19:14 +0000
draft: false
url: /2016/02/28/access-xml-elements-during-conversion-create-grouped-checkboxes-rectangle-and-drawing-objects-with-alpha-and-transparent-color-channels-with-aspose.pdf-for-.net-11.2.0/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net_100.png" alt="Aspose.Pdf for .NET logo">}}


As a regular monthly release process, [Aspose.PDF for .NET 11.2.0][1] has been published and this new release also contains new features of binding XML file for conversion to PDF format, accessing individual XML elements during PDF transformation, creation of grouped check-boxes, creation of Rectangle with Alpha color channel, change of TOC page numbering and placing a drawing object inside PDF with transparent color. Among these new features, there have been numerous improvements in terms of performance and resolution to issues reported in earlier release versions.

## Access TextFragement and TextSegment elements from XML file

The BindXML(..) method offers the feature to load XML file contents and Document.save() method can be used to save the output in PDF format. However during conversion, we can also access individual elements inside XML and use XML as template. The following code snippet shows the steps to access TextSegments from XML file.

```
// instantiate Document object
Document doc = new Document();
// bind source XML file
doc.BindXml("source.xml");
// get reference of page object from XML
Page page = (Page)doc.GetObjectById("mainSection");
// get reference of first TextSegment with ID boldHtml
TextSegment segment = (TextSegment)doc.GetObjectById("boldHtml");
// get reference of second TextSegment with ID strongHtml
segment = (TextSegment)doc.GetObjectById("strongHtml");
// save resultant PDF file
doc.Save("Resultant.pdf");
```

For more information, please visit Convert an XML file to PDF.

## Add to Grouped Checkboxes in PDF

The Document class provides a collection named Form which helps you manage form fields in a PDF document. The RadioButtonField provides the feature to add RadioButtons field to PDF document and in order to represent checkboxes, you may consider setting border style for RadioButtonField. Once the RadioButtonField object is created, you need to add RadioButtonOptionField instances to RadioButtonField object and in order to set border style, you need to use Style property and set value from BoxStyle enumeration.

```
// instantiate Document object
Document pdfDocument = new Document();
// add a page to PDF file
Page page = pdfDocument.Pages.Add();
// instatiate RadioButtonField object with page number as argument
RadioButtonField radio = new RadioButtonField(pdfDocument.Pages[1]);
// add first radio button option and also specify its origin using Rectangle object
RadioButtonOptionField opt1 = new RadioButtonOptionField(page, new Aspose.Pdf.Rectangle(0, 0, 20, 20));
RadioButtonOptionField opt2 = new RadioButtonOptionField(page, new Aspose.Pdf.Rectangle(100, 0, 120, 20));
opt1.OptionName = "Test1";
opt2.OptionName = "Test2";

radio.Add(opt1);
radio.Add(opt2);
opt1.Style = Aspose.Pdf.InteractiveFeatures.Forms.BoxStyle.Square;
opt2.Style = Aspose.Pdf.InteractiveFeatures.Forms.BoxStyle.Square;
opt1.Style = BoxStyle.Cross;
opt2.Style = BoxStyle.Cross;
opt1.Border = new Border(opt1);
opt1.Border.Style = Aspose.Pdf.InteractiveFeatures.Annotations.BorderStyle.Solid;
opt1.Border.Width = 1;
opt1.Characteristics.Border = System.Drawing.Color.Black;
opt2.Border = new Border(opt2);
opt2.Border.Width = 1;

opt2.Border.Style = Aspose.Pdf.InteractiveFeatures.Annotations.BorderStyle.Solid;
opt2.Characteristics.Border = System.Drawing.Color.Black;


// add radio button to form object of Document object
pdfDocument.Form.Add(radio);
// save the PDF file
pdfDocument.Save("c:/pdftest/RadioButtonSample.pdf");
```

## Create a Rectangle with Alpha Color Channel

Aspose.Pdf for .NET supports the feature to add graph objects (for example graph, line, rectangle etc.) to PDF documents. It also offers the feature to fill the rectangle object with a certain color. A rectangle object can also have Alpha color channel to give a transparent appearance.

```
// instantiate Document instance
Document doc = new Document();
// add page to pages collection of PDF file
Aspose.Pdf.Page page = doc.Pages.Add();
// create Graph instance
Aspose.Pdf.Drawing.Graph canvas = new Aspose.Pdf.Drawing.Graph(100, 400);
// create rectangle object with specific dimensions
Aspose.Pdf.Drawing.Rectangle rect = new Aspose.Pdf.Drawing.Rectangle(100, 100, 200, 100);
// set graph fill color from System.Drawing.Color structure from a 32-bit ARGB value
rect.GraphInfo.FillColor = Aspose.Pdf.Color.FromRgb(System.Drawing.Color.FromArgb(128, System.Drawing.Color.FromArgb(12957183)));
// add rectangle object to shapes collection of Graph instance
canvas.Shapes.Add(rect);

// create second rectangle object
Aspose.Pdf.Drawing.Rectangle rect1 = new Aspose.Pdf.Drawing.Rectangle(200, 150, 200, 100);
rect1.GraphInfo.FillColor = Aspose.Pdf.Color.FromRgb(System.Drawing.Color.FromArgb(128, System.Drawing.Color.FromArgb(16118015)));
canvas.Shapes.Add(rect1);
// add graph instance to paragraph collection of page object
page.Paragraphs.Add(canvas);
// save resultant file
doc.Save("c:/Rectangle_with_Alpha_Color_Channel.pdf");
```

For further details, please visit [Create Rectangle with Alpha color channel][2]

## Add Drawing with Transparent Color

While creating drawing objects such as Rectangle, Circle, Eclipse etc, we provide color information for border as well as fill color information. In order to have transparent fill impression, the \*FromArgb(..)\* method of Aspose.Pdf.Color object can be used. Please take a look over following code snippet which demonstrates the feature to fill rectangle object with transparent color.

```
int alpha = 10;
int green = 0;
int red = 100;
int blue = 0;
// create Color object using Alpha RGB 
Aspose.Pdf.Color alphaColor = Aspose.Pdf.Color.FromArgb(alpha, red, green, blue); // provide alpha channel
// instantiate Document object
Document document = new Document();
// add page to pages collection of PDF file
Page page = document.Pages.Add();
// create Graph object with certain dimensions
Aspose.Pdf.Drawing.Graph graph = new Aspose.Pdf.Drawing.Graph(300, 400);
// set border for Drawing object
graph.Border = (new Aspose.Pdf.BorderInfo(Aspose.Pdf.BorderSide.All, Aspose.Pdf.Color.Black));
// add graph object to paragraphs collection of Page instance
page.Paragraphs.Add(graph);
// create Rectangle object with certain dimensions
Aspose.Pdf.Drawing.Rectangle rectangle = new Aspose.Pdf.Drawing.Rectangle(0, 0, 100, 50);
// create graphInfo object for Rectangle instance
Aspose.Pdf.GraphInfo graphInfo = rectangle.GraphInfo;
// set color information for GraphInfo instance
graphInfo.Color = (Aspose.Pdf.Color.Red);
// set fill color for GraphInfo
graphInfo.FillColor = (alphaColor);
// add rectangle shape to shapes collection of graph object
graph.Shapes.Add(rectangle);
// save PDF file
document.Save("c:/pdftest/TransparentColor.pdf");
```

Further details can be found over [How to add drawing with transparent Color][3].

## Add Transparent Text in PDF

A PDF file contains Image, Text, Graph, attachment, Annotations objects and while creating TextFragment, you can set foreground, background color information as well as text formatting. Aspose.Pdf for .NET supports the feature to add text with Alpha color channel.

```
// create Document instance
Document doc = new Document();
// create page to pages collection of PDF file
Aspose.Pdf.Page page = doc.Pages.Add();

// create Graph object 
Aspose.Pdf.Drawing.Graph canvas = new Aspose.Pdf.Drawing.Graph(100, 400);
// create rectangle instance with certain dimensions
Aspose.Pdf.Drawing.Rectangle rect = new Aspose.Pdf.Drawing.Rectangle(100, 100, 400, 400);
// create color object from Alpha color channel
rect.GraphInfo.FillColor = Aspose.Pdf.Color.FromRgb(System.Drawing.Color.FromArgb(128, System.Drawing.Color.FromArgb(12957183)));
// add rectanlge to shapes collection of Graph object
canvas.Shapes.Add(rect);
// add graph object to paragraphs collection of page object
page.Paragraphs.Add(canvas);
// set value to not change position for graph object
canvas.IsChangePosition = false;

// create TextFragment instance with sample value
TextFragment text = new TextFragment("transparent text transparent text transparent text transparent text transparent text transparent text transparent text transparent text transparent text transparent text transparent text transparent text transparent text transparent text transparent text transparent text ");
// create color object from Alpha channel
Aspose.Pdf.Color color = Aspose.Pdf.Color.FromArgb(30, 0, 255, 0);
// set color information for text instance
text.TextState.ForegroundColor = color;
// add text to paragraphs collection of page instance
page.Paragraphs.Add(text);
// save PDF file
doc.Save("c:/pdftest/Transparent_Text.pdf");
```

For more information, please visit How to add transparent Text in PDF.

## Miscellaneous fixes

As well as the enhancements and features discussed above, there have been specific improvements regarding Footnote rendering, TOC rendering, PDF to HTML, HTML to PDF conversion features. Among these fixes, the PCL to PDF, SVG to PDF, PDF to Excel, PDF to DOC, PDF to TIFF, XML to PDF, TIFF to PDF conversion, conversion of PDF to PDF/A compliant documents, text replacement, rendering PDF files to XPS format are also improved. Please download and try the latest release of [Aspose.PDF for .NET 11.2.0][4].




[1]: https://downloads.aspose.com/pdf/net
[2]: https://docs.aspose.com/display/pdfnet/Working+with+Graphs#WorkingwithGraphs-CreateRectanglewithAlphacolorchannel
[3]: https://docs.aspose.com/display/pdfnet/Working+with+Graphs#WorkingwithGraphs-HowtoadddrawingwithtransparentColor
[4]: https://downloads.aspose.com/pdf/net




