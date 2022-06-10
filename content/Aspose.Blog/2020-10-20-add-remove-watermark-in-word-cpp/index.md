---
title: 'Add or Remove Watermark in Word (DOC/DOCX) using C++'
seoTitle: "Add Insert Delete Remove Watermark in Word DOC/DOCX with C++"
description: "You can programmatically Add Insert Delete Remove Watermark in Word DOC/DOCX document files with C++. Image or Text watermark can be used."
date: Tue, 20 Oct 2020 06:16:43 +0000
draft: false
url: /2020/10/20/add-remove-watermark-in-word-cpp/
author: Farhan Raza
summary: 'Watermarks are usually used to show ownership or the nature of the document. You can add/insert or remove watermark in Word Documents (DOC/DOCX) programmatically using C++. For instance, a word document contains classified information and you want to add a watermark in the file then these requirements can be met efficiently with Aspose.Words for C++ API.'
tags: ['add watermark in word', 'delete watermark from word', 'insert watermark in word', 'remove watermark from word', 'remove watermark in docx using C++', 'watermark in docx with C++', 'watermark in word']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/add-remove-watermark-in-word-c.png" alt="Add Remove Watermark in Word C++">}}


Watermarks are usually used to show ownership or the nature of the document. You can add/insert or remove watermark in Word Documents ([DOC][1]/[DOCX][2] programmatically using C++. For instance, a word document contains classified information and you want to add a watermark in the file then these requirements can be met efficiently with [Aspose.Words for C++][3] API.

*   [Insert or Remove Watermark in Word Files in C++ – API Installation][4]
*   [Add or Insert Text Watermark in Word Document (DOC/DOCX) using C++][5]
*   [Add or Insert Image Watermark in Word Document (DOC/DOCX) using C++][6]
*   [Delete or Remove Watermark from Word Document (DOC/DOCX) using C++][7]

## Insert or Remove Watermark in Word Files – API Installation {#section1}

For working with watermarks in word documents, you need to configure Aspose.Words for C++ API by downloading it from the [official site][8], or via the following [NuGet][9] command:

```
Install-Package Aspose.Words.Cpp -Version 20.10.0
```

After installing it, you will be able to edit and manipulate Microsoft Word Document formats including DOC, DOCX, and other [supported file formats][10].

## Add or Insert Text Watermark in Word Document (DOC/DOCX) using C++ {#section2}

You can add or insert watermark text in word documents using C++. Moreover, you can control the formatting of text like font style, size, color, and transparency. You need to follow the steps below for inserting watermark text in Word documents (DOC/DOCX).

1.  Load input document
2.  Initialize TextWatermarkOptions object
3.  Set Font Style, Size, and Color
4.  Set Text as Watermark
5.  Save the output word document

The code snippet below shows how to add or insert text watermark in word documents using C++:

{{< gist aspose-com-gists da4488531d68cbaad746340b8dd19dfa "AddTextWatermark.cpp" >}}

## Add or Insert Image Watermark in Word Document (DOC/DOCX) using C++ {#section3}

You can add or insert image watermark in word documents (DOC/DOCX) by your C++ applications. The picture may contain some text or logo with some transparency value. You need to follow the following steps to add an image watermark in a word document:

1.  Load input word document
2.  Initialize an object of ImageWatermarkOptions class
3.  Load watermark image
4.  Save the output word file

The following code is based on these steps which shows how to add or insert image watermark in word documents using C++:

{{< gist aspose-com-gists da4488531d68cbaad746340b8dd19dfa "AddImageWatermark.cpp" >}}

## Delete or Remove Watermark from Word Document (DOC/DOCX) using C++ {#section4}

You might need to update a watermark in a word document. In many such related scenarios, you might want to remove or delete a watermark from word document (DOC/DOCX). The API gives you the control to decide if you want to delete a text watermark or image watermark because single word document can contain more than one kind of watermark. Here we will be removing text watermark in a DOCX file with the following steps:

1.  Load input word document
2.  Access watermark of Text type
3.  Remove Text watermark in the document
4.  Save output word document

The code below shows how to delete or remove watermark from DOC/DOCX word document using C++:

{{< gist aspose-com-gists da4488531d68cbaad746340b8dd19dfa "RemoveWatermark.cpp" >}}

## Conclusion

We have learned how to add or insert watermark in word documents (DOC/DOCX) programmatically using the C++ language. You can insert text or image watermark as per your requirements. Moreover, you can also remove or delete a watermark from a word document. Both image and text watermarks can be removed using C++. Furthermore, you can explore the API further by referring to [Product Documentation][11], [API References][12], [Examples Project][13], or you can reach us anytime at [Free Support Forum][14] for any query.

## See Also

[Convert Word (DOC/DOCX) to HTML MHTML Programmatically using C++][15]




[1]: https://docs.fileformat.com/word-processing/doc/
[2]: https://docs.fileformat.com/word-processing/docx/)
[3]: https://products.aspose.com/words/cpp
[4]: #section1
[5]: #section2
[6]: #section3
[7]: #section4
[8]: https://releases.aspose.com/
[9]: https://www.nuget.org/packages/Aspose.Words.Cpp/
[10]: https://docs.aspose.com/words/cpp/supported-document-formats/
[11]: https://docs.aspose.com/words/cpp/
[12]: https://apireference.aspose.com/words/cpp
[13]: https://github.com/aspose-words/Aspose.Words-for-C
[14]: https://forum.aspose.com/c/words
[15]: https://blog.aspose.com/2020/08/19/convert-word-to-html-mhtml-cpp/





