---
title: 'Extract Text and Images from OneNote Documents using C#'
date: Tue, 22 Feb 2022 05:01:50 +0000
draft: false
url: /2022/02/22/extract-text-and-images-from-onenote-documents-using-csharp/
author: 'Muzammil Khan'
summary: 'You can easily extract text or images from OneNote documents programmatically without using MS OneNote. In this article, you will learn **how to extract text and images from OneNote documents using C#**.'
tags: ['extract images', 'extract images from onenote', 'extract images onenote c#', 'extract text from onenote', 'extract text onenote c#']
categories: ['Aspose.Note Product Family']
---



{{< figure align=center src="images/extract-text-and-images-from-onenote-documents-using-csharp.jpg" alt="Extract Text and Images from OneNote Documents using C#">}}


We collect, organize, and collaborate notes and ideas in OneNote documents. It is a sort of digital notebook used to take notes and share with other OneNote users. In certain cases, we may need to extract text or images from OneNote documents programmatically without using MS OneNote. In this article, we will learn **how to extract text and images from OneNote documents using C#**.

The following topics shall be covered in this article:

*   [OneNote Text and Image Extractor C# API][1]
*   [Extract All the Text from OneNote Documents][2]
*   [Get Text from Specific Pages of OneNote Documents][3]
*   [Extract Images from OneNote Documents][4]

## OneNote Text and Image Extractor C# API {#OneNote-Text-and-Image-Extractor-CSharp-API}

For extracting text and images from the [OneNote][5] document, we will be using the [Aspose.Note for .NET][6] API. It is a feature-rich OneNote document manipulation API that lets you create, read, and convert OneNote documents programmatically. Please either [download][7] the DLL of the API or install it using [NuGet][8].

```
PM> Install-Package Aspose.Note
```

## Extract All the Text from OneNote Documents {#Extract-All-the-Text-from-OneNote-Documents}

We can easily extract all the text from the OneNote document by following the steps given below:

1.  Firstly, load a OneNote file using the **_[Document][9]_**class.
2.  After that, call the **_[GetChildNodes][10]_** method with RichText as _**[NodeType][11]**_ to extract text.
3.  Finally, show the extracted text.

The following code sample shows how to extract all the text from a OneNote file using C#.

{{< gist aspose-com-gists c472c90dc92b80a384e516e1064d722b "ExtractTextAndImagesFromOneNote_CSharp_ExtractAll.cs" >}}



{{< figure align=center src="images/Extract-All-the-Text-from-OneNote-Documents-1024x544.jpg" alt="Extract All the Text from OneNote Documents." caption="Extract All the Text from OneNote Documents.">}}


## Get Text from Specific Pages of OneNote Documents {#Get-Text-from-Specific-Pages-of-OneNote-Documents}

We can extract text from specific pages of the OneNote document by following the steps given below:

1.  Firstly, load a OneNote file using the **_[Document][12]_**class.
2.  Next, call the **_[GetChildNodes][13]_** method with **_[Page][14]_** as _**[NodeType][15]**_ to extract pages.
3.  After that, get a list of text items using the **_[GetChildNodes][16]_** method with RichText as _**[NodeType][17]**_.
4.  Finally, show the extracted text.

The following code sample shows how to extract text from a specific page of a OneNote file using C#.

{{< gist aspose-com-gists c472c90dc92b80a384e516e1064d722b "ExtractTextAndImagesFromOneNote_CSharp_ExtractFromPages.cs" >}}

## Extract Images from OneNote Documents {#Extract-Images-from-OneNote-Documents}

We can also extract images from the OneNote document by following the steps given below:

1.  Firstly, load a OneNote file using the **_[Document][18]_**class.
2.  After that, get a list of images using the **_[GetChildNodes][19]_** method with _**[Image][20]**_ as _**[NodeType][21]**_.
3.  Finally, show the image properties and save to local disk.

The following code sample shows how to extract images from a OneNote file using C#.

{{< gist aspose-com-gists c472c90dc92b80a384e516e1064d722b "ExtractTextAndImagesFromOneNote_CSharp_ExtractImages.cs" >}}



{{< figure align=center src="images/Extract-Images-from-OneNote-Documents-1024x512.jpg" alt="Extract Images from OneNote Documents." caption="Extract Images from OneNote Documents.">}}


## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][22] to try the library without evaluation limitations.

## Conclusion

In this article, we have learned **how to extract text from the OneNote document or from specific pages** of the document. We have also seen **how to extract images from OneNote documents** programmatically. Besides, you can learn more about Aspose.Note for .NET API using the [documentation][23]. In case of any ambiguity, please feel free to contact us on the [forum][24].

## See Also

*   [Insert or Extract Image from OneNote .one File in C# .NET][25]




[1]: #OneNote-Text-and-Image-Extractor-CSharp-API
[2]: #Extract-All-the-Text-from-OneNote-Documents
[3]: #Get-Text-from-Specific-Pages-of-OneNote-Documents
[4]: #Extract-Images-from-OneNote-Documents
[5]: https://docs.fileformat.com/note-taking/one/
[6]: https://products.aspose.com/note/net
[7]: https://downloads.aspose.com/note/net
[8]: https://www.nuget.org/packages/aspose.note
[9]: https://apireference.aspose.com/note/net/aspose.note/document
[10]: https://apireference.aspose.com/note/net/aspose.note.compositenode/1/methods/getchildnodes/_1
[11]: https://apireference.aspose.com/note/net/aspose.note/nodetype
[12]: https://apireference.aspose.com/note/net/aspose.note/document
[13]: https://apireference.aspose.com/note/net/aspose.note.compositenode/1/methods/getchildnodes/_1
[14]: https://apireference.aspose.com/note/net/aspose.note/page
[15]: https://apireference.aspose.com/note/net/aspose.note/nodetype
[16]: https://apireference.aspose.com/note/net/aspose.note.compositenode/1/methods/getchildnodes/_1
[17]: https://apireference.aspose.com/note/net/aspose.note/nodetype
[18]: https://apireference.aspose.com/note/net/aspose.note/document
[19]: https://apireference.aspose.com/note/net/aspose.note.compositenode/1/methods/getchildnodes/_1
[20]: https://apireference.aspose.com/note/net/aspose.note/image
[21]: https://apireference.aspose.com/note/net/aspose.note/nodetype
[22]: https://purchase.aspose.com/temporary-license
[23]: https://docs.aspose.com/note/net/
[24]: https://forum.aspose.com/c/note/28
[25]: https://blog.aspose.com/2021/10/05/insert-extract-image-onenote-csharp/




