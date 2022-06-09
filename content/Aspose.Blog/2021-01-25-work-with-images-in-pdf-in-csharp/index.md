---
title: 'Add, Remove, Extract and Replace Images in PDF using C#'
seoTitle: "C# Add, Remove, Extract Images in PDF | .NET PDF API"
description: "Use C# PDF API to work with images in PDF files using C#. Add, extract, remove and replace images in PDF files programmatically using C#."
date: Mon, 25 Jan 2021 17:32:46 +0000
draft: false
url: /2021/01/25/work-with-images-in-pdf-in-csharp/
author: Usman Aziz
summary: 'A picture is worth a thousand words. Therefore, images and graphics play an important role in PDF as well as other documents. Since PDF has become one of the most popular and widely used file formats, this article targets how to manipulate images in PDF files programmatically. More precisely, you will learn **how to add, extract, remove, and replace images from PDF files using C#**.'
tags: ['Add-an-Image-in-a-PDF-using-Csharp', 'Csharp-API-to-Work-with-Images-in-PDF', 'Extract-Images-from-a-PDF-using-Csharp', 'Remove-Images-from-a-PDF-using-Csharp', 'Replace-an-Image-in-a-PDF-using-Csharp']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Work-with-Images-in-PDF.png.jpg" alt="Work with images in PDF C#">}}


