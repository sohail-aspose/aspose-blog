---
title: 'Get Height of Table in PDF File and Convert PDF to PDF/A with Aspose.PDF for Java 17.6'
date: Fri, 14 Jul 2017 11:23:02 +0000
draft: false
url: /2017/07/14/get-height-table-existing-pdf-file-reliable-pdf-pdfa-conversion-features-aspose.pdf-java-17.6/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'Add or manipuate tables in PDF in Java', 'Convert PDF to PDF/A in Java', 'Get table height in existing PDF in Java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-Java.png" alt="">}}


A new release of [Aspose.PDF for Java 17.6][1] has been published offering a new feature to Get height of table in existing PDF file. Apart from this new feature, we have also introduced many fixes related to bus reported in earlier release versions. In fact, the conversion of PDF files to PDF/A format has been specifically improved to cater wide variety of PDF files.

## Get Height of Table in Existing PDF File

Aspose.PDF for Java offers the feature to [Add table in existing PDF file][2], as well as [Manipulate tables in existing PDF file][3]. Starting this new release, we also have introduced the feature to Get height of table in existing PDF document. In order to get the height information, we need to create an instance of **TableAbsorber** instance, iterate through page of PDF file, get rectangular instance for table object and then print the Height and Width information of extracted table instance.

```
// load an existing PDF document
Document doc = new Document("testtable2.pdf");
// get reference of first page of PDF document
Page page = doc.getPages().get_Item(1);
// instantiate TableAbsorber instance
TableAbsorber absorber = new TableAbsorber();
// iterate through first page of PDF file
absorber.visit(page);
// get rectangular region of first table instance
Rectangle table1_rect = absorber.getTableList().get_Item(0).getRectangle();
// print height and width of table instance
System.out.println("height: " + table1_rect.getHeight() + "; width: " + table1_rect.getWidth());
```

The following code snippets shows the steps to determine the rectangular region of two tables already present inside PDF file and then draw a LineAnnotation between the gap of both tables.

```
// load an existing PDF document
Document doc = new Document("testtable2.pdf");
// get reference of first page of PDF document
Page page = doc.getPages().get_Item(1);
// instantiate TableAbsorber instance
TableAbsorber absorber = new TableAbsorber();
// iterate through first page of PDF file
absorber.visit(page);
// get rectangular region of first table instance
Rectangle table1_rect = absorber.getTableList().get_Item(0).getRectangle();
//get rectangular region of second table instance
Rectangle table2_rect = absorber.getTableList().get_Item(1).getRectangle();
// get lowerLeftX and LowerLeftY for first table instance
Point point1 = new Point(table1_rect.getLLX(), table1_rect.getLLY());
Point point2 = new Point(table2_rect.getURX() - table2_rect.getWidth(), table2_rect.getURY());
// get rectangular region around first table
Rectangle rect = new Rectangle(table1_rect.getLLX(), table1_rect.getLLY(), table2_rect.getURX() - table2_rect.getWidth(), table2_rect.getURY());
// create Lineannotation instance
LineAnnotation lineBetweenTables = new LineAnnotation(page, rect, point1, point2);
// set LineEnding style as OpenArrow
lineBetweenTables.setEndingStyle(LineEnding.OpenArrow);
//set LineStarting style as OpenArrow
lineBetweenTables.setStartingStyle(LineEnding.OpenArrow);
// create border instance    
com.aspose.pdf.Border border = new com.aspose.pdf.Border(lineBetweenTables);
// set border width
border.setWidth(1);
// set line foreground color as blue        
lineBetweenTables.setColor(Color.getBlue());
// set border for LineAnnotation
lineBetweenTables.setBorder(border);                
// add Annotation to Annotations collection of first page of PDF file         
page.getAnnotations().add(lineBetweenTables);
// save PDF document
doc.save("c:/pdftest/testtableOut.pdf");
```



{{< figure align=center src="images/Line_Between_Tables.png" alt="">}}


Please notice the blue line in above image.

## Miscellaneous fixes

As mentioned above, the significant improvements have been made in PDF to PDF/A conversion. Furthermore, the HTML to PDF conversion, PDF to DOCX and PCL file to PDF conversion are also among the improvement features which help to create output files with great fidelity. As it is always recommended to use latest release of our API's, so we suggest you to please download the latest release of [Aspose.PDF for Java 17.6][4] and check Release Notes section regarding list of issues fixed in [Aspose.PDF for Java 17.6][5]

*   [Home page for Aspose.PDF for Java][6]
*   [Download Aspose.PDF for Java][7]
*   [Aspose.PDF product family forum][8]– Post your technical questions and queries, or any other problem you faced while running Aspose.PDF APIs.
*   [Aspose.PDF for Java online documentation][9]– help documentation and API reference documents.
*   [Enable Blog Subscription][10]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.PDF APIs, new features, fixes and other API related topics by subscribing to Aspose.PDF blog.
*   [Aspose.PDF for Java Examples][11] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/pdf/java/new-releases/aspose.pdf-for-java-17.6/
[2]: https://docs.aspose.com/display/pdfjava/Add+Table+in+Existing+PDF+Document
[3]: https://docs.aspose.com/display/pdfjava/Manipulate+tables+in+existing+PDF
[4]: https://downloads.aspose.com/pdf/java/new-releases/aspose.pdf-for-java-17.6/
[5]: https://docs.aspose.com/display/pdfjava/Aspose.Pdf+for+Java+17.6+Release+Notes
[6]: https://www.aspose.com/products/pdf/java
[7]: https://downloads.aspose.com/pdf/java
[8]: https://forum.aspose.com/c/pdf
[9]: https://docs.aspose.com/display/pdfjava/Home
[10]: https://blog.aspose.com/category/aspose-products/aspose-pdf-product-family/
[11]: https://github.com/aspose-pdf/Aspose.Pdf-for-Java




