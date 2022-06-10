---
title: 'Set Best Fit Position of Data Labels in Pie Chart in Word Documents using Aspose.Words'
date: Sat, 12 Apr 2014 06:15:37 +0000
draft: false
url: /2014/04/12/partial-support-for-eudc-fonts-best-fit-position-of-data-labels-in-pie-chart-insertion-of-ole-objects-in-aspose.words-14.3.0/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose.words_logo.png" alt="Aspose.Words logo">}}


Aspose.Words 14.3.0 has been released with this month’s release containing over 95 useful new features, enhancements and bug fixes to the Aspose.Words products.

You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 14.3.0][1]
*   [Aspose.Words for Java 14.3.0][2]

Here is a look at just a few of the biggest features in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the links above.

## Best Fit Position of Data Labels in Pie Chart

Starting from Aspose.Words 14.3.0, Best Fit position of data labels in pie charts is partially supported. In previous versions, labels with best-fit positions were rendered as if they had the inside end position. Currently, we use a modified Open Office algorithm to set the best fit position of data labels. Here are a few examples:

1\. Best fit position of data labels of the 2D Pie chart:



{{< figure align=center src="images/TestDataLabelBestFitPosition-Pdf-0-Gold.png" alt="">}}


2\. Best fit position of data labels of the 3D Pie chart:



{{< figure align=center src="images/TestDataLabelBestFitPosition-Pdf-1-Gold.png" alt="">}}


## Partial Support of EUDC Fonts

Aspose.Words' rendering engine now partially supports EUDC (End-User-Defined-Characters) fonts. Please find below the description of how EUDC fonts work on Windows (Microsoft Word also seems to follow this logic in general):

*   [End-User-Defined and Private Use Area Characters][3].aspx)

In this first implementation, Aspose.Words uses a single EUDC font. When rendering a document to fixed-page formats, this font is searched among the specified font sources by "EUDC" family name.

## Insert Embedded or Linked OLE Objects

Aspose.Words now supports insertion of OLE objects such as another Microsoft Word document or a Microsoft Excel chart. A new public method, InsertOleObject, has been introduced in the DocumentBuilder class. This method can be used to insert an embedded or linked OLE object from a file into a Word document.

The following code inserts embedded Excel 97-2003 document as iconic OLE object from the stream using the predefined image.

```
Document doc = new Document();
DocumentBuilder builder = new DocumentBuilder(doc);
Stream memoryStream = File.OpenRead(MyDir + "Book1.xls");
Shape oleObject = builder.InsertOleObject(memoryStream, "Excel.Sheet.8", true, null);
doc.Save(MyDir + @"out.docx");
```

The following code inserts linked Word document from file as normal OLE object using a custom presentation image.

```
Document doc = new Document();
DocumentBuilder builder = new DocumentBuilder(doc);
Image image = Image.FromFile(MyDir + "Aspose.Words.png");
Shape oleObject = builder.InsertOleObject(MyDir + "Doc1.docx", true, false, image);
doc.Save(MyDir + @"out.docx");
```



[1]: https://downloads.aspose.com/words/net
[2]: https://downloads.aspose.com/words/java
[3]: http://msdn.microsoft.com/en-us/library/windows/desktop/dd317802(v=vs.85




