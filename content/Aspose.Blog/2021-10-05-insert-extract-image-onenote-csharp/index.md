---
title: 'Insert or Extract Images from OneNote File in C#'
seoTitle: "Insert or Extract Image from OneNote .one File in C# .NET"
description: "You can insert or extract image from OneNote .one file programmatically in .NET framework using C#. Insert or Export pictures from .one file."
date: Tue, 05 Oct 2021 08:18:00 +0000
draft: false
url: /2021/10/05/insert-extract-image-onenote-csharp/
author: Farhan Raza
summary: 'OneNote files are popularly used for taking notes. In certain situations, you might need to extract or insert an image in a OneNote .one document. This article covers **how to insert or extract images from a OneNote file using C#.**'
tags: ['Extract image from .one csharp', 'Extract image from OneNote', 'Insert Image in OneNote', 'Insert Image into .one csharp']
categories: ['Aspose.Note Product Family']
---



{{< figure align=center src="images/Insert-Extract-Image-OneNote-1.jpg" alt="Insert Extract Image OneNote">}}


OneNote files are popularly used for taking notes. In certain situations, you might need to extract or insert an image in a OneNote [.one][1] document. This article covers how to insert or extract images from a OneNote file using C#.

*   [Insert or Extract Image from OneNote .one File – C# API Installation][2]
*   [Insert Image in OneNote .one File in C#][3]
*   [Extract Images from OneNote .one File using C#][4]

## Insert or Extract Image in OneNote .one File – .NET API Installation {#section1}

[Aspose.Note for .NET][5] API supports creating or editing the OneNote files. You can configure it by downloading the DLL file from the Downloads section or using the below [NuGet][6] installation command in Microsoft Visual Studio IDE:

```
PM> Install-Package Aspose.Note
```

## Insert Image in OneNote .one File in C# {#section2}

You can insert an image in a OneNote document with the following steps:

1.  Initialize a [LoadOptions][7] class object.
2.  Load the input OneNote file with the [Document][8] class.
3.  Get the first page of the document with [FirstChild][9] property.
4.  Add the image to the page with [appendChildLast][10] method.
5.  Finally, save the output OneNote file.

The code snippet below shows how to insert an image in a OneNote .one document using C#:

{{< gist aspose-com-gists 12bbcc53310dce4971854eae512f54e8 "Insert-Image-OneNote.cs" >}}

## Extract Images from OneNote .one File using C# {#section3}

You can extract images from a OneNote file with the following steps:

1.  Firstly, load the input OneNote file with the [Document][11] class.
2.  Get all images using [GetChildNodes][12] method.
3.  Traverse the list and save output images.

The following code sample explains how to extract images from a OneNote document using C#:



## Get Free API License

You can request a [free temporary license][13] for evaluating the API without any limitations.

## Conclusion

In conclusion, you have learned how to extract or insert image into a OneNote .one file in C#. You can explore several other features of the API by taking a look at the [documentation][14]. Furthermore, you can contact us at the [free support forum][15] in case of any concerns.

## See Also

[Print OneNote .one NoteBook File using C#][16]




[1]: https://docs.fileformat.com/note-taking/one/
[2]: #section1
[3]: #section2
[4]: #section3
[5]: https://products.aspose.com/note/net/
[6]: https://www.nuget.org/packages/Aspose.Note
[7]: https://apireference.aspose.com/note/net/aspose.note/loadoptions
[8]: https://apireference.aspose.com/note/net/aspose.note/document
[9]: https://apireference.aspose.com/note/net/aspose.note.compositenode/1/properties/firstchild
[10]: https://apireference.aspose.com/note/net/aspose.note.compositenode/1/methods/appendchildlast/_1
[11]: https://apireference.aspose.com/note/net/aspose.note/document
[12]: https://apireference.aspose.com/note/net/aspose.note.compositenode/1/methods/getchildnodes/index
[13]: https://purchase.aspose.com/temporary-license
[14]: https://docs.aspose.com/note/net/
[15]: https://forum.aspose.com/
[16]: https://blog.aspose.com/2021/10/20/print-onenote-csharp/




