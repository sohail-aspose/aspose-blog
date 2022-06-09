---
title: 'Rotate Text inside PDF Documents in C#'
seoTitle: "Rotate Text inside PDF in C# .NET | .NET PDF Generator API"
description: "Use .NET PDF generator API to rotate text inside PDF documents programmatically in C#. Rotate text fragments or paragraphs dynamically in a PDF file."
date: Fri, 13 May 2022 16:04:43 +0000
draft: false
url: /2022/05/13/rotate-text-inside-pdf-documents-in-csharp/
author: Usman Aziz
summary: '[PDF][1] has become a ruling document format in the digital world. Its cross-platform support has made it a widely adopted format for generating and sharing documents, such as research articles, invoices, etc. While generating a PDF programmatically, you often need to change the position and orientation of the text according to the layout of the document. In this article, we will demonstrate **how to rotate text inside PDF documents programmatically in C# .NET**.'
tags: ['Apply Rotation to Text Fragment in PDF', 'Apply Rotation to Text Paragraph in PDF', 'DotNet PDF Generator API', 'Rotate Text inside PDF in CSharp', 'dotnet pdf api']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Rotate-Text-in-PDF.jpg" alt="Rotate Text inside PDF Documents in C#">}}


[PDF][2] has become a ruling document format in the digital world. Its cross-platform support has made it a widely adopted format for generating and sharing documents, such as research articles, invoices, etc. While generating a PDF programmatically, you often need to change the position and orientation of the text according to the layout of the document. In this article, we will demonstrate **how to rotate text inside PDF documents programmatically in C# .NET**.

*   [.NET API to Rotate Text in PDF][3]
*   [Rotate Text inside PDF in C#][4]
    *   [Apply Text Rotation using TextFragment][5]
    *   [Apply Text Rotation using TextParagraph][6]

## C# .NET API to Rotate Text in PDF {#NET-API-to-Rotate-Text-in-PDF}

[Aspose.PDF for .NET][7] is a C# class library that provides basic as well as advanced PDF manipulation features for .NET applications. Using the API, you can generate PDF documents with simple or complex layouts seamlessly. We will use this API to rotate text inside PDF documents. You can either [download][8] the API’s DLL or install it using [NuGet][9].

```
PM> Install-Package Aspose.PDF
```

## Rotate Text inside PDF in C# {#Rotate-Text-inside-PDF}

There are multiple ways to rotate a text inside a PDF document. You can either rotate a text fragment or the complete paragraph. Let's see how each of these text rotations works.

### PDF Text Rotation using TextFragment in C# {#Apply-Text-Rotation-using-TextFragment}

The following are the steps to rotate a text fragment in a PDF document using C#.

*   First, create a new document using the [Document][10] class.
*   Then, add a page to the document and get its reference using [Document.Pages.Add()][11] method.
*   After that, create a new text fragment using [TextFragment][12] class.
*   Set text fragment's position and font.
*   Set rotation angle using [TextFragment.TextState.Rotation][13] property.
*   Create a new [TextBuilder][14] object and initialize it with the _Page_ object.
*   Use [TextBuilder.AppendText(TextFragment)][15] method to add text to the page.
*   Finally, save the PDF document using [Document.Save(string)][16] method.

The following code sample shows how to rotate text in a PDF document in C#.

{{< gist aspose-com-gists 64858027248d9961768e71e1aa5edcf8 "rotate-text-using-textfragment.cs" >}}

#### Output



{{< figure align=center src="images/PDF-Text-Rotation_TextFragment.png" alt="PDF Text Rotation using TextFragment in C#">}}


## PDF Text Rotation using TextParagraph in C# {#Apply-Text-Rotation-using-TextParagraph}

You can also apply rotation to the text while creating a new paragraph. This can be achieved using [TextParagraph][17] class. The following are the steps to apply text rotation using _TextParagraph_ class.

*   First, create a new document using the [Document][18] class.
*   Then, add a page to the document and get its reference using [Document.Pages.Add()][19] method.
*   After that, create a new [TextParagraph][20] object.
*   Create a new text fragment using [TextFragment][21] class and set the text and font.
*   Set rotation angle using [TextFragment.TextState.Rotation][22] property.
*   Add text to paragraph using [TextParagraph.AppendLine(TextFragment)][23] method.
*   Create a new [TextBuilder][24] object and initialize it with the _Page_ object.
*   Use [TextBuilder.AppendParagraph(TextParagraph)][25] method to add paragraph to the page.
*   Finally, save the PDF document using [Document.Save(string)][26] method.

The following code sample shows how to rotate text inside a paragraph in PDF programmatically.

{{< gist aspose-com-gists 64858027248d9961768e71e1aa5edcf8 "rotate-text-using-textparagraph.cs" >}}

#### Output



{{< figure align=center src="images/PDF-Text-Rotation_TextParagraph.png" alt="PDF Text Rotation using TextParagraph in C#">}}


## Get a Free API License {#Get-a-Free-API-License}

You can try Aspose.PDF for .NET for free by [getting a temporary license][27].

## Conclusion

PDF automation is widely adopted to create and manipulate PDF documents from within the web or desktop applications. In this article, you have learned how to rotate text in PDF programmatically using C#. We have explicitly covered how to rotate text using _TextFragment_ and _TextParagraph_ classes. Besides, you can explore other features using the [documentation][28] of Aspose.PDF for .NET. In case you would have any questions or queries, you can contact us via our [forum][29].

## See Also

*   [Create PDF Files using C# – .NET PDF API][30]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: #NET-API-to-Rotate-Text-in-PDF
[4]: #Rotate-Text-inside-PDF
[5]: #Apply-Text-Rotation-using-TextFragment
[6]: #Apply-Text-Rotation-using-TextParagraph
[7]: https://products.aspose.com/pdf/net/
[8]: https://downloads.aspose.com/pdf/net/
[9]: http://nuget.org/packages/Aspose.pdf
[10]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[11]: https://apireference.aspose.com/pdf/net/aspose.pdf/document/properties/pages
[12]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textfragment
[13]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textfragmentstate/properties/rotation
[14]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textbuilder
[15]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textbuilder/methods/appendtext
[16]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/5
[17]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textparagraph
[18]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[19]: https://apireference.aspose.com/pdf/net/aspose.pdf/document/properties/pages
[20]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textparagraph
[21]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textfragment
[22]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textfragmentstate/properties/rotation
[23]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textparagraph/methods/appendline
[24]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textbuilder
[25]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textbuilder/methods/appendparagraph
[26]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/5
[27]: https://purchase.aspose.com/temporary-license
[28]: https://docs.aspose.com/pdf/net/
[29]: https://forum.aspose.com/
[30]: https://blog.aspose.com/2020/12/02/create-pdf-files-using-csharp/




