---
title: 'Create Tagged PDF Files in C# .NET'
seoTitle: "Create Tagged PDF Files in C# .NET | .NET PDF Generator Library"
description: "Use .NET PDF Generator library to create tagged PDF files in C#. Create nested elements, apply styling, and illustrate structure elements in tagged PDF."
date: Fri, 20 May 2022 23:06:00 +0000
draft: false
url: /2022/05/20/create-tagged-pdf-files-in-csharp-net/
author: Usman Aziz
summary: 'A tagged PDF file is a type of PDF that uses tags to define the logical structure of the content in the document. It is used to enhance the reading experience for those who use assistive technologies and screen readers. In a [previous post][1], we covered creating PDF files within a .NET application. In this article, we will demonstrate **how to create tagged PDF files programmatically in C# .NET**.'
tags: ['Create a Tagged PDF File in CSharp', 'Create a Tagged PDF with Nested Elements Csharp', 'DotNet API to Create Tagged PDF Files', 'DotNet PDF Generator API']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Create-Tagged-PDF-File.png" alt="Create Tagged PDF Files in C# .NET">}}


A tagged [PDF][2] file is a type of PDF that uses tags to define the logical structure of the content in the document. It is used to enhance the reading experience for those who use assistive technologies and screen readers. In a [previous post][3], we covered creating PDF files within a .NET application. In this article, we will demonstrate **how to create tagged PDF files programmatically in C# .NET**.

*   [.NET API to Create Tagged PDF Files][4]
*   [Create a Tagged PDF File][5]
*   [Create a Tagged PDF with Nested Elements][6]
*   [Styling Text Structure in a Tagged PDF][7]
*   [Illustrating Structure Elements in a Tagged PDF][8]

## C# .NET API to Create Tagged PDF Files {#API-to-Create-Tagged-PDF-Files}

[Aspose.PDF for .NET][9] is a robust API for PDF generation and manipulation within the .NET applications. Using the API, you can seamlessly create, process, and convert PDF files of simple and complex layouts. You can [download][10] the API's binaries or install it using [NuGet][11].

```
PM> Install-Package Aspose.PDF
```

## Create a Tagged PDF File in C# {#Create-a-Tagged-PDF-File}

To create structure elements in a tagged PDF, _Aspose.PDF for .NET_ provides the ****[ITaggedContent][12]**** interface. So let's see how to use this interface to create a tagged PDF file in C#.

*   Create a new PDF or load an existing one using the ******[Document][13]****** class.
*   Get the reference of the **[TaggedContent][14]** of the document into an **[ITaggedContent][15]** object.
*   Set title, header, and language and add elements to the PDF using the **ITaggedContent** object.
*   Create a new ****[ParagraphElement][16]**** using [**ITaggedContent.CreateParagraphElement()**][17] method and set its text.
*   Add the paragraph to the document using **[ITaggedContent.RootElement.AppendChild()][18]** method.
*   Finally, save the PDF file using ******[Document.Save(String)][19]****** method.

The following code sample shows how to create a tagged PDF in C#.

{{< gist aspose-com-gists 4c91dc6aea2cfa5a0971de4fe5de1429 "create-tagged-pdf.cs" >}}

The following is the output of the above code sample.



{{< figure align=center src="images/Create-Tagged-PDF-1024x477.png" alt="Create a Tagged PDF File in C#">}}


## Create a Tagged PDF with Nested Elements in C# {#Create-a-Tagged-PDF-with-Nested-Elements}

In the previous example, we created a simple tagged PDF that contains a paragraph. Let's now have a look at how to add nested elements in a tagged PDF. The following are the steps to perform this operation.

*   Create a new PDF or load an existing one using the **[Document][20]** class.
*   Get the reference of the **[TaggedContent][21]** of the document into an **[ITaggedContent][22]** object.
*   Set title, header, and language and add elements to the PDF using the **ITaggedContent** object.
*   Create a new **[ParagraphElement][23]** using [**ITaggedContent.CreateParagraphElement()**][24] method and set its text.
*   Use **[SpanElement][25]** class to add the nested elements.
*   Add nested element to paragraph using **[ParagraphElement.AppendChild()][26]** method.
*   Add the paragraph to the document using **[ITaggedContent.RootElement.AppendChild()][27]** method.
*   Finally, save the PDF file using **[Document.Save(String)][28]** method.

The following code sample shows how to add nested elements in a tagged PDF in C#.

{{< gist aspose-com-gists 4c91dc6aea2cfa5a0971de4fe5de1429 "create-tagged-pdf-nested-elements.cs" >}}

The following screenshot shows the tagged PDF with nested elements.



{{< figure align=center src="images/Create-Tagged-PDF-Nested-Elements-1024x445.png" alt="Create a Tagged PDF with Nested Elements in C#">}}


## Styling Text Structure in a Tagged PDF {#Styling-Text-Structure-in-a-Tagged-PDF}

