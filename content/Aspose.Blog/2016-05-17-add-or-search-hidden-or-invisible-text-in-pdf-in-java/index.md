---
title: 'Add and Search Hidden Text in PDF Documents using Java'
date: Tue, 17 May 2016 16:10:29 +0000
draft: false
url: /2016/05/17/add-or-search-hidden-or-invisible-text-in-pdf-in-java/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'Add Hidden Text in PDF in Java', 'Extract Hidden Text in PDF in Java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-Java_100.png" alt="Aspose.Pdf for .NET logo">}}


As a part of our continuous improvement process, a new release of [Aspose.PDF for Java 11.4.0][1] has been released having the capability to add or search hidden text in PDF documents. Furthermore, we have introduced the feature to use PDF file objects after calling ProcessPragraphs() method, so that further manipulation can be performed over this object (_it was not possible with earlier release versions_).

## Add and Search Hidden Text in PDF using Java

In order to add hidden text, pass an argument of true to TextState.setInvisible(...) method. TextFragmentAbsorber finds the text that matches pattern (if specified). Please note that hidden text in the document will only be invisible for end-user while viewing the document with PDF reading software (e.g. Acrobat Reader). There are several ways to make text invisible for end-user in PDF and we have implemented one of those techniques. However, the text added through this approach can be found using TextFragmentAbsorber class and we can not guarantee that any hidden text added by third-party applications can be found using the same approach. However, in case you encounter any issue, please share the resource file and we can further investigate the scenario.

**Public API changes**  
The following methods are added:

*   com.aspose.pdf.TextFragmentState.isInvisible()
*   com.aspose.pdf.TextFragmentState.setInvisible(boolean)
*   com.aspose.pdf.TextState.isInvisible()
*   com.aspose.pdf.TextState.setInvisible(boolean)

```
//Create document with hidden text
 com.aspose.pdf.Document doc = new com.aspose.pdf.Document();
 // add page to pages collection of PDF file
 Page page = doc.getPages().add();
 // create TextFragment instance
 TextFragment frag1 = new TextFragment("This is common text.");
 TextFragment frag2 = new TextFragment("This is invisible text.");
 //Set text property - invisible
 frag2.getTextState().setInvisible(true);
 // add TextFragment to paragraphs collection of page instance
 page.getParagraphs().add(frag1);
 page.getParagraphs().add(frag2);
 // save the PDF document
 doc.save("c:/pdftest/HiddenText_output.pdf");
 doc.dispose();

 //Search text in the document
 doc = new com.aspose.pdf.Document("c:/pdftest/HiddenText_output.pdf");
 // create TextFragmentAbsorber instance
 TextFragmentAbsorber absorber = new TextFragmentAbsorber();
 // get text content from first page of PDF file
 absorber.visit(doc.getPages().get_Item(1));
 // iterate through TextFragment inside TextFragments collection 
 for(com.aspose.pdf.TextFragment fragment : (Iterable)absorber.getTextFragments())
 {
     //Display extracted TextFragments and their related properties
     System.out.println("Text = " +fragment.getText() + ", on pos = "+ fragment.getPosition().toString() + 
    		 " and invisibility = " + fragment.getTextState().isInvisible());
 }
 // dispose Document object
 doc.dispose();
```

## Using Page Object after ProcessPragraphs() Call

The processParagraphs() method was introduced to calculate objects placed inside PDF file and in case we need to have page count information during PDF file generation, this method can be used as it manipulates file objects and returns the desired information. In earlier release versions, once this method was called, the file objects could not be accessed any further. So if you need to add any new object to the existing page instance, it was not possible and you had to have a new Page instance where objects can be placed. Nevertheless, starting this new release, you can utilize the same Page objects even after calling the processParagraphs() method.

```
// instantiate Document object
 Document document = new Document();
 // add page to pages collection of PDF file
 Page page1 = document.getPages().add();

 // create a loop to add 5 TextFragments
 for (int i = 1; i <= 5; i++)
 {
	 // create table object
	 Table table1 = new com.aspose.pdf.Table();
	 // set width for Table columns
	 table1.setColumnWidths("100");
	 // render table in new page
	 table1.setInNewPage(true);
	 // create a row object and add it to rows collection of table instance
	 com.aspose.pdf.Row row1 = table1.getRows().add();
	 // create TextFragment
	 TextFragment tf = new TextFragment("part"+ i);
	 tf.setInLineParagraph(false);
	 tf.setKeptWithNext(false);
	 // add cell to cells collection of row instance
	 com.aspose.pdf.Cell cell1 = row1.getCells().add();
	 // add text fragment to paragraphs collection of table cell
	 cell1.getParagraphs().add(tf);
	 // add table to paragraphs collection of page object
	 page1.getParagraphs().add(table1);

	 // process paragraph objects inside PDF
	 document.processParagraphs();
	 // get page count information from PDF file
	 System.out.println("Number of pages in PDF = " + document.getPages().size());
 }
 // save resultant file
 document.save("c:/PageCount_out.pdf");
```

## Rotate Method in FreeTextAnnotation Class

A new Rotate(...) method is added for annotation which provides the capabilities to change annotations orientation.

**Public API changes**  
The following methods are added:

*   com.aspose.pdf.FreeTextAnnotation.getRotate
*   com.aspose.pdf.FreeTextAnnotation.setRotate(int)
*   com.aspose.pdf.Rectangle.rotateAngle(int)

```
// instantiate Document object
 Document document = new Document();
 // add page to pages collection of PDF file
 Page page1 = document.getPages().add();
// create FreeTextAnnotation instance
 FreeTextAnnotation annotation = new FreeTextAnnotation(document.getPages().get_Item(1), new com.aspose.pdf.Rectangle(50, 600, 250, 630),
 new DefaultAppearance("Helvetica", 16, java.awt.Color.RED));
// set contents for FreeTextAnnotation
 annotation.setContents("ABCDEFG");
 // set rotating angle for Annotation
 annotation.setRotate(Rotation.on90);
 // create Rectangle object as per Annotation dimensions
 Rectangle rect = annotation.getRect();
 // rotate Rectangle object
 rect.rotateAngle(90);
 annotation.setRect(rect);
 // set border color for Annotation as Red
 annotation.getCharacteristics().setBorder(java.awt.Color.RED);
 // set border information for Annotation instance
 annotation.setBorder(new Border(annotation));
 // set border width information for annotation instance
 annotation.getBorder().setWidth(1);
 // add annotation to first page of PDF file
 document.getPages().get_Item(1).getAnnotations().add(annotation);
 // save resultant file
 document.save("c:/pdftest/Annotation_Rotate.pdf");
```

## Miscellaneous Fixes

As well as the enhancements and features discussed above, there have been specific improvements regarding Text extraction from PDF, image placement inside PDF, PDF to HTML, HTML to PDF, PDF to PDF/A, XPS to PDF, PDF to Image, PDF to TIFF, TIFF to PDF conversion and PDF printing are also improved. Please download and try the latest release of [Aspose.PDF for Java 11.4.0][2].




[1]: https://downloads.aspose.com/pdf/java
[2]: https://downloads.aspose.com/pdf/java




