---
title: 'Rotate Text inside PDF Documents in Java'
seoTitle: "Rotate Text inside PDF in Java | Java PDF Generator API"
description: "Use Java PDF generator API to rotate text inside PDF documents programmatically in Java. Rotate text fragments or paragraphs dynamically in a PDF file."
date: Sun, 17 Apr 2022 16:42:00 +0000
draft: false
url: /2022/04/17/rotate-text-inside-pdf-documents-in-java/
author: Usman Aziz
summary: '[PDF][1] is a cross-platform document format that provides a consistent layout across different operating systems. It is widely used for generating and sharing documents, such as research articles, invoices, etc. While generating a PDF files programmatically, you often need to change the position and orientation of the text according to the layout of the document. In this article, we will show you **how to rotate text inside PDF documents in Java**.'
tags: ['Apply Text Rotation using TextFragment in Java', 'Apply Text Rotation using TextParagraph in Java', 'Java API to Rotate Text in PDF', 'Java PDF Generator API', 'Rotate Text inside a PDF File in Java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Rotate-Text-in-PDF.jpg" alt="Rotate Text inside PDF Documents in Java">}}


[PDF][2] is a cross-platform document format that provides a consistent layout across different operating systems. It is widely used for generating and sharing documents, such as research articles, invoices, etc. While generating a PDF files programmatically, you often need to change the position and orientation of the text according to the layout of the document. In this article, we will show you **how to rotate text inside PDF documents in Java**.

*   [Java API to Rotate Text in PDF][3]
*   [Rotate Text inside a PDF File][4]
    *   [Apply Text Rotation using TextFragment][5]
    *   [Apply Text Rotation using TextParagraph][6]

## Java API to Rotate Text in PDF {#API-to-Rotate-Text-in-PDF}

To rotate text inside PDF files, we will use [Aspose.PDF for Java][7]. It is a powerful library that provides basic as well as advanced PDF manipulation features. You can [download][8] the API or install it using the following Maven configurations.

```
**Repository:** <repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>

**Dependency:** <dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-pdf</artifactId>
    <version>22.4</version>
</dependency>
```

## Rotate Text inside PDF in Java {#Rotate-Text-inside-PDF}

There are multiple ways to rotate a text inside a PDF document. You can either rotate a text fragment or the complete paragraph. Let's see how each of these text rotations works.

### PDF Text Rotation using TextFragment in Java {#Apply-Text-Rotation-using-TextFragment}

The following are the steps to rotate a text fragment in a PDF document using Java.

*   First, create a new document using the [Document][9] class.
*   Then, add a page to the document and get its reference using [Document.getPages().add()][10] method.
*   After that, create a new text fragment using [TextFragment][11] class.
*   Set text fragment's position and font.
*   Set rotation angle using [TextFragment.getTextState().setRotation()][12] method.
*   Create a new [TextBuilder][13] object and initialize it with the _Page_ object.
*   Use [TextBuilder.appendText(TextFragment)][14] method to add text to the page.
*   Finally, save the PDF document using [Document.save(string)][15] method.

The following code sample shows how to rotate text in a PDF document in Java.

{{< gist aspose-com-gists 53f41801e9c9cb34512a4153cc858416 "rotate-text-using-textfragment.java" >}}

#### Output



{{< figure align=center src="images/PDF-Text-Rotation_TextFragment.png" alt="PDF Text Rotation using TextFragment in Java">}}


## PDF Text Rotation using TextParagraph in Java {#Apply-Text-Rotation-using-TextParagraph}

You can also apply rotation to the text while creating a new paragraph. This can be achieved using [TextParagraph][16] class. The following are the steps to apply text rotation using _TextParagraph_ class.

*   First, create a new document using the [Document][17] class.
*   Then, add a page to the document and get its reference using [Document.getPages().add()][18] method.
*   After that, create a new [TextParagraph][19] object.
*   Create a new text fragment using [TextFragment][20] class and set the text and font.
*   Set rotation angle using [TextFragment.getTextState().setRotation()][21] method.
*   Add text to paragraph using [TextParagraph.appendLine(TextFragment)][22] method.
*   Create a new [TextBuilder][23] object and initialize it with the _Page_ object.
*   Use [TextBuilder.appendParagraph(TextParagraph)][24] method to add paragraph to the page.
*   Finally, save the PDF document using the [Document.save(string)][25] method.

The following code sample shows how to rotate text inside a paragraph in PDF programmatically.

{{< gist aspose-com-gists 53f41801e9c9cb34512a4153cc858416 "rotate-text-using-textparagraph.java" >}}

#### Output



{{< figure align=center src="images/PDF-Text-Rotation_TextParagraph.png" alt="PDF Text Rotation using TextParagraph in Java">}}


## Get a Free API License {#Get-a-Free-API-License}

You can try Aspose.PDF for Java for free by [getting a temporary license][26].

## Conclusion

In this article, you have learned how to rotate text in PDF programmatically using Java. We have covered how to rotate text using _TextFragment_ and _TextParagraph_ classes. In addition, you can explore more about Aspose.PDF for Java using the [documentation][27]. In case you would have any questions or queries, you can contact us via our [forum][28].

## See Also

*   [Creating PDF Files from Scratch using Java][29]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: #API-to-Rotate-Text-in-PDF
[4]: #Rotate-Text-inside-PDF
[5]: #Apply-Text-Rotation-using-TextFragment
[6]: #Apply-Text-Rotation-using-TextParagraph
[7]: https://products.aspose.com/pdf/java/
[8]: https://downloads.aspose.com/pdf/java
[9]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[10]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/PageCollection
[11]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextFragment
[12]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextFragmentState#setRotation-double-
[13]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextBuilder
[14]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextBuilder#appendText-com.aspose.pdf.TextFragment-
[15]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[16]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextParagraph
[17]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[18]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/PageCollection
[19]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextParagraph
[20]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextFragment
[21]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextFragmentState#setRotation-double-
[22]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextParagraph#appendLine-com.aspose.pdf.TextFragment-
[23]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextBuilder
[24]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextBuilder#appendParagraph-com.aspose.pdf.TextParagraph-
[25]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[26]: https://purchase.aspose.com/temporary-license
[27]: https://docs.aspose.com/pdf/java/
[28]: https://forum.aspose.com/
[29]: https://blog.aspose.com/2020/12/31/create-pdf-files-in-java/