You can also apply styling to the text in a tagged PDF by setting font style, family, size, etc. For this, _Aspose.PDF for .NET_ provides [**Font**][29], [**FontSize**][30], [**FontStyle**][31] and [**ForegroundColor**][32] properties of [**StructureTextState**][33] class. The following code sample shows how to apply text styling in a tagged PDF in C#.

{{< gist aspose-com-gists 4c91dc6aea2cfa5a0971de4fe5de1429 "create-tagged-pdf-styling.cs" >}}

## Illustrating Structure Elements in a Tagged PDF in C# {#Illustrating-Structure-Elements-in-a-Tagged-PDF}

To illustrate the structure elements, _Aspose.PDF for .NET_ provides **[IllustrationElement][34]** class. The following code sample shows how to use this class to illustrate the structure elements in a tagged PDF.

{{< gist aspose-com-gists 4c91dc6aea2cfa5a0971de4fe5de1429 "create-tagged-pdf-illustrating-structure.cs" >}}

## Get a Free License {#Get-a-Free-License}

You can [get a free temporary license][35] in order to use Aspose.PDF for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to create tagged PDF files in C#. Furthermore, you have seen how to create nested elements, apply styling to text, and illustrate structure elements in a tagged PDF programmatically. Besides, you can explore more about .NET PDF API using the [documentation][36]. In case you would have any questions or queries, you can contact us via our [forum][37].

## See Also

*   [Add or Remove Annotations in PDF Files using C#][38]
*   [Extract Images from PDF using C#][39]
*   [Create PDF File from Images using C#][40]




[1]: https://blog.aspose.com/2020/12/02/create-pdf-files-using-csharp/
[2]: https://docs.fileformat.com/pdf/
[3]: https://blog.aspose.com/2020/12/02/create-pdf-files-using-csharp/
[4]: #API-to-Create-Tagged-PDF-Files
[5]: #Create-a-Tagged-PDF-File
[6]: #Create-a-Tagged-PDF-with-Nested-Elements
[7]: #Styling-Text-Structure-in-a-Tagged-PDF
[8]: #Illustrating-Structure-Elements-in-a-Tagged-PDF
[9]: https://products.aspose.com/pdf/net/
[10]: https://downloads.aspose.com/pdf/net/
[11]: http://nuget.org/packages/Aspose.PDF
[12]: https://apireference.aspose.com/pdf/net/aspose.pdf.tagged/itaggedcontent
[13]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[14]: https://apireference.aspose.com/pdf/net/aspose.pdf/document/properties/taggedcontent
[15]: https://apireference.aspose.com/pdf/net/aspose.pdf.tagged/itaggedcontent
[16]: https://apireference.aspose.com/pdf/net/aspose.pdf.logicalstructure/paragraphelement
[17]: https://apireference.aspose.com/pdf/net/aspose.pdf.tagged/itaggedcontent/methods/createparagraphelement
[18]: https://apireference.aspose.com/pdf/net/aspose.pdf.logicalstructure/element/methods/appendchild
[19]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/5
[20]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[21]: https://apireference.aspose.com/pdf/net/aspose.pdf/document/properties/taggedcontent
[22]: https://apireference.aspose.com/pdf/net/aspose.pdf.tagged/itaggedcontent
[23]: https://apireference.aspose.com/pdf/net/aspose.pdf.logicalstructure/paragraphelement
[24]: https://apireference.aspose.com/pdf/net/aspose.pdf.tagged/itaggedcontent/methods/createparagraphelement
[25]: https://apireference.aspose.com/pdf/net/aspose.pdf.logicalstructure/spanelement
[26]: https://apireference.aspose.com/pdf/net/aspose.pdf.logicalstructure/element/methods/appendchild
[27]: https://apireference.aspose.com/pdf/net/aspose.pdf.logicalstructure/element/methods/appendchild
[28]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/5
[29]: https://apireference.aspose.com/pdf/net/aspose.pdf.logicalstructure/structuretextstate/properties/font
[30]: https://apireference.aspose.com/pdf/net/aspose.pdf.logicalstructure/structuretextstate/properties/fontsize
[31]: https://apireference.aspose.com/pdf/net/aspose.pdf.logicalstructure/structuretextstate/properties/fontstyle
[32]: https://apireference.aspose.com/pdf/net/aspose.pdf.logicalstructure/structuretextstate/properties/foregroundcolor
[33]: https://apireference.aspose.com/pdf/net/aspose.pdf.logicalstructure/structuretextstate
[34]: https://apireference.aspose.com/pdf/net/aspose.pdf.logicalstructure/illustrationelement
[35]: https://purchase.aspose.com/temporary-license
[36]: https://docs.aspose.com/pdf/net/
[37]: https://forum.aspose.com/
[38]: https://blog.aspose.com/2021/01/04/add-or-remove-annotations-in-pdf-using-csharp/
[39]: https://blog.aspose.com/2021/06/15/extract-images-from-pdf-in-csharp/
[40]: https://blog.aspose.com/2021/04/20/create-pdf-from-images-using-csharp/




