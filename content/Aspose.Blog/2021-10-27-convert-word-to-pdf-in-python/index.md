---
title: 'Convert Word DOCX or DOC to PDF in Python'
seoTitle: "Convert Word to PDF in Python | DOCX to PDF, DOC to PDF in Python"
description: "Use Python Word Processing API to convert Word DOCX/DOC files to PDF in Python. Customize Word to PDF conversion from within your Python applications."
date: Wed, 27 Oct 2021 15:59:27 +0000
draft: false
url: /2021/10/27/convert-word-to-pdf-in-python/
author: Usman Aziz
summary: 'Word to [PDF][1] is one of the most popular and immensely performed document conversions. The [DOCX][2] or [DOC][3] files are converted to PDF format before they are printed or shared. In this article, we will automate **Word to PDF conversion in Python**. The steps and code samples will demonstrate how to convert **DOCX or DOC files to PDF within a few lines of Python code**. Also, you will learn about different options to customize Word to PDF conversion.'
tags: ['doc to pdf python', 'docx to pdf python', 'python word to pdf converter', 'word to pdf python']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Word-to-PDF-Conversion-C.png" alt="Word to PDF Conversion Python">}}


Word to [PDF][4] is one of the most popular and immensely performed document conversions. The [DOCX][5] or [DOC][6] files are converted to PDF format before they are printed or shared. In this article, we will automate **Word to PDF conversion in Python**. The steps and code samples will demonstrate how to convert **DOCX or DOC files to PDF within a few lines of Python code**. Also, you will learn about different options to customize Word to PDF conversion.

*   [Python API for DOCX/DOC to PDF Conversion][7]
*   [Convert Word DOCX/DOC to PDF][8]
*   [Word to PDF with a Particular PDF Standard][9]
*   [Convert Range of Pages in Word document to PDF][10]
*   [Apply Image Compression in Word to PDF][11]

## Python API for Word to PDF Conversion {#API-for-Word-to-PDF-Conversion}

For converting Word documents to PDF format, we will use [Aspose.Words for Python][12]. It is a feature-rich Python library for creating and manipulating Word documents. Moreover, it lets you convert DOCX and DOC files to PDF format with high fidelity. The library is hosted on [PyPI][13] and you can install it using the following pip command.

```
pip install aspose-words
```

## Convert Word DOCX/DOC to PDF using Python {#Convert-Word-to-PDF}

The following are the steps to convert a Word document to PDF in Python.

*   Load the Word document using _Document_ class.
*   Convert Word document to PDF using _Document.save()_ method.

The following code sample shows how to convert a Word DOCX file to PDF.

{{< gist aspose-com-gists 55ed600cecd8b9a8a882e398b2682851 "word-to-pdf.py" >}}

## Python Word to PDF with a Particular Standard {#Word-to-PDF-with-a-Particular-PDF-Standard}

You can also specify the particular standard for the converted PDF document such as PDF/A. The following are the steps to specify the PDF standard in Word to PDF conversion using Python.

*   Load the Word document using _Document_ class.
*   Create an object of _PdfSaveOptions_ class and set PDF standard using _PdfSaveOptions.compliance_ property.
*   Convert Word document to PDF using _Document.save()_ method.

The following code sample shows how to set a particular standard in Word to PDF conversion.

{{< gist aspose-com-gists 55ed600cecd8b9a8a882e398b2682851 "word-to-pdf-compliance.py" >}}

## Convert Range of Pages in DOCX/DOC to PDF using Python {#Convert-Range-of-Pages-in-Word-document-to-PDF}

You can also specify the range of pages you want to convert to PDF format. For this, you can use _PdfSaveOptions.page\_set_ property. The following code sample shows how to convert a range of pages in Word document to PDF.

{{< gist aspose-com-gists 55ed600cecd8b9a8a882e398b2682851 "word-to-pdf-pages.py" >}}

## Apply Image Compression in DOCX to PDF using Python {#Apply-Image-Compression-in-Word-to-PDF}

Aspose.Words for Python also lets you apply image compression in the converted PDF document. In addition, you can specify the JPEG quality for the images. The following are the steps to set image compression while converting a Word document to PDF in Python.

*   Load the Word document using _Document_ class.
*   Create an object of _PdfSaveOptions_ class.
*   Set image compression using _PdfSaveOptions.image\_compression_ property.
*   Set JPEG quality using _PdfSaveOptions.jpeg\_quality_ property.
*   Convert Word document to PDF using _Document.save()_ method.

The following code sample shows how to set image compression in Word to PDF conversion.

{{< gist aspose-com-gists 55ed600cecd8b9a8a882e398b2682851 "word-to-pdf-image-compression.py" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can [get a temporary license][14] in order to use Aspose.Words for Python without evaluation limitations.

**Info**: You may be interested in another Python API that allows developers and applications to convert PowerPoint to PDF - [Aspose.Slides for Python][15]. And you might also want to check out Aspose [PowerPoint to PDF Converter][16] because it is a live implementation of the PowerPoint to PDF conversion process.

## Conclusion

In this article, you have learned how to convert Word DOCX or DOC files to PDF in Python. Moreover, you have seen different options to customize the Word to PDF conversion programmatically. You can learn more about Aspose.Words for Python using [documentation][17]. In case you would have any questions, feel free to let us know via our [forum][18].

## See Also

*   [Create MS Word Documents using Python][19]
*   [Convert Word Documents to Image in Python][20]
*   [Create MS Word Documents (DOC/DOCX) using C++][21]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/word-processing/docx/
[3]: https://docs.fileformat.com/word-processing/doc/
[4]: https://docs.fileformat.com/pdf/
[5]: https://docs.fileformat.com/word-processing/docx/
[6]: https://docs.fileformat.com/word-processing/doc/
[7]: #API-for-Word-to-PDF-Conversion
[8]: #Convert-Word-to-PDF
[9]: #Word-to-PDF-with-a-Particular-PDF-Standard
[10]: #Convert-Range-of-Pages-in-Word-document-to-PDF
[11]: #Apply-Image-Compression-in-Word-to-PDF
[12]: https://products.aspose.com/words/python/
[13]: https://pypi.org/project/aspose-words/
[14]: https://purchase.aspose.com/temporary-license
[15]: https://products.aspose.com/slides/python-net/
[16]: https://products.aspose.app/slides/conversion
[17]: https://docs.aspose.com/words/python/product-overview/
[18]: https://forum.aspose.com/
[19]: https://blog.aspose.com/2021/10/28/create-word-documents-using-python/
[20]: https://blog.aspose.com/2021/11/04/convert-word-to-png-jpg-bmp-in-python/
[21]: https://blog.aspose.com/2020/08/25/create-ms-word-documents-using-cpp/




