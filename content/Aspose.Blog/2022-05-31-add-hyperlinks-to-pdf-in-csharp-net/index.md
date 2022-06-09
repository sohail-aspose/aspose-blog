---
title: 'Add or Update Hyperlinks in PDF using C# .NET'
seoTitle: "Add Hyperlink in PDF in C# .NET | Fetch and Update Hyperlinks in PDF"
description: "Use .NET PDF API to add hyperlinks in PDF using C#. Add a hyperlink to a webpage, page, or an external PDF file. Update hyperlink in a PDF in C#."
date: Tue, 31 May 2022 09:50:46 +0000
draft: false
url: /2022/05/31/add-hyperlinks-to-pdf-in-csharp-net/
author: Usman Aziz
summary: '[PDF][1] is a feature-rich document format that supports a range of elements including annotations, media, forms, etc. Hyperlink is an important element that is used to navigate within the PDF, from one PDF to another, to a web page, etc. While generating the PDF documents programmatically, you may often need to insert hyperlinks. Accordingly, in this article, you will learn **how to add and update hyperlinks in PDF files in C# .NET**.'
tags: ['Add Hyperlink in a PDF Csharp', 'Add Hyperlink to an External PDF Csharp', 'DotNet API to Add Hyperlinks in PDF', 'DotNet PDF Generator API', 'Insert Hyperlink to a Particular Page Csharp']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Add-Hyperlink-in-PDF.png" alt="Add or Update Hyperlinks in PDF using C# .NET">}}


[PDF][2] is a feature-rich document format that supports a range of elements including annotations, media, forms, etc. Hyperlink is an important element that is used to navigate within the PDF, from one PDF to another, to a web page, etc. While generating the PDF documents programmatically, you may often need to insert hyperlinks. Accordingly, in this article, you will learn **how to add and update hyperlinks in PDF files in C# .NET**.

*   [.NET API to Add Hyperlinks in PDF][3]
*   [Add Hyperlink in a PDF][4]
*   [Add Hyperlink to an External PDF][5]
*   [Insert Hyperlink to a Particular Page][6]
*   [Update a Hyperlink in PDF][7]

## C# .NET API to Add or Update Hyperlinks in PDF {#API-to-Add-Hyperlinks-in-PDF}

To manipulate hyperlinks in PDF files, we will use [Aspose.PDF for .NET][8]. It is a popular API that allows you to create, process, and convert PDF files from within .NET applications. You can [download][9] the API's binaries or install it using [NuGet][10].

```
PM> Install-Package Aspose.PDF
```

## Add Hyperlink in a PDF in C# {#Add-Hyperlink-in-a-PDF}

The following are the steps to add a hyperlink to a PDF file in C#.

*   Create a new PDF or load an existing one using ******[Document][11]****** class.
*   Get reference of the page where you want to add hyperlink from **[Document.Pages][12]** collection.
*   Create an object of **[LinkAnnotation][13]** class and set its properties.
*   Initialize **[LinkAnnotation.Action][14]** property to **[GoToURIAction][15]** object containing URL.
*   Add link to **[Page.Annotations][16]** collection.
*   Save PDF using ******[Document.Save(String)][17]****** method.

The following code sample shows how to add a hyperlink in PDF in C#.

{{< gist aspose-com-gists 87c1b3797fdd7b1530c4a4aeb97588e7 "add-hyperlink-in-pdf.cs" >}}

## Add Hyperlink to an External PDF in C# {#Add-Hyperlink-to-an-External-PDF}

You can also navigate to an external PDF file from one PDF using a hyperlink. The following steps demonstrate how to add a hyperlink to an external PDF file in C#.

*   Create a new PDF or load an existing one using **[Document][18]** class.
*   Get reference of the page where you want to add hyperlink from **[Document.Pages][19]** collection.
*   Create an object of **[LinkAnnotation][20]** class and set its properties.
*   Initialize **[LinkAnnotation.Action][21]** property to **[GoToRemoteAction][22]** object containing path to external PDF.
*   Add link to **[Page.Annotations][23]** collection.
*   Save document using **[Document.Save(String)][24]** method.

The following code sample shows how to add hyperlink to an external PDF in C#.

{{< gist aspose-com-gists 87c1b3797fdd7b1530c4a4aeb97588e7 "add-hyperlink-to-external-pdf.cs" >}}

## Insert Hyperlink to a Particular PDF Page {#Insert-Hyperlink-to-a-Particular-Page}

In certain cases, you have to navigate from one page to another within a PDF document. The [**LocalHyperlink**][25] class is used to navigate to the particular page in a PDF. The following are the steps to achieve this.

