---
title: 'Create Tagged PDF Files in Java'
seoTitle: "Create Tagged PDF Files in Java | Java PDF Generator Library"
description: "Use Java PDF Generator library to create tagged PDF files in Java. Create nested elements, apply styling, and illustrate structure elements in tagged PDF."
date: Mon, 25 Apr 2022 12:23:00 +0000
draft: false
url: /2022/04/25/create-tagged-pdf-files-in-java/
author: Usman Aziz
summary: 'A tagged [PDF][1] file uses tags to define the logical structure of the content in the document. This type of PDF file improves the reading experience using assistive technologies and screen readers. In the [previous post][2], you have seen how to create PDF files programmatically in Java applications. In this article, you will learn **how to create tagged PDF files programmatically in Java**.'
tags: ['Create a Tagged PDF File in Java', 'Create a Tagged PDF with Nested Elements', 'Illustrating Structure Elements in a Tagged PDF', 'Java API to Create Tagged PDF Files', 'Styling Text Structure in a Tagged PDF']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Create-Tagged-PDF-File.png" alt="Create Tagged PDF Files in Java">}}


A tagged [PDF][3] file uses tags to define the logical structure of the content in the document. This type of PDF improves the reading experience using assistive technologies and screen readers. In the [previous post][4], you have seen how to create PDF files programmatically in Java applications. In this article, you will learn **how to create tagged PDF files programmatically in Java**.

*   [Java API to Create Tagged PDF Files][5]
*   [Create a Tagged PDF File][6]
*   [Create a Tagged PDF with Nested Elements][7]
*   [Styling Text Structure in a Tagged PDF][8]
*   [Illustrating Structure Elements in a Tagged PDF][9]

## Java API to Create Tagged PDF Files {#API-to-Create-Tagged-PDF-Files}

To create the tagged PDF files, we will use [Aspose.PDF for Java][10]. It is one of the popular APIs for PDF generation and manipulation. Using the API, you can seamlessly create, process, and convert PDF files of simple and complex layouts. You can [download][11] the API or install it using the following Maven configurations.

```
**Repository:**
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>

**Dependency:**
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-pdf</artifactId>
    <version>22.4</version>
</dependency>
```

## Create a Tagged PDF File in Java {#Create-a-Tagged-PDF-File}

To create structure elements in a tagged PDF, _Aspose.PDF for Java_ provides the ****[ITaggedContent][12]**** interface. So let's see how to use this interface to create a tagged PDF file in Java.

*   Create a new PDF using the **[Document][13]** class.
*   Get the reference of the **[TaggedContent][14]** of the document into an ******[ITaggedContent][15]****** object.
*   Set title, header, and language and add elements to the PDF using the ******ITaggedContent****** object.
*   Create a new ****[ParagraphElement][16]**** using **[ITaggedContent.createParagraphElement()][17]** method and set its text.
*   Add the paragraph to the document using **[ITaggedContent.getRootElement().appendChild()][18]** method.
*   Finally, save the PDF file using ******[Document.save(String)][19]****** method.

The following code sample shows how to create a tagged PDF in Java.

{{< gist aspose-com-gists 191d997a5b1b0216a2b4d0546bcef9cf "create-tagged-pdf.java" >}}

The following is the output of the above code sample.



{{< figure align=center src="images/Create-Tagged-PDF-1024x477.png" alt="Create a Tagged PDF File in Java">}}


## Create a Tagged PDF with Nested Elements in Java {#Create-a-Tagged-PDF-with-Nested-Elements}

In the previous example, we created a simple tagged PDF that contains a paragraph. Let's now have a look at how to add nested elements in a tagged PDF. The following are the steps to perform this operation.

*   Create a new PDF or load an existing one using the ****[Document][20]**** class.
*   Get the reference of the ****[TaggedContent][21]**** of the document into an ******[ITaggedContent][22]****** object.
*   Set title, header, and language and add elements to the PDF using the **ITaggedContent** object.
*   Create a new ******[ParagraphElement][23]****** using ****[ITaggedContent.createParagraphElement()][24]**** method and set its text.
*   Use **[SpanElement][25]** class to add the nested elements.
*   Add nested element to paragraph using **[ParagraphElement.appendChild()][26]** method.
*   Add the paragraph to the document using **[ITaggedContent.getRootElement().appendChild()][27]** method.
*   Finally, save the PDF file using **[Document.save(String)][28]** method.

