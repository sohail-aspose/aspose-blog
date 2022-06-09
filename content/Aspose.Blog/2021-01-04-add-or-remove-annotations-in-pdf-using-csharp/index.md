---
title: 'Add or Remove Annotations in PDF Files using C#'
seoTitle: "Add or Remove Annotations in PDF using C# | .NET PDF API"
description: "Use .NET PDF API to add or remove annotations in PDF documents using C# or VB.NET. Add line, text, watermark, circles, popup and multimedia annotations."
date: Mon, 04 Jan 2021 11:53:00 +0000
draft: false
url: /2021/01/04/add-or-remove-annotations-in-pdf-using-csharp/
author: Usman Aziz
summary: 'PDF annotations are the additional objects that are used to marking up the content in PDFs. Since PDF files are not easily editable, the annotations are used to add notes about the content using comments, popups, and various other graphical objects. In this article, you will learn how to work with annotations in PDF documents programmatically. Particularly, the article will cover **how to add and remove annotations in PDF files using C#**.'
tags: ['add annotations from pdf csharp', 'remove annotations from pdf csharp']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Add-or-Remove-Annotation-in-PDF-2.jpg" alt="Add or Remove Annotation in PDF">}}


PDF annotations are the additional objects used to mark up the content in PDFs. Since [PDF][1] files are not easily editable, the annotations are used to add notes about the content. The PDF annotations include comments, popups, and various other graphical objects. In this article, you will learn how to work with PDF annotations programmatically. Particularly, we will cover **how to add and remove annotations in PDF files using [C#][2]**.

*   [C# API to Work with PDF Annotations][3]
*   [Add Annotations to PDF using C#][4]
*   [Remove Annotations from PDF in C#][5]

## C# API to Add PDF Annotations - Free Download {#CSharp-API-to-Work-with-PDF-Annotations}

In order to work with PDF documents from within your .NET applications, Aspose provides [Aspose.PDF for .NET][6]. Using the API, you can create new as well as manipulate existing PDF files seamlessly. Furthermore, the API also allows you to add and remove PDF annotations. You can either [download][7] the API or install it within your .NET applications using [NuGet][8].

```
PM> Install-Package Aspose.Pdf
```

## Add Annotations to PDF using C# {#Add-Annotations-to-PDF-using-CSharp}

PDF format supports various types of annotations such as text, line, circle, square, redaction and etc. In order to work with each PDF annotation, Aspose.PDF for .NET provides separate classes. For example, [LineAnnotation][9] class is used for adding a line whereas [HighlightAnnotation][10] class is used to add a highlight annotation. Let's have a look at the steps of adding any type of annotation to a PDF.

### Steps to Add Annotation in PDF using C#

*   Load the PDF file using [Document][11] class.
*   Create the instance of the desired annotation class i.e. [HighlightAnnotation][12] or [LineAnnotation][13].
*   Set the properties of the annotation such as position, color, size and etc.
*   Add annotation to the [Annotations][14] collection of the particular PDF page using [Document.Pages\[1\].Annotations.Add(Annotation)][15] method.
*   Save the PDF document using [Document.Save(String)][16] method.

For demonstration, the following code sample shows how to add a line annotation to the PDF using C#.

{{< gist aspose-com-gists 796daba61df7d5752a0e55f1bfc513ee "add-annotation.cs" >}}

For the code samples of other annotation types, you can visit the following documentation articles:

*   [Free text Annotation][17]
*   [Link Annotation][18]
*   [Line Annotation][19]
*   [Square and Circle Annotations][20]
*   [Polygon and Polyline Annotations][21]
*   [Text Markup Annotation][22]
*   [Widget Annotation][23]
*   [Caret Annotation][24]
*   [Ink Annotation][25]
*   [Popup Annotation][26]
*   [Multimedia Annotation][27]
*   [Watermark Annotation][28]

## Remove Annotations from PDF in C# {#Remove-Annotations-from-PDF-in-CSharp}

You can also remove the PDF annotations from existing PDF documents using Aspose.PDF for .NET. You can either remove all or a particular annotation from a PDF. The following are the steps to remove PDF annotations.

*   Load the PDF file using [Document][29] class.
*   Delete all annotations from a particular page using [Document.Pages\[index\].Annotations.Delete()][30] method.
*   Or delete a particular annotation using [Document.Pages\[index\].Annotations.Delete(Int index)][31] or [Document.Pages\[index\].Annotations.Delete(Annotation)][32] methods.
*   Save the document using [Document.Save(String)][33] method.

The following code sample shows how to remove annotations from a PDF file using C#.

{{< gist aspose-com-gists 796daba61df7d5752a0e55f1bfc513ee "remove-annotation.cs" >}}

## Conclusion

PDF annotations are used to annotate the documents in order to insert text, graphics, and multimedia objects. Furthermore, the annotations help you add additional information or explanation about the content. In accordance with that, this article covered how to add and remove annotations from PDF using C#. In case you want to explore more about working with PDF annotations, visit [documentation][34].

## See Also

*   [Create PDF Files using C# – .NET PDF API][35]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/programming/cs/
[3]: #CSharp-API-to-Work-with-PDF-Annotations
[4]: #Add-Annotations-to-PDF-using-CSharp
[5]: #Remove-Annotations-from-PDF-in-CSharp
[6]: https://products.aspose.com/pdf/net
[7]: https://downloads.aspose.com/pdf/net
[8]: http://nuget.org/packages/Aspose.PDF
[9]: https://apireference.aspose.com/pdf/net/aspose.pdf.annotations/lineannotation/methods/index
[10]: https://apireference.aspose.com/pdf/net/aspose.pdf.annotations/highlightannotation
[11]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[12]: https://apireference.aspose.com/pdf/net/aspose.pdf.annotations/highlightannotation
[13]: https://apireference.aspose.com/pdf/net/aspose.pdf.annotations/lineannotation/methods/index
[14]: https://apireference.aspose.com/pdf/net/aspose.pdf/page/properties/annotations
[15]: https://apireference.aspose.com/pdf/net/aspose.pdf.annotations/annotationcollection/methods/add
[16]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/4
[17]: https://docs.aspose.com/pdf/net/add-free-text-annotation/
[18]: https://docs.aspose.com/pdf/net/add-link-annotation/
[19]: https://docs.aspose.com/pdf/net/add-line-annotation/
[20]: https://docs.aspose.com/pdf/net/add-square-and-circle-annotations/
[21]: https://docs.aspose.com/pdf/net/add-polygon-and-polyline-annotations/
[22]: https://docs.aspose.com/pdf/net/add-text-markup-annotation/
[23]: https://docs.aspose.com/pdf/net/add-widget-annotation/
[24]: https://docs.aspose.com/pdf/net/add-caret-annotation/
[25]: https://docs.aspose.com/pdf/net/ink-annotation/
[26]: https://docs.aspose.com/pdf/net/add-popup-annotation/
[27]: https://docs.aspose.com/pdf/net/add-multimedia-annotation/
[28]: https://docs.aspose.com/pdf/net/add-watermarkannotation/
[29]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[30]: https://apireference.aspose.com/pdf/net/aspose.pdf.annotations/annotationcollection/methods/delete
[31]: https://apireference.aspose.com/pdf/net/aspose.pdf.annotations.annotationcollection/delete/methods/2
[32]: https://apireference.aspose.com/pdf/net/aspose.pdf.annotations.annotationcollection/delete/methods/1
[33]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/4
[34]: https://docs.aspose.com/pdf/net/annotations/
[35]: https://blog.aspose.com/2020/12/02/create-pdf-files-using-csharp/