*   Create a new PDF or load an existing one using **[Document][26]** class.
*   Get reference of the page where you want to add hyperlink from **[Document.Pages][27]** collection.
*   Create an instance of **[TextFragment][28]** to set text of the hyperlink.
*   Create an instance of **[LocalHyperlink][29]** class and set **[**LocalHyperlink**.TargetPageNumber][30]** property to desired page number.
*   Assign **LocalHyperlink** object to **[TextFragment.Hyperlink][31]** property.
*   Add text to the page using **[Page.Paragraphs.Add(TextFragment)][32]** method.
*   Save PDF using **[Document.Save(String)][33]** method.

The following code sample shows how to add hyperlink to navigate to a particular page in PDF.

{{< gist aspose-com-gists 87c1b3797fdd7b1530c4a4aeb97588e7 "add-hyperlink-to-pdf-page.cs" >}}

## Update a Hyperlink in PDF using C# {#Update-Hyperlink-in-PDF}

You can also retrieve a hyperlink in a PDF file and update its properties. The following are the steps to perform this operation.

*   Load the PDF file using **[Document][34]** class.
*   Get reference of the page where the hyperlink is located from **[Document.Pages][35]** collection.
*   Extract the desired **[LinkAnnotation][36]** object from **[Page.Annotations][37]** collection by index.
*   Update the required properties and save PDF using **[Document.Save(String)][38]** method.

The following code sample shows how to update a hyperlink in PDF using C#.

{{< gist aspose-com-gists 87c1b3797fdd7b1530c4a4aeb97588e7 "update-hyperlink-in-pdf.cs" >}}

## Get a Free License {#Get-a-Free-License}

You can [get a free temporary license][39] in order to use Aspose.PDF for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to add different types of hyperlinks in PDF files using C#. Furthermore, you have seen how to retrieve the hyperlinks from existing PDF files and update their properties programmatically. In addition, you can explore more about .NET PDF API using the [documentation][40]. In case you would have any questions or queries, you can contact us via our [forum][41].

## See Also

*   [Add or Remove Annotations in PDF Files using C#][42]
*   [Extract Images from PDF using C#][43]
*   [Create PDF File from Images using C#][44]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: #API-to-Add-Hyperlinks-in-PDF
[4]: #Add-Hyperlink-in-a-PDF
[5]: #Add-Hyperlink-to-an-External-PDF
[6]: #Insert-Hyperlink-to-a-Particular-Page
[7]: #Update-Hyperlink-in-PDF
[8]: https://products.aspose.com/pdf/net/
[9]: https://downloads.aspose.com/pdf/net/
[10]: http://nuget.org/packages/Aspose.PDF
[11]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[12]: https://apireference.aspose.com/pdf/net/aspose.pdf/document/properties/pages
[13]: https://apireference.aspose.com/pdf/net/aspose.pdf.annotations/linkannotation
[14]: https://apireference.aspose.com/pdf/net/aspose.pdf.annotations/linkannotation/properties/action
[15]: https://apireference.aspose.com/pdf/net/aspose.pdf.annotations/gotouriaction
[16]: https://apireference.aspose.com/pdf/net/aspose.pdf/page/properties/annotations
[17]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/5
[18]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[19]: https://apireference.aspose.com/pdf/net/aspose.pdf/document/properties/pages
[20]: https://apireference.aspose.com/pdf/net/aspose.pdf.annotations/linkannotation
[21]: https://apireference.aspose.com/pdf/net/aspose.pdf.annotations/linkannotation/properties/action
[22]: https://apireference.aspose.com/pdf/net/aspose.pdf.annotations/gotoremoteaction
[23]: https://apireference.aspose.com/pdf/net/aspose.pdf/page/properties/annotations
[24]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/5
[25]: https://apireference.aspose.com/pdf/net/aspose.pdf/localhyperlink
[26]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[27]: https://apireference.aspose.com/pdf/net/aspose.pdf/document/properties/pages
[28]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textfragment
[29]: https://apireference.aspose.com/pdf/net/aspose.pdf/localhyperlink
[30]: https://apireference.aspose.com/pdf/net/aspose.pdf/localhyperlink/properties/targetpagenumber
[31]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textfragment/properties/hyperlink
[32]: https://apireference.aspose.com/pdf/net/aspose.pdf/page/properties/paragraphs
[33]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/5
[34]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[35]: https://apireference.aspose.com/pdf/net/aspose.pdf/document/properties/pages
[36]: https://apireference.aspose.com/pdf/net/aspose.pdf.annotations/linkannotation
[37]: https://apireference.aspose.com/pdf/net/aspose.pdf/page/properties/annotations
[38]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/5
[39]: https://purchase.aspose.com/temporary-license
[40]: https://docs.aspose.com/pdf/net/
[41]: https://forum.aspose.com/
[42]: https://blog.aspose.com/2021/01/04/add-or-remove-annotations-in-pdf-using-csharp/
[43]: https://blog.aspose.com/2021/06/15/extract-images-from-pdf-in-csharp/
[44]: https://blog.aspose.com/2021/04/20/create-pdf-from-images-using-csharp/




