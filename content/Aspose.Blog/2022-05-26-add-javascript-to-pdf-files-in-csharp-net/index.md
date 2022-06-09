---
title: 'Add or Remove JavaScript in PDF Files in C# .NET'
seoTitle: "Add JavaScript to PDF in C# .NET | .NET PDF Generator Library"
description: "Use .NET PDF API to add JavaScript to PDF files in C#. Add page level or document level JavaScript in PDF. Remove JavaScript from PDF programmatically."
date: Thu, 26 May 2022 06:30:39 +0000
draft: false
url: /2022/05/26/add-javascript-to-pdf-files-in-csharp-net/
author: Usman Aziz
summary: '[PDF][1] is a rich document format in terms of versatility and features. One of the major advantages of PDF is its consistent layout across heterogeneous platforms. Moreover, it has the ability to be displayed in desktop applications and web browsers at the same time. This is the reason that PDF files are capable of running JavaScript. In this article, we will demonstrate **how to add or remove JavaScript in PDF files using C#**.'
tags: ['Add Document Level JavaScript in PDF Csharp', 'Add JavaScript to PDF Files Csharp', 'DotNet API to Work with JavaScript in PDF', 'DotNet PDF Generator API', 'Remove JavaScript from PDF in Csharp']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Add-JavaScript-to-PDF.png" alt="Add JavaScript to PDF Files in C# .NET">}}


[PDF][2] is a rich document format in terms of versatility and features. One of the major advantages of PDF is its consistent layout across heterogeneous platforms. Moreover, it has the ability to be displayed in desktop applications and web browsers at the same time. This is the reason that PDF files are capable of running JavaScript. In this article, we will demonstrate **how to add or remove JavaScript in PDF files using C#**.

*   [.NET API to Add or Remove JavaScript in PDF][3]
*   [Add JavaScript to PDF Files][4]
*   [Add Document Level JavaScript in PDF][5]
*   [Remove JavaScript from PDF][6]

## C# .NET API to Add or Remove JavaScript in PDF {#API-to-Work-with-JavaScript-in-PDF}

[Aspose.PDF for .NET][7] is designed to perform PDF generation and manipulation within the .NET applications. The API lets you seamlessly create, process, and convert PDF files of simple and complex layouts. You can [download][8] the API's binaries or install it using [NuGet][9].

```
PM> Install-Package Aspose.PDF
```

## Add JavaScript to PDF Files in C# {#Add-JavaScript-to-PDF-Files}

PDF files support Acrobat JavaScript, which is based on the core of JavaScript version 1.5 of ISO-16262, formerly known as ECMAScript. It is an object-oriented scripting language developed by Netscape Communications. Before proceeding to add JavaScript to PDF files, let's have a look at the differences between Acrobat JavaScript and HTML JavaScript which is used in web browsers.

*   Acrobat JavaScript does not have access to objects within an HTML page. Similarly, HTML JavaScript cannot access objects within a PDF file.
*   HTML JavaScript is able to manipulate objects such as Window. However, Acrobat JavaScript cannot access these particular objects but it can manipulate PDF-specific objects.

The following are the steps to add JavaScript to a PDF file in C#.

*   Load the PDF file using ****[Document][10]**** class.
*   Create an instance of **[JavascriptAction][11]** class and initialize it with the desired script.
*   Assign **JavascriptAction** object to **[Document.OpenAction][12]** property for document level JavaScript.
*   To add page level JavaScript, use **[Document.Pages\[index\].Actions][13]** property.
*   Save PDF using ****[Document.Save(String)][14]**** method.

The following code sample shows how to add JavaScript to a PDF.

{{< gist aspose-com-gists 5b20d81a544834f70783ec6c84ef91cb "add-javascript-to-pdf.cs" >}}

## Add Document Level JavaScript in a PDF in C# {#Add-Document-Level-JavaScript-in-PDF}

You can also add JavaScript to the document level using [**Document.JavaScript**][15] property. The following are the steps to add JavaScript to the document level in C#.

*   Load the PDF file using **[Document][16]** class.
*   Use [**Document.JavaScript**][17] collection to add JavaScript functions.
*   Save PDF using **[Document.Save(String)][18]** method.

The following code sample shows how to add JavaScript to a PDF in C#.

{{< gist aspose-com-gists 5b20d81a544834f70783ec6c84ef91cb "add-document-level-javascript-to-pdf.cs" >}}

## Remove JavaScript from a PDF in C# {#Remove-JavaScript-from-PDF}

The following are the steps to remove JavaScript from a PDF in C#.

*   Load the PDF file using **[Document][19]** class.
*   Remove desired JavaScript module using [**Document.JavaScript.Remove(String)**][20] method.
*   Save PDF using **[Document.Save(String)][21]** method.

The following code sample shows how to remove JavaScript from a PDF in C#.

{{< gist aspose-com-gists 5b20d81a544834f70783ec6c84ef91cb "remove-javascript-from-pdf.cs" >}}

## Get a Free License {#Get-a-Free-License}

You can [get a free temporary license][22] in order to use Aspose.PDF for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to add JavaScript to PDF files in C#. Furthermore, you have seen how to remove JavaScript from a PDF programmatically. Besides, you can explore more about .NET PDF API using the [documentation][23]. In case you would have any questions or queries, you can contact us via our [forum][24].

## See Also

*   [Add or Remove Annotations in PDF Files using C#][25]
*   [Extract Images from PDF using C#][26]
*   [Create PDF File from Images using C#][27]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: #API-to-Work-with-JavaScript-in-PDF
[4]: #Add-JavaScript-to-PDF-Files
[5]: #Add-Document-Level-JavaScript-in-PDF
[6]: #Remove-JavaScript-from-PDF
[7]: https://products.aspose.com/pdf/net/
[8]: https://downloads.aspose.com/pdf/net/
[9]: http://nuget.org/packages/Aspose.PDF
[10]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[11]: https://apireference.aspose.com/pdf/net/aspose.pdf.annotations/javascriptaction
[12]: https://apireference.aspose.com/pdf/net/aspose.pdf/document/properties/openaction
[13]: https://apireference.aspose.com/pdf/net/aspose.pdf/page/properties/actions
[14]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/5
[15]: https://apireference.aspose.com/pdf/net/aspose.pdf/document/properties/javascript
[16]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[17]: https://apireference.aspose.com/pdf/net/aspose.pdf/document/properties/javascript
[18]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/5
[19]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[20]: https://apireference.aspose.com/pdf/net/aspose.pdf/javascriptcollection/methods/remove
[21]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/5
[22]: https://purchase.aspose.com/temporary-license
[23]: https://docs.aspose.com/pdf/net/
[24]: https://forum.aspose.com/
[25]: https://blog.aspose.com/2021/01/04/add-or-remove-annotations-in-pdf-using-csharp/
[26]: https://blog.aspose.com/2021/06/15/extract-images-from-pdf-in-csharp/
[27]: https://blog.aspose.com/2021/04/20/create-pdf-from-images-using-csharp/




