---
title: 'Extract Images from Word Documents in C#'
seoTitle: "Extract Images in Word Documents in C# | Image Extractor for DOCX DOC"
description: "Use .NET Word API to extract images from Word documents using C# or VB.NET. Extract images from DOCX or DOC and save them to the desired location."
date: Tue, 30 Nov 2021 06:56:57 +0000
draft: false
url: /2021/11/30/extract-images-from-word-in-csharp/
author: Usman Aziz
summary: 'Images play an important role to illustrate the key information in Word documents. Moreover, they make the document more attractive and improve its presentation. As a programmer, you may get a job to extract the images embedded within the Word DOCX or DOC documents. To achieve that, this article covers **how to extract images from Word documents programmatically using C#**. Moreover, you will see how to save the extracted images to the desired location.'
tags: ['dotnet image extractor for word documents', 'extract images from doc in csharp', 'extract images from docx in csharp', 'extract images from word in csharp']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Extract-Images-from-Word-Document.jpg" alt="Extract images from word documents using C#">}}


Images play an important role to illustrate the key information in Word documents. Moreover, they make the document more attractive and improve its presentation. As a programmer, you may get a job to extract the images embedded within the Word DOCX or DOC documents. To achieve that, this article covers **how to extract images from Word documents programmatically using C#**. Moreover, you will see how to save the extracted images to the desired location.

*   [.NET API to Extract Images from Word Documents][1]
*   [Extract Images from a Word Document][2]

**Tip**: If you ever need to get a Word document from a PowerPoint presentation, you can use Aspose [Presentation to Word Document][3] converter.

## C# API to Extract Images from Word Documents {#API-to-Extract-Images-from-Word-Documents}

To extract images from MS Word DOCX/DOC documents, we will use [Aspose.Words for .NET][4]. It is a powerful and widely used API for creating and manipulating Word documents. You can [download][5] the API's DLL and add its reference to your application. Also, you can install it directly from [NuGet][6] using the package manager console.

```
PM> Install-Package Aspose.Words
```

## Extract Images from a Word Document in C# {#Extract-Images-from-a-Word-Document}

In Word documents, images are represented as shapes. Therefore, to extract images, you will have to process all the shapes in the document. The following are the steps to extract images from a Word DOCX document programmatically in C#.

*   Load the Word file using [Document][7] class.
*   Get all the shapes which have images into an _IEnumerable<Shape>_ object using [Document.GetChildNodes(NodeType.Shape, Boolean)][8] method.
*   Loop through the retreieved shapes.
*   In each iteration, extract the image and save it using [Shape.ImageData.Save(string)][9] method.

The following code sample shows how to extract images from a Word document in C#.

{{< gist aspose-com-gists ca012b5e162ecd752c0c4dd990ca2089 "extract-images-from-word.cs" >}}

## Try Aspose.Words for .NET for Free

You can get a free temporary license to try Aspose.Words for .NET without any limitations. [Get your temporary license now][10].

## Conclusion

Images have become an integral part of Word documents, which make the content more attractive. Therefore, Aspose.Words for .NET provides a wide range of features to add or manipulate images in Word documents.

This article particularly covered the extraction of images from Word documents. With the help of a code sample, you have learned how to extract each image in a Word DOCX/DOC file programmatically using C#. Moreover, you have seen how to save the extracted images to your desired location. You can read more about Aspose.Words for .NET using the [documentation][11]. In case you would have any questions, feel free to let us know via our [forum][12].

## See Also

*   [Create Word Documents in C# without MS Office][13]
*   [Generate Word Documents from Templates in C# .NET][14]




[1]: #API-to-Extract-Images-from-Word-Documents
[2]: #Extract-Images-from-a-Word-Document
[3]: https://products.aspose.app/slides/conversion/ppt-to-word
[4]: https://products.aspose.com/words/net
[5]: https://downloads.aspose.com/words/net
[6]: https://www.nuget.org/packages/Aspose.Words
[7]: https://apireference.aspose.com/words/net/aspose.words/document
[8]: https://apireference.aspose.com/words/net/aspose.words/compositenode/methods/getchildnodes
[9]: https://apireference.aspose.com/words/net/aspose.words.drawing.imagedata/save/methods/1
[10]: https://purchase.aspose.com/temporary-license
[11]: https://docs.aspose.com/words/net/
[12]: https://forum.aspose.com/
[13]: https://blog.aspose.com/2020/01/08/csharp-word-automation-create-edit-process-word-documents/
[14]: https://blog.aspose.com/2020/03/05/generate-word-documents-from-templates-in-csharp-net/




