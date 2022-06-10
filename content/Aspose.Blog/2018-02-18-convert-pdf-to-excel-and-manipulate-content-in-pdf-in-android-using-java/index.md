---
title: 'Convert PDF to Excel and Manipulate Content in PDF in Android using Java'
date: Sun, 18 Feb 2018 21:18:57 +0000
draft: false
url: /2018/02/18/convert-pdf-to-excel-and-manipulate-content-in-pdf-in-android-using-java/
author: Asad Ali
summary: ''
tags: ['Asad Ali', 'Convert PDF to Excel in Android', 'Convert PDF to XLS in Android', 'Convert PDF to XLSX in Android']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-Android_100.png" alt="">}}


After Aspose.PDF for Android via Java 17.7 release, we are honored to announce [Aspose.PDF for Android via Java 17.12][1]. Aspose.PDF for Android via Java 17.12 has been released for Android platforms and ready to be used in Android Applications. For a detailed overview of the changes and improvements in this new release of the API, please visit the release notes page in the API documentation. However, there are the following major features, we would like to mention, which have been added in [Aspose.PDF for Android via Java 17.12][2].

## Convert PDF to Excel in Android

Since Inter-File Formats Conversion has been an interesting feature of the APIs offered by Aspose – we have added support to convert PDF file into Excel format, in Aspose.PDF for Android via Java 17.12. This new release of the API offers you following two different methods which can be used according to your requirements regarding conversion:

*   Using [com.aspose.pdf.SaveFormat][3] Class
*   Using [ExcelSaveOptions][4] Class

The following code sample shows how to convert PDF to Excel in Android using Java:

{{< gist aspose-pdf 474c352a71ac9477aa0d604fd32e1c6a "Examples-src-main-java-com-aspose-pdf-examples-CovertPDFtoXLSX.java" >}}

More details about this feature have also been given in [Convert PDF file to Excel Format][5] article of API documentation.

## Manipulate Tables in Existing PDF

Aspose.PDF for Android via Java 17.12, now offers the feature to search and parse simple tables that already exist in PDF document. This new feature in the API has come with the addition of new class **com.aspose.pdf.TableAbsorber** which provides the capabilities to search and manipulate the tables in PDF documents. The usage of **TableAbsorber** is very much similar to the existing **TextFragmentAbsorber** Class. The following code snippet shows the steps to update contents in particular table cell:

```
String inputPath = "/mnt/sdcard/Table.pdf";
String outputPath = "/mnt/sdcard/Table_out.pdf";
// Load document
Document pdfDocument = new Document(inputPath);
// Create TableAbsorber object to find tables
TableAbsorber absorber = new TableAbsorber();
// Visit first page with absorber
absorber.visit(pdfDocument.getPages().get_Item(1));
// Get access to first table on page, their first cell and 
// text fragments in it
Table table = (Table) absorber.getTableList().get_Item(0);                      
Cell cell = table.getRows().get_Item(0).getCells().get_Item(0);                  
TextFragment fragment = 
(TextFragment) cell.getParagraphs().get_Item(1);
// Change text of the first text fragment in the cell
fragment.setText ("Hello World!");
// Save updated document
pdfDocument.save(outputPath);
```

## Apply Gradient Color to Graph

We have implemented support for gradient color in Aspose.PDF for Android via Java 17.12, in order to apply gradient color to the Graph. The feature can be used with new property **PatternColorSpace** and class **GradientAxialShading** which has been added into **com.aspose.pdf.drawing** Package. The following code snippet demonstrates the usage of new added properties and classes, in order to apply gradient color:

```
String outputPath = "/mnt/sdcard/GradientColor_out.xlsx";
// Initialize Document object
Document doc = new Document();
// Add a new page
Page page = doc.getPages().add();
Graph graph = new Graph(300, 300);
// Add a Graph
page.getParagraphs().add(graph);
com.aspose.pdf.drawing.Rectangle rect = 
new com.aspose.pdf.drawing.Rectangle(0, 0, 300, 300);
graph.getShapes().add(rect);
rect.getGraphInfo().setFillColor(new com.aspose.pdf.Color());
// Use GradientAxialShadding for Gradient
GradientAxialShading gradientAxialShading = 
new GradientAxialShading(Color.getRed(), Color.getBlue());
gradientAxialShading.setStart(new Point(0, 0));
gradientAxialShading.setEnd(new Point(300, 300));
rect.getGraphInfo().getFillColor().setPatternColorSpace(gradientAxialShading);
// Save the document
doc.save(outputPath);
```

## Miscellaneous Fixes and Resources

Along with the new features, which have been shared above, we have also made some bug fixes in this release of the API – which can be seen in the release notes section of the API documentation. Please visit the following links for information regarding the latest release of Aspose.PDF for Android via Java and Release Notes section. In case you have any questions about Aspose.PDF for Android via Java, you can post your inquiry in [Aspose.PDF forums][6]. We will be more than happy to assist you there.

*   [Homepage for Aspose.PDF for Android via Java][7]
*   [Download Aspose.PDF for Android via Java][8]
*   [Aspose.PDF product family forum][9]– Post your technical questions and queries, or any other problem you face while running Aspose.PDF APIs.
*   Aspose.PDF for Android via Java online documentation– Help documentation on using Aspose.PDF for Android via Java API.
*   [Aspose.PDF for Android via Java API Reference][10]– Online public API reference for using the API.
*   [Enable Blog Subscription][11]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.PDF APIs, new features, fixes and other API related topics by subscribing to Aspose.PDF blog.




[1]: http://maven.aspose.com/artifactory/simple/ext-release-local/com/aspose/aspose-pdf-android-via-java/17.12/
[2]: http://maven.aspose.com/artifactory/simple/ext-release-local/com/aspose/aspose-pdf-android-via-java/17.12/
[3]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/SaveFormat
[4]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/ExcelSaveOptions
[5]: https://docs.aspose.com/display/pdfjava/Convert+PDF+to+Excel+XLS+and+XLSX
[6]: https://forum.aspose.com/c/pdf
[7]: https://products.aspose.com/pdf/android-java
[8]: http://maven.aspose.com/artifactory/simple/ext-release-local/com/aspose/aspose-pdf-android-via-java/17.12/
[9]: https://forum.aspose.com/c/pdf
[10]: https://apireference.aspose.com/java/pdf
[11]: https://blog.aspose.com/category/aspose-products/aspose-pdf-product-family/




