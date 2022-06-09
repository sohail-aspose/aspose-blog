---
title: 'Add or Update Hyperlinks in PDF using Java'
seoTitle: "Add Hyperlink in PDF in Java | Fetch and Update Hyperlinks in PDF"
description: "Use Java PDF API to add hyperlinks in PDF using Java. Add a hyperlink to a webpage, page, or an external PDF file. Update hyperlink in a PDF in Java."
date: Sat, 30 Apr 2022 15:16:00 +0000
draft: false
url: /2022/04/30/add-hyperlinks-in-pdf-using-java/
author: Usman Aziz
summary: '[PDF][1] is a popular document format that provides cross-platform support with a range of features to create rich documents. Furthermore, it supports a variety of elements such as media, forms, annotations, artifacts, etc. Among these elements, the hyperlinks are used quite often to navigate within the PDF, from one PDF to another, to open a URL, etc. So in this article, you will learn **how to add and update hyperlinks in PDF files programmatically in Java**.'
tags: ['Add Hyperlink in a PDF in Java', 'Add Hyperlink to an External PDF Java', 'Insert Hyperlink to a Particular Page Java', 'Java API to Add Hyperlinks in PDF', 'Java PDF Generator API', 'Update a Hyperlink in a PDF Java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Add-Hyperlink-in-PDF.png" alt="Add or Update Hyperlinks in PDF using Java">}}


[PDF][2] is a popular document format that provides cross-platform support with a range of features to create rich documents. Furthermore, it supports a variety of elements such as media, forms, annotations, artifacts, etc. Among these elements, the hyperlinks are used quite often to navigate within the PDF, from one PDF to another, to open a URL, etc. So in this article, you will learn **how to add and update hyperlinks in PDF files programmatically in Java**.

*   [Java API to Add Hyperlinks in PDF][3]
*   [Add Hyperlink in a PDF][4]
*   [Add Hyperlink for an External PDF][5]
*   [Insert Hyperlink to a Particular Page][6]
*   [Update a Hyperlink in a PDF][7]

## Java API to Add or Update Hyperlinks in PDF {#API-to-Add-Hyperlinks-in-PDF}

[Aspose.PDF for Java][8] is an amazing API for PDF generation and manipulation. Using the API, you can seamlessly create, process, and convert PDF files of simple and complex layouts. We will use this API to add and update hyperlinks in PDF files. You can [download][9] the API's JAR or install it using the following Maven configurations.

```
PM> Install-Package Aspose.PDF
```

## Add Hyperlink in a PDF in Java {#Add-Hyperlink-in-a-PDF}

The following are the steps to add a hyperlink to a PDF file in Java.

*   Create a new PDF or load an existing one using ******[Document][10]****** class.
*   Get the reference of the page where you want to add the hyperlink from **[Document.getPages()][11]** collection.
*   Create an object of **[LinkAnnotation][12]** class and set its properties.
*   Use **[LinkAnnotation.setAction()][13]** method to assign **[GoToURIAction][14]** object containing URL.
*   Add hyperlink to page using **[Page.getAnnotations().add()][15]** method.
*   Save PDF using ******[Document.save(String)][16]****** method.

The following code sample shows how to add a hyperlink in PDF in Java.

{{< gist aspose-com-gists 1a9e355db2f188865ecb308bf4ce050e "add-hyperlink-in-pdf.java" >}}

## Add Hyperlink for an External PDF in Java {#Add-Hyperlink-to-an-External-PDF}

You can also navigate to an external PDF file from a PDF using a hyperlink. The following steps demonstrate how to add a hyperlink for an external PDF file in Java.

*   Create a new PDF or load an existing one using **[Document][17]** class.
*   Get the reference of the page where you want to add the hyperlink from **[Document.getPages()][18]** collection.
*   Create an object of **[LinkAnnotation][19]** class and set its properties.
*   Use **[LinkAnnotation.setAction()][20]** method to set action to **[GoToRemoteAction][21]** object containing path to external PDF.
*   Add hyperlink to page using **[Page.getAnnotations().add()][22]** method.
*   Save PDF using **[Document.save(String)][23]** method.

The following code sample shows how to add a hyperlink for an external PDF in Java.

{{< gist aspose-com-gists 1a9e355db2f188865ecb308bf4ce050e "add-hyperlink-to-external-pdf.java" >}}

## Insert Hyperlink to a Particular PDF Page {#Insert-Hyperlink-to-a-Particular-Page}

In certain cases, you have to navigate from one page to another within a PDF document. The [**LocalHyperlink**][24] class is used to navigate to a particular page in a PDF. The following are the steps to achieve this.

*   Create a new PDF or load an existing one using **[Document][25]** class.
*   Get the reference of the page where you want to add the hyperlink from **[Document.getPages()][26]** collection.
*   Create an instance of **[TextFragment][27]** class to set the text of the hyperlink.
*   Create an instance of **[LocalHyperlink][28]** class and use **[**LocalHyperlink**.setTargetPageNumber()][29]** method to set the target page number.
*   Assign **LocalHyperlink** object using **[TextFragment.setHyperlink()][30]** method.
*   Add text to the page using **[Page.getParagraphs().add(TextFragment)][31]** method.
*   Save PDF using **[Document.save(String)][32]** method.

The following code sample shows how to add a hyperlink to navigate to a particular page in PDF.

{{< gist aspose-com-gists 1a9e355db2f188865ecb308bf4ce050e "add-hyperlink-to-pdf-page.java" >}}

## Update a Hyperlink in PDF using Java {#Update-Hyperlink-in-PDF}

You can also retrieve a hyperlink from a PDF file and update its properties. The following are the steps to perform this operation.

*   Create a new PDF or load an existing one using **[Document][33]** class.
*   Get the reference of the page where the hyperlink is located from **[Document.getPages()][34]** collection.
*   Extract the desired ****[LinkAnnotation][35]**** object by index using **[Page.getAnnotations().get\_item()][36]** method.
*   Update the required properties of hyperlink and save PDF using **[Document.save(String)][37]** method.

The following code sample shows how to update a hyperlink in PDF using Java.

{{< gist aspose-com-gists 1a9e355db2f188865ecb308bf4ce050e "update-hyperlink-in-pdf.java" >}}

## Get a Free License {#Get-a-Free-License}

You can [get a free temporary license][38] in order to use Aspose.PDF for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to add different types of hyperlinks in PDF files using Java. Furthermore, you have seen how to retrieve the hyperlinks from existing PDF files and update their properties programmatically. In addition, you can explore more about Java PDF API using the [documentation][39]. In case you would have any questions or queries, you can contact us via our [forum][40].

## See Also

*   [Creating PDF Files from Scratch using Java][41]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: #API-to-Add-Hyperlinks-in-PDF
[4]: #Add-Hyperlink-in-a-PDF
[5]: #Add-Hyperlink-to-an-External-PDF
[6]: #Insert-Hyperlink-to-a-Particular-Page
[7]: #Update-Hyperlink-in-PDF
[8]: https://products.aspose.com/pdf/java/
[9]: https://downloads.aspose.com/pdf/java
[10]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[11]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#getPages--
[12]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/LinkAnnotation
[13]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/LinkAnnotation#setAction-com.aspose.pdf.PdfAction-
[14]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/PdfAction
[15]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/AnnotationCollection#add-com.aspose.pdf.Annotation-
[16]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[17]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[18]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#getPages--
[19]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/LinkAnnotation
[20]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/LinkAnnotation#setAction-com.aspose.pdf.PdfAction-
[21]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/PdfAction
[22]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/AnnotationCollection#add-com.aspose.pdf.Annotation-
[23]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[24]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/LocalHyperlink
[25]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[26]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#getPages--
[27]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextFragment
[28]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/LocalHyperlink
[29]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/LocalHyperlink#setTargetPageNumber-int-
[30]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextFragment#setHyperlink-com.aspose.pdf.Hyperlink-
[31]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Paragraphs#add-com.aspose.pdf.BaseParagraph-
[32]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[33]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[34]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#getPages--
[35]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/LinkAnnotation
[36]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/AnnotationCollection#get_Item-int-
[37]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[38]: https://purchase.aspose.com/temporary-license
[39]: https://docs.aspose.com/pdf/java/
[40]: https://forum.aspose.com/
[41]: https://blog.aspose.com/2020/12/31/create-pdf-files-in-java/




