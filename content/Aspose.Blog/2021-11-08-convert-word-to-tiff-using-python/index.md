---
title: 'Convert Word Documents to TIFF using Python'
seoTitle: "Convert Word Documents to TIFF in Python | DOCX, DOC to TIFF"
description: "Use Python Word library to convert Word documents to multipage TIFF images in Python. Customize DOCX to TIFF or DOC to TIFF with different options."
date: Mon, 08 Nov 2021 14:52:20 +0000
draft: false
url: /2021/11/08/convert-word-to-tiff-using-python/
author: Usman Aziz
summary: '[TIFF][1] is a popular format to store raster images. Unlike other image formats, TIFF supports multiple pages. It means, a multipage TIFF file can have more than one images in the form of pages. This feature makes TIFF a suitable option to render the Word documents. To perform this conversion programmatically, this article covers **how to convert Word [DOCX][2] or [DOC][3] files to TIFF using Python**.'
tags: ['doc to tiff in python', 'docx to tiff python', 'word to tiff in python']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Word-to-Tiff.jpg" alt="Convert Word to TIFF in Python">}}


[TIFF][4] is a popular format to store raster images. Unlike other image formats, TIFF supports multiple pages. It means, a multipage TIFF file can have more than one images in the form of pages. This feature makes TIFF a suitable option to render the Word documents. To perform this conversion programmatically, this article covers **how to convert Word [DOCX][5] or [DOC][6] files to TIFF using Python**.

*   [Python Library for Word to TIFF Conversion][7]
*   [Convert a Word Document to TIFF][8]
*   [Customize Word to TIFF Conversion][9]

## Python Library for Word to TIFF Conversion {#Python-Library-for-Word-to-TIFF-Conversion}

In order to convert DOCX or DOC documents to TIFF format, we will use [Aspose.Words for Python][10]. It is a powerful Python library to create and manipulate Word documents seamlessly. Moreover, it provides a high fidelity conversion of Word files to other popular document and image formats. You can install the library from [PyPI][11] using the following pip command.

```
pip install aspose-words
```

## Convert a Word Document to TIFF using Python {#Convert-a-Word-Document-to-TIFF}

The following are the steps to convert a Word document to multipage TIFF using Python.

*   Load the Word file using _Document_ class.
*   Save the document as TIFF file using _Document.save(string)_ method.

The following code sample shows how to convert a Word document to TIFF format.

{{< gist aspose-com-gists d976d7e4bbfa9eae014c85d1bdf06620 "word-to-tiff.py" >}}

## Customize Word to TIFF Conversion using Python {#Customize-Word-to-TIFF-Conversion}

You can also customize the Word to TIFF conversion using different options. For example, you can set the image brightness, resolution, range of pages to convert, compression scheme, and so on. To set these options, _ImageSaveOptions_ class is used. The following are the steps to set different options in Word to TIFF conversion.

*   Load the Word file using _Document_ class.
*   Create an instance of _ImageSaveOptions_ class.
*   Pass the input image format in the constructor of _ImageSaveOptions_.
*   Set the desired options for the converted TIFF.
*   Convert Word to TIFF using _Document.save(string, ImageSaveOptions)_ method.

The following code sample shows how to convert a Word document to TIFF with additional options.

{{< gist aspose-com-gists d976d7e4bbfa9eae014c85d1bdf06620 "word-to-tiff-custom.py" >}}

## Get a Free API License {#Get-a-Free-API-License}

Use Aspose.Words for Python without evaluation limitations using a [free temporary license][12].

## Conclusion

In this article, you have seen how to convert Word documents to TIFF format using Python. Also, you have learned how to use different options to customize Word to TIFF conversion dynamically. Besides, you can visit the [documentation][13] of Aspose.Words for Python to explore other features. You can also ask your questions via our [forum][14].

## See Also

*   [Convert Word Files to PDF using Python][15]
*   [Create Word Documents in Python without MS Office][16]




[1]: https://docs.fileformat.com/image/tiff/
[2]: https://docs.fileformat.com/word-processing/docx/
[3]: https://docs.fileformat.com/word-processing/doc/
[4]: https://docs.fileformat.com/image/tiff/
[5]: https://docs.fileformat.com/word-processing/docx/
[6]: https://docs.fileformat.com/word-processing/doc/
[7]: #Python-Library-for-Word-to-TIFF-Conversion
[8]: #Convert-a-Word-Document-to-TIFF
[9]: #Customize-Word-to-TIFF-Conversion
[10]: https://products.aspose.com/words/python/
[11]: https://pypi.org/project/aspose-words/
[12]: https://purchase.aspose.com/temporary-license
[13]: https://docs.aspose.com/words/python/
[14]: https://forum.aspose.com/
[15]: https://blog.aspose.com/2021/10/27/convert-word-to-pdf-in-python/
[16]: https://blog.aspose.com/2021/10/28/create-word-documents-using-python/




