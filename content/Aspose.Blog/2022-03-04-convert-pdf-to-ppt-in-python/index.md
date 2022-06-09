---
title: 'Convert PDF Files to PowerPoint PPT in Python'
seoTitle: "Python: Convert PDF to PowerPoint PPT PPTX | Python PPTX Library"
description: "Use Python PowerPoint library to convert PDF to PPT or PPTX in Python. Import pages from PDF to slides in PowerPoint presentation in Python."
date: Fri, 04 Mar 2022 11:49:19 +0000
draft: false
url: /2022/03/04/convert-pdf-to-ppt-in-python/
author: Usman Aziz
summary: '[PDF][1] format is very much in the business for creating and sharing digital documents. Since it provides cross-platform support, people opt to send and receive documents in PDF format. There could be the case when you need to import the content from a PDF file to another document such as Word, PowerPoint, etc. To accomplish this programmatically, in this article, you will learn **how to convert a PDF file to PowerPoint PPT/PPTX in Python**.'
tags: ['Convert a PDF File to PowerPoint PPT', 'Python Library for PDF to PowerPoint Conversion', 'convert pdf to ppt in python', 'convert pdf to pptx in python']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Convert-PDF-to-PPT-C.png" alt="Convert PDF Files to PowerPoint PPT in Python">}}


[PDF][2] format is very much in the business for creating and sharing digital documents. Since it provides cross-platform support, people opt to send and receive documents in PDF format. There could be the case when you need to import the content from a PDF file to another document such as Word, PowerPoint, etc. To accomplish this programmatically, in this article, you will learn **how to convert a PDF file to PowerPoint PPT/PPTX in Python**.

*   [Python Library for PDF to PowerPoint Conversion][3]
*   [Convert a PDF File to PowerPoint PPT][4]

## Python Library for PDF to PowerPoint PPT Conversion {#Library-for-PDF-to-PowerPoint-Conversion}

[Aspose.Slides for Python][5] is an amazing library that provides basic as well as advanced features to create and manipulate PowerPoint presentations. In addition, it provides high-fidelity conversion of presentations to other formats. We will use this library to import content from PDF to PPT/PPTX slides. You can install the library from [PyPI][6] using the following command.

```
> pip install aspose.slides
```

## Convert PDF to PowerPoint PPT in Python {#Convert-a-PDF-File-to-PowerPoint-PPT}

In PDF to PowerPoint conversion, you do not need to go through the pages in PDF to import the content. Instead, Aspose.Slides for Python takes care of these operations and makes the conversion quite easier for you. The following is the workflow of PDF to PPT conversion.

*   Create an empty presentation.
*   Specify a PDF to import into presentation.
*   Aspose.Slides fetches the PDF pages and converts them to the slides.
*   Save presentation.

The following are the steps to convert a PDF file to PowerPoint PPTX in Python.

*   Create a new presentation using **Presentation** class.
*   Remove the default slide added to the presentation using **Presentation.slides.remove\_at(0)** method.
*   Import PDF to the presentation using **Presentation.slides.add\_from\_pdf(string)** method.
*   Save the presentation as a PPT/PPTX file using **Presentation.save(string, SaveFormat)** method.

The following code sample shows how to convert a PDF file to a PowerPoint presentation in Python.

{{< gist aspose-com-gists 56bb8e495d7312e480cb5132f6e5ba2a "pdf-to-ppt.py" >}}

The following is the PDF that we took to convert into the PowerPoint PPTX.



{{< figure align=center src="images/PDF-to-PPT-Conversion.png" alt="Convert PDF to PowerPoint PPT in Python">}}


Below is the PowerPoint presentation that we get after importing the PDF file.



{{< figure align=center src="images/PDF-to-PPT.png" alt="Python PDF to PPT PPTX">}}


## Get a Free License {#Get-a-Free-API-License}

You can use Aspose.Slides for Python without evaluation limitations by getting a [temporary license][7].

## Conclusion

In this article, you have learned how to convert a PDF file to PowerPoint PPT/PPTX in Python. We have demonstrated how Aspose.Slides for Python converts each page in PDF to a slide in PowerPoint PPT. Besides, you can visit the [documentation][8] to explore more about Aspose.Slides for Python. Also, you can post your queries to our [forum][9].

## See Also

*   [Create PowerPoint Files in Python][10]
*   [Convert PPTX to PDF in Python][11]
*   [Convert PPT to PNG in Python][12]
*   [Add Watermark in PowerPoint PPT in Python][13]
*   [Apply 3D Effects in PowerPoint PPT using Python][14]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: #Library-for-PDF-to-PowerPoint-Conversion
[4]: #Convert-a-PDF-File-to-PowerPoint-PPT
[5]: https://products.aspose.com/slides/python-net/
[6]: https://pypi.org/project/aspose.slides/
[7]: https://purchase.aspose.com/temporary-license
[8]: https://docs.aspose.com/slides/python-net/
[9]: https://forum.aspose.com/
[10]: https://blog.aspose.com/2021/12/31/create-powerpoint-presentations-in-python/
[11]: https://blog.aspose.com/2021/12/28/convert-pptx-ppt-to-pdf-python/
[12]: https://blog.aspose.com/2021/12/29/convert-ppt-to-png-in-python/
[13]: https://blog.aspose.com/2022/02/09/add-watermark-to-powerpoint-ppt-in-python/
[14]: https://blog.aspose.com/2022/01/08/create-three-d-effects-in-ppt-python/




