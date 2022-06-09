---
title: 'Find and Replace Text in OneNote file Programmatically in C#'
seoTitle: "C# Find and Replace Text in OneNote file Programmatically in .NET"
description: "You can find and replace text in onenote file programmatically using C# language in .NET framework based applicatons. Search and Replace text."
date: Wed, 17 Mar 2021 01:04:00 +0000
draft: false
url: /2021/03/17/find-replace-text-onenote-csharp/
author: Farhan Raza
summary: 'OneNote file contain digital notes that are stored in hierarchy as different pages and sections. Such files may contain text, drawings, images etc., for different purposes. You may need to find and replace some text in OneNote files. Instead of going through different pages or sections every time, you can easily perform the task programmatically using C# language. Let us check out the following use cases for more information.'
tags: ['find and replace onenote', 'replace text onenote', 'search and replace in onenote', 'search note']
categories: ['Aspose.Note Product Family']
---



{{< figure align=center src="images/Find-and-Replace-Text-OneNote.png" alt="find replace text onenote">}}


OneNote files contain digital notes that are stored in the hierarchy as different pages and sections. Such files may contain text, drawings, images, etc., for different purposes. You may need to find and replace some text in OneNote files. Instead of going through different pages or sections every time, you can easily perform the task programmatically using C# language. Please check out the following use cases for details:

*   [Search and Replace Text in OneNote File – C# API Installation][1]
*   [Find and Replace Text in all Pages of OneNote file Programmatically in C#][2]
*   [Find and Replace Text on a Specific Page of OneNote file with C#][3]

## Search and Replace Text in OneNote File – C# API Installation {#section1}

[Aspose.Note for .NET][4] API supports creating, editing, and manipulating OneNote files. Installing the API is pretty simple as you can quickly download the DLL file from the [New Releases][5] section. Alternatively, you can configure the API from [NuGet][6] gallery with the following installation command in Microsoft Visual Studio IDE:

```
PM> Install-Package Aspose.Note
```

## Find and Replace Text in all Pages of OneNote file Programmatically in C# {#section2}

OneNote files can contain several pages of text, shapes, images, or drawings. Moreover, several text phrases can repeat on different pages and you may need to search and replace all instances. You need to follow the following steps to find and replace text on all pages of the OneNote file:

1.  Specify search and replace string.
2.  Load the input document using the [Document][7] class.
3.  Get all [RichText][8] nodes.
4.  Update the replaced string in the file.
5.  Save updated one note file.

The code below elaborates how to find and replace text on all pages of OneNote file (.one) programmatically using C#:

{{< gist aspose-com-gists 96e35f16c7b847479832665a28f2340e "find-replace-text-onenote-all-pages.cs" >}}

## Find and Replace Text on a Specific Page of OneNote file with C# {#section3}

You can find and replace specific instances of text in OneNote files. Please follow the steps below to update text on a specific page of a OneNote file:

1.  Specify find and replace string.
2.  Load the input document into Aspose.Note.
3.  Get all [RichText][9] nodes.
4.  Update text on a specific page.
5.  Save output .one file using [Save][10] method.

The following code shows how to find and replace text on a specific page in OneNote file programmatically with C#:

{{< gist aspose-com-gists 96e35f16c7b847479832665a28f2340e "find-replace-text-onenote-specific-page.cs" >}}

## Conclusion

In conclusion, you have learned how to find and replace text contents in OneNote (.one) file. Moreover, you have explored different use cases related to text contents in a .one file. You can take a look at different features of the API by visiting the [Documentation][11]. Furthermore, you can always get in touch with us for discussing your use case or POC by writing to us at [Free Support Forum][12]. Happy coding!

## See Also

[Create OneNote (.ONE) Documents Programmatically in C#][13]




[1]: #section1
[2]: #section2
[3]: #section3
[4]: https://products.aspose.com/note/net
[5]: https://downloads.aspose.com/note/net
[6]: https://www.nuget.org/packages/Aspose.Note
[7]: https://apireference.aspose.com/note/net/aspose.note/document
[8]: https://apireference.aspose.com/note/net/aspose.note/richtext
[9]: https://apireference.aspose.com/note/net/aspose.note/richtext
[10]: https://apireference.aspose.com/note/net/aspose.note/document/methods/save/index
[11]: https://docs.aspose.com/note/net/
[12]: https://forum.aspose.com/c/note
[13]: https://blog.aspose.com/2020/05/08/create-onenote-files-add-images-tables-tags-to-onenote-file-using-csharp/