The following code sample shows how to add nested elements in a tagged PDF in Java.

{{< gist aspose-com-gists 191d997a5b1b0216a2b4d0546bcef9cf "create-tagged-pdf-nested-elements.java" >}}

The following screenshot shows the tagged PDF with nested elements.



{{< figure align=center src="images/Create-Tagged-PDF-Nested-Elements-1024x445.png" alt="Create a Tagged PDF with Nested Elements in Java">}}


## Styling Text Structure in a Tagged PDF {#Styling-Text-Structure-in-a-Tagged-PDF}

You can also apply styling to the text in a tagged PDF by setting font style, family, size, etc. For this, _Aspose.PDF for Java_ allows you to set **font, font size**, **font style,** and **foreground color** using [**StructureTextState**][29] class. The following code sample shows how to apply text styling in a tagged PDF in Java.

{{< gist aspose-com-gists 191d997a5b1b0216a2b4d0546bcef9cf "create-tagged-pdf-styling.java" >}}

## Illustrating Structure Elements in a Tagged PDF in Java {#Illustrating-Structure-Elements-in-a-Tagged-PDF}

To illustrate the structure elements, _Aspose.PDF for Java_ provides [**IllustrationElement**][30] class. The following code sample shows how to use this class to illustrate the structure elements in a tagged PDF.

{{< gist aspose-com-gists 191d997a5b1b0216a2b4d0546bcef9cf "create-tagged-pdf-illustrating-structure.java" >}}

## Get a Free License {#Get-a-Free-License}

You can [get a free temporary license][31] in order to use _Aspose.PDF for Java_ without evaluation limitations.

## Conclusion

In this article, you have learned how to create tagged PDF files in Java. Furthermore, you have seen how to create nested elements, apply styling to text, and illustrate structure elements in a tagged PDF programmatically. In addition, you can explore more about Java PDF API using the [documentation][32]. In case you would have any questions or queries, you can contact us via our [forum][33].

## See Also

*   [Creating PDF Files from Scratch using Java][34]




[1]: https://docs.fileformat.com/pdf/
[2]: https://blog.aspose.com/2020/12/31/create-pdf-files-in-java/
[3]: https://docs.fileformat.com/pdf/
[4]: https://blog.aspose.com/2020/12/31/create-pdf-files-in-java/
[5]: #API-to-Create-Tagged-PDF-Files
[6]: #Create-a-Tagged-PDF-File
[7]: #Create-a-Tagged-PDF-with-Nested-Elements
[8]: #Styling-Text-Structure-in-a-Tagged-PDF
[9]: #Illustrating-Structure-Elements-in-a-Tagged-PDF
[10]: https://products.aspose.com/pdf/java/
[11]: https://downloads.aspose.com/pdf/java
[12]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.tagged/ITaggedContent
[13]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[14]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.tagged/TaggedContent
[15]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.tagged/ITaggedContent
[16]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.tagged.logicalstructure.elements.bls/ParagraphElement
[17]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.tagged/ITaggedContent#createParagraphElement--
[18]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.tagged.logicalstructure.elements/Element#appendChild-com.aspose.pdf.tagged.logicalstructure.elements.Element-
[19]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[20]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[21]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.tagged/TaggedContent
[22]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.tagged/ITaggedContent
[23]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.tagged.logicalstructure.elements.bls/ParagraphElement
[24]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.tagged/ITaggedContent#createParagraphElement--
[25]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.tagged.logicalstructure.elements.ils/SpanElement
[26]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.tagged.logicalstructure.elements/Element#appendChild-com.aspose.pdf.tagged.logicalstructure.elements.Element-
[27]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.tagged.logicalstructure.elements/Element#appendChild-com.aspose.pdf.tagged.logicalstructure.elements.Element-
[28]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[29]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.tagged.logicalstructure.elements/StructureTextState
[30]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.tagged.logicalstructure.elements/IllustrationElement
[31]: https://purchase.aspose.com/temporary-license
[32]: https://docs.aspose.com/pdf/java/
[33]: https://forum.aspose.com/
[34]: https://blog.aspose.com/2020/12/31/create-pdf-files-in-java/




