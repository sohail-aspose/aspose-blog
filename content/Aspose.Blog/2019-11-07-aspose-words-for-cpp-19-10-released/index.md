---
title: 'Convert Word Document to Multipage TIFF Image using C++'
date: Thu, 07 Nov 2019 12:51:11 +0000
draft: false
url: /2019/11/07/aspose-words-for-cpp-19-10-released/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Today, I will highlight the major features introduced in the [Aspose.Words for C++ 19.10][1] release:

## Save Word Document as MutiPage TIFF

One of the useful things you may need to do with your Word document (such as DOCX, DOC, RTF and many more) is a conversion to image file(s). For example if you have to present your Word document in a readable and printable but not editable format (e.g. for publication on the Web). One of the simple approaches you could use is a conversion to a multipage TIFF file. Please refer to the following article to learn how to convert a Word document to TIFF format by using Aspose.Words for C++:  
[Convert Word Document to Multipage TIFF Image][2]

{{< gist aspose-words 9a306a41bb6aea8adfcabf5a575c5718 "Examples-CSharp-Rendering-Printing-SaveAsMultipageTiff-SaveAsTIFF.cs" >}}

## Convert an Image to PDF using C++

It is now possible to create a PDF document from an Image by using Aspose.Words for C++ API. The code example mentioned in the following article shows how easy it is to do with Aspose.Words for C++. The code allows converting single-frame images, such as JPEG, PNG, BMP, EMF or WMF, as well as multi-frame TIFF images and GIF to PDF.  
[Convert an Image to PDF][3]

## Control Threshold for TIFF Binarization using C++

The process of reducing the information contained within the grayscale image from 256 shades of grey to 2 which are black and white and converting it to the binary image is binarization. When a document is converted to TIFF file format, you can control the threshold for TIFF binarization by using the ImageSaveOptions.ThresholdForFloydSteinbergDithering property. The default value of this property is 128. The higher the value, the darker the image. The following code example shows how to use this property to [Control Threshold for TIFF Binarization][4].

{{< gist aspose-com-gists 518f03cac02abb105e02f55edb7de9f9 "cpp-Rendering-Printing-ImageColorFilters-ExposeThresholdControlForTiffBinarization.cpp" >}}

## Save Image to One Bit per Pixel using C++

The following code example demonstrates how to save the image to one bit per pixel by setting PixelFormat to Format1bppIndexed.

{{< gist aspose-com-gists 518f03cac02abb105e02f55edb7de9f9 "cpp-Rendering-Printing-ImageColorFilters-SaveImageToOnebitPerPixel.cpp" >}}

## Encrypt DOC or DOT Files With Password using C++

The DocSaveOptions class is used to specify additional options when saving a document into the DOC or DOT format. Using this class, you can set the password to an encrypted document and ignore RoutingSlip data while saving the document. The code example given below shows how to [set the password to encrypt the document using RC4 encryption method][5].

{{< gist aspose-com-gists 518f03cac02abb105e02f55edb7de9f9 "cpp-Loading-and-Saving-WorkingWithDoc-EncryptDocumentWithPassword.cpp" >}}

## Encrypt DOCX Files With Password using C++

The OoXMLSaveOptions class provides an opportunity to save any document encrypted with the password. Using this class, you can set the password by using OoxmlSaveOptions.Password property while saving the document. The following code example demonstrates how to [set the password and save the document to DOCX format][6].  

{{< gist aspose-com-gists 518f03cac02abb105e02f55edb7de9f9 "cpp-Loading-and-Saving-WorkingWithOoxml-EncryptDocxWithPassword.cpp" >}}

## Extract Content by using DocumentVisitor

You can now use the DocumentVisitor class to implement this usage scenario. This class corresponds to the well-known Visitor design pattern. With DocumentVisitor, you can define and execute custom operations that require enumeration over the document tree. For more details, please check:  
[How to Extract Content using DocumentVisitor][7]

## Get Font Line Spacing

The line spacing of a font is the vertical distance between the baselines of two consecutive lines of text. Thus, the line spacing includes the blank space between lines along with the height of the character itself. The LineSpacing property was introduced in the Font class to [Obtain the Value of Font's Line Spacing][8] as shown in the example given below:

{{< gist aspose-com-gists 518f03cac02abb105e02f55edb7de9f9 "cpp-Programming-Documents-Document-GetFontLineSpacing-GetFontLineSpacing.cpp" >}}

## See Also Useful Links

The resources, you may need to accomplish your tasks:

*   [Aspose.Words for C++ Online Documentation][9] - up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Words for C++ Product Page][10]
*   [Install Aspose.Words for C++ NuGet Package][11]
*   [Aspose.Words for C++ API Reference Guide][12] - detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Download Examples at GitHub Repository][13] - we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

Keeping the Aspose tradition, you are welcome to shape the upcoming releases of Aspose.Words for C++ API by posting your suggestions and concerns in the [Aspose.Words for C++ support forum][14].




[1]: https://downloads.aspose.com/words/cpp/new-releases/aspose.words-for-c---19.10/
[2]: https://docs.aspose.com/words/cpp/saving-a-document-as-a-multipage-tiff/
[3]: https://docs.aspose.com/words/cpp/converting-a-document/#ConvertingaDocument-ConvertanImagetoPDF
[4]: https://docs.aspose.com/words/cpp/rendering/#Rendering-ControlThresholdforTIFFBinarization
[5]: https://docs.aspose.com/words/cpp/working-with-saveoptions/#encrypt-document-with-password
[6]: https://docs.aspose.com/words/cpp/working-with-ooxml/#encrypt-document-with-password
[7]: https://docs.aspose.com/words/cpp/how-to-extract-selected-content-between-nodes-in-a-document/#how-to-extract-content-using-documentvisitor
[8]: https://docs.aspose.com/words/cpp/working-with-document/#get-font-line-spacing
[9]: https://docs.aspose.com/words/cpp/
[10]: https://products.aspose.com/words/cpp
[11]: https://www.nuget.org/packages/Aspose.Words.Cpp/
[12]: https://apireference.aspose.com/cpp/words
[13]: https://github.com/aspose-words/Aspose.words-for-C
[14]: https://forum.aspose.com/c/words




