---
title: 'Convert Word Documents to PNG, JPEG, or BMP in Python'
seoTitle: "Convert Word to PNG, JPG, or BMP in Python | Python Word to Image"
description: "Use Python Word library to convert Word documents to PNG, JPEG, BMP image in python. Control DOCX or DOC files to image conversion dynamically."
date: Thu, 04 Nov 2021 14:05:13 +0000
draft: false
url: /2021/11/04/convert-word-to-png-jpg-bmp-in-python/
author: Usman Aziz
summary: "The conversion of MS Word files to image formats lets you embed the document's pages into your web or desktop applications. In order to perform this conversion from within the Python applications, this article covers **how to convert Word [DOCX][1] or [DOC][2] files to [PNG][3], [JPEG][4], or [BMP][5] images using Python**. Moreover, you will learn how to control the Word to image conversion using different options."
tags: ['Convert Word to BMP Python', 'Convert Word to Image Python', 'Convert Word to JPEG Python', 'Convert Word to PNG Python', 'DOC DOCX to Image in Python']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Word-to-Image.jpg" alt="Word to PNG JPEG BMP using Python">}}


The conversion of MS Word files to image formats lets you embed the document's pages into your web or desktop applications. In order to perform this conversion from within the Python applications, this article covers **how to convert Word [DOCX][6] or [DOC][7] files to [PNG][8], [JPEG][9], or [BMP][10] images using Python**. Moreover, you will learn how to control the Word to image conversion using different options.

*   [Python API for Word to Image Conversion][11]
*   [Convert a Word Document to PNG, JPEG, or BMP][12]
*   [Control Word to Image Conversion][13]

## Python API for Word to Image Conversion {#Python-API-for-Word-to-Image-Conversion}

To convert Word documents to PNG. JPEG, or BMP images, we will use [Aspose.Words for Python][14]. It is a powerful Python library to create, process, and convert MS Word documents. Aspose.Words for Python is available on [PyPI][15] and you can install it using the following pip command.

```
pip install aspose-words
```

## Convert a Word Document to PNG, JPEG, or BMP in Python {#Convert-a-Word-Document-to-PNG-JPEG-or-BMP}

It is quite easier to convert a Word document to popular images formats using Aspose.Words for Python. You can opt for the desired output image format from PNG, JPEG, and BMP. The following are the steps to convert a Word document to a PNG image using Python.

*   Load the Word document using _Document_ class.
*   Specify the output image format using _ImageSaveOptions_ class.
*   Loop through the page count in the document.
*   Convert each page in Word document to PNG image using _Document.save(string, ImageSaveOptions)_ method.

The following code sample shows how to convert a Word document to PNG images in Python.

{{< gist aspose-com-gists b34557af65be5264d357aa828e9e3f67 "word-to-image.py" >}}

## Control Word to Image Conversion in Python {#Control-Word-to-Image-Conversion}

You can also control the Word to image conversion using different options. For example, you can set horizontal resolution, vertical resolution, overall resolution, scale, pixel format, brightness, color mode, contrast, and paper color. The following are the steps to use the above-mentioned features in Word to image conversion using Python.

*   Load the Word document using _Document_ class.
*   Specify the output image format using _ImageSaveOptions_ class.
*   Set desired options such as _ImageSaveOptions_._image\_brightness_, _ImageSaveOptions_._image\_brightness_, etc.
*   Loop through the page count in the document.
*   Convert each page to image using _Document.save(string, ImageSaveOptions)_ method.

The following code sample shows how to control Word to JPEG image conversion using different options.

{{< gist aspose-com-gists b34557af65be5264d357aa828e9e3f67 "word-to-image-custom.py" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can [get a temporary license][16] in order to use Aspose.Words for Python without evaluation limitations.

**Info**: You may be interested in another Python API ([Aspose.Slides for Python via NET][17] that allows you to [convert presentations to images][18] and [import images into presentations][19].

## Conclusion

In this article, you have learned how to convert Word documents to PNG, JPEG, or BMP images using Python. Moreover, you have seen how to control Word to image conversion using different options. Apart from that, you can explore other features offered by Aspose.Words for Python using the [documentation][20]. Also, you can post your questions on our [forum][21].

## See Also

*   [Convert Word Files to PDF using Python][22]
*   [Create Word Documents in Python without MS Office][23]




[1]: https://docs.fileformat.com/word-processing/docx/
[2]: https://docs.fileformat.com/word-processing/doc/
[3]: https://docs.fileformat.com/image/png/
[4]: https://docs.fileformat.com/image/jpeg/
[5]: https://docs.fileformat.com/image/bmp/
[6]: https://docs.fileformat.com/word-processing/docx/
[7]: https://docs.fileformat.com/word-processing/doc/
[8]: https://docs.fileformat.com/image/png/
[9]: https://docs.fileformat.com/image/jpeg/
[10]: https://docs.fileformat.com/image/bmp/
[11]: #Python-API-for-Word-to-Image-Conversion
[12]: #Convert-a-Word-Document-to-PNG-JPEG-or-BMP
[13]: #Control-Word-to-Image-Conversion
[14]: https://products.aspose.com/words/python/
[15]: https://pypi.org/project/aspose-words/
[16]: https://purchase.aspose.com/temporary-license
[17]: https://products.aspose.com/slides/python-net/)
[18]: https://products.aspose.app/slides/conversion/ppt-to-jpg
[19]: https://products.aspose.app/slides/import/jpg-to-ppt
[20]: https://docs.aspose.com/words/python/product-overview/
[21]: https://forum.aspose.com/
[22]: https://blog.aspose.com/2021/10/27/convert-word-to-pdf-in-python/
[23]: https://blog.aspose.com/2021/10/28/create-word-documents-using-python/