A picture is worth a thousand words. Therefore, images and graphics play an important role in [PDF][1] as well as other documents. Since PDF has become one of the most popular and widely used file formats, this article targets how to manipulate images in PDF files programmatically. More precisely, you will learn **how to add, extract, remove, and replace images from PDF files using [C#][2]**.

*   [C# API to Work with Images in PDF][3]
*   [Add an Image in a PDF using C#][4]
*   [Extract Images from a PDF using C#][5]
*   [Remove Images from a PDF using C#][6]
*   [Replace an Image in a PDF using C#][7]
*   [Get a Free License][8]

## C# API to Add, Remove, and Extract Images in PDF {#CSharp-API-to-Work-with-Images-in-PDF}

[Aspose.PDF for .NET][9] is a C# class library that lets you create and manipulate PDF documents from within the .NET applications. Using the API, you can perform basic as well as advanced PDF automation features quite easily. In addition, you can manipulate images in existing PDF files. The API can be downloaded as [DLL][10] or installed via [NuGet][11].

```
PM> Install-Package Aspose.Pdf
```

## Add Image in a PDF File using C# {#Add-Image-in-a-PDF-using-CSharp}

The following are the steps to add an image to a PDF file using Aspose.PDF for .NET.

*   Use [Document][12] class to create a new or load an existing PDF file.
*   Get the reference of the desired page in [Page][13] object.
*   Add the image to [Resources][14] collection of the page.
*   Use the following operators to place the image on the page:
    *   [GSave][15] operator to save the current graphical state.
    *   [ConcatenateMatrix][16] operator to specify where the image is to be placed.
    *   [Do][17] operator to draw the image on the page.
    *   [GRestore][18] operator to save the updated graphical state.
*   Save the updated PDF file using [Document.Save(String)][19] method.

The following code sample shows how to add image to a PDF file using C#.

{{< gist aspose-com-gists 73276ad00873beae0d7abe8c587405de "add-image-pdf.cs" >}}

## Extract Images from PDF using C# {#Extract-Images-from-PDF-using-CSharp}

In case you want to extract all the images from a PDF file, you can do it by following the below steps.

*   Use [Document][20] class to load an existing PDF file.
*   Get the desired image in the [XImage][21] object from a particular page's [Resources][22] collection using the index.
*   Save the extracted image in the desired format using [XImage.Save(FileStream, ImageFormat)][23] method.

The following code sample shows how to extract images from PDF using C#.

{{< gist aspose-com-gists 73276ad00873beae0d7abe8c587405de "extract-image-pdf.cs" >}}

## Remove Images from PDF using C# {#Remove-Images-from-PDF-using-CSharp}

Once you have got access to the resources of a page in PDF, you can remove the images from it. The following are the steps to remove images from a PDF file using C#.

*   Load the PDF file using [Document][24] class.
*   Remove image(s) using one of the following methods.
    *   [Delete()][25] - Delete all images.
    *   [Delete(Int32)][26] - Delete image by index.
    *   [Delete(String)][27] - Delete image by name.
*   Save the updated PDF file using [Document.Save(String)][28] method.

The following code sample shows how to remove images from a PDF using C#.

{{< gist aspose-com-gists 73276ad00873beae0d7abe8c587405de "remove-image-pdf.cs" >}}

## Replace Image in PDF using C# {#Replace-Image-in-PDF-using-CSharp}

Aspose.PDF for .NET also lets you replace a particular image in the PDF. For this, you can replace the image in the image collection of the page. The following are the steps to replace an image in PDF using C#.

*   Load the PDF file using [Document][29] class.
*   Replace the desired image using [Document.Pages\[1\].Resources.Images.Replace(Int32, Stream, Int32, Boolean)][30] method.
*   Save the updated PDF file using [Document.Save(String)][31] method.

The following code sample shows how to replace an image in PDF using C#.

{{< gist aspose-com-gists 73276ad00873beae0d7abe8c587405de "replace-image-pdf.cs" >}}

## Get a Free License {#Get-a-Free-License}

You can [get a free temporary license][32] in order to try the API without evaluation limitations.

## Conclusion

Images and graphical objects are important elements of PDF documents. Therefore, in this article, we have covered how to manipulate images in a PDF. The step-by-step tutorial and code samples have shown how to add, extract, remove and replace images in PDF files using C#. You can explore more about the C# PDF API using the [documentation][33].

## See Also

*   [Add or Remove Annotations in PDF Files using C#][34]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/programming/cs/
[3]: #CSharp-API-to-Work-with-Images-in-PDF
[4]: #Add-Image-in-a-PDF-using-CSharp
[5]: #Extract-Images-from-PDF-using-CSharp
[6]: #Remove-Images-from-PDF-using-CSharp
[7]: #Replace-Image-in-PDF-using-CSharp
[8]: #Get-a-Free-License
[9]: https://products.aspose.com/pdf/net
[10]: https://products.aspose.com/pdf/net
[11]: http://nuget.org/packages/Aspose.PDF
[12]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[13]: https://apireference.aspose.com/pdf/net/aspose.pdf/page
[14]: https://apireference.aspose.com/pdf/net/aspose.pdf/page/properties/resources
[15]: https://apireference.aspose.com/pdf/net/aspose.pdf.operators/gsave
[16]: https://apireference.aspose.com/pdf/net/aspose.pdf.operators/concatenatematrix
[17]: https://apireference.aspose.com/pdf/net/aspose.pdf.operators/do
[18]: https://apireference.aspose.com/pdf/net/aspose.pdf.operators/grestore
[19]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/4
[20]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[21]: https://apireference.aspose.com/pdf/net/aspose.pdf/ximage
[22]: https://apireference.aspose.com/pdf/net/aspose.pdf/page/properties/resources
[23]: https://apireference.aspose.com/pdf/net/aspose.pdf.ximage/save/methods/1
[24]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[25]: https://apireference.aspose.com/pdf/net/aspose.pdf/ximagecollection/methods/delete
[26]: https://apireference.aspose.com/pdf/net/aspose.pdf.ximagecollection/delete/methods/1
[27]: https://apireference.aspose.com/pdf/net/aspose.pdf.ximagecollection/delete/methods/3
[28]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/4
[29]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[30]: https://apireference.aspose.com/pdf/net/aspose.pdf.ximagecollection/replace/methods/2
[31]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/4
[32]: https://purchase.aspose.com/temporary-license
[33]: https://docs.aspose.com/pdf/net/overview/
[34]: https://blog.aspose.com/2021/01/04/add-or-remove-annotations-in-pdf-using-csharp/





