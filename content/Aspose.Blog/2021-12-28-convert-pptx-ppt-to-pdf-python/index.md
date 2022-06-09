---
title: 'Convert PPT to PDF in Python'
seoTitle: "Convert PPT to PDF in Python | Export PPTX PPT to PDF in Python"
description: "Convert PowerPoint PPTX PPT to PDF in Python. Customize PPTX to PDF conversion using different options. Set PDF compliance, password and access permissions."
date: Tue, 28 Dec 2021 09:31:48 +0000
draft: false
url: /2021/12/28/convert-pptx-ppt-to-pdf-python/
author: Usman Aziz
summary: '[PDF][1] is a popular and widely used file format having cross-platform support. The layout of PDF documents appears to be the same in heterogeneous environments. Thus, PDF becomes handy when you need to share your documents across multiple platforms. PowerPoint to PDF is among the common document conversions these days. To automate this conversion, we will show you **how to convert [PPTX][2] or [PPT][3] files to PDF format in Python**. Moreover, we will demonstrate how to customize the PPTX to PDF conversion using different options.'
tags: ['Convert PPTX to Password protected PDF in Python', 'Convert Selected Slides in PPTX to PDF in Python', 'Convert a PowerPoint PPTX File to PDF Python', 'Include Hidden Slides in PPTX to PDF Conversion Python', 'Python PPTX to PDF Converter Library', 'Set PDF Compliance in PPTX to PDF in Python']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Convert-PPT-PPTX-to-PDF-1.png" alt="Convert PPTX PPT to PDF in Python">}}


[PDF][4] is a popular and widely used file format having cross-platform support. The layout of PDF documents appears to be the same in heterogeneous environments. Thus, PDF becomes handy when you need to share your documents across multiple platforms. PowerPoint to PDF is among the common document conversions these days. To automate this conversion, we will show you **how to convert [PPT][5] or **[PPTX][6]**** **files to PDF format in Python**. Moreover, we will demonstrate how to customize the PPTX to PDF conversion using different options.

*   [Python PPT to PDF Converter Library][7]
*   [Convert a PowerPoint PPTX File to PDF][8]
*   [Include Hidden Slides in PPTX to PDF Conversion][9]
*   [Convert Selected Slides in PPTX to PDF][10]
*   [Set PDF Compliance in PPT to PDF Conversion][11]
*   [Convert PPTX to Password-protected PDF][12]

**TIP**: You want to try out Aspose FREE [PowerPoint to PDF][13] Converter.

## Python PPT to PDF Converter Library {#Python-PPTX-to-PDF-Converter-Library}

To convert the PowerPoint files to PDF format, we will use [Aspose.Slides for Python via .NET][14]. It is a powerful library that lets you automate the presentation manipulation operations from within your Python applications. Using the library, you can create, edit and convert the presentations seamlessly. You can install the library from [PyPI][15] using the following pip command.

```
> pip install aspose.slides
```

[Read more][16] about the system requirements to use this library.

## Convert a PPT to PDF in Python {#Convert-a-PowerPoint-PPTX-File-to-PDF}

The conversion of PPT files to PDF can be performed in a couple of steps. Just load the presentation file and save it as a PDF document. The following are the steps to convert a PPT file to PDF in Python.

*   Load the PPT/PPTX presentation using **Presentation** class.
*   Convert PPT to PDF using **Presentation.save(string, export.SaveFormat.PDF)** method.

The following code sample shows how to convert a PowerPoint PPTX to PDF in Python.

{{< gist aspose-com-gists cbc95264bf51d082800eca055e38cc5c "pptx-to-pdf.py" >}}

The following screenshot shows the input PPTX file that we used in this article.



{{< figure align=center src="images/PowerPoint-Presentation.png" alt="PowerPoint PPTX Presentation" caption="PPTX Presentation">}}


The following is the screenshot of the converted PDF file.



{{< figure align=center src="images/PPTX-to-PDF-in-Python.png" alt="PPTX to PDF Conversion" caption="PPTX Converted to PDF">}}


You would have noticed that the third slide in the PPTX presentation is marked as hidden. Therefore, it is not included in the converted PDF file. However, in certain cases, you may have to include hidden slides in PPTX to PDF conversion. So let's see how to achieve that.

## Include Hidden Slides - Python PPTX to PDF {#Include-Hidden-Slides-in-PPTX-to-PDF-Conversion}

To customize the PowerPoint to PDF conversion, Aspose.Slides for Python via .NET provides **PdfOptions** class. The following are the steps to include hidden slides in PowerPoint to PDF conversion in Python.

*   Load the PPTX presentation using **Presentation** class.
*   Create an object of **PdfOptions** class.
*   Set **PdfOptions.show\_hidden\_slides** property to **True**.
*   Convert PPTX to PDF using **Presentation.save(string, export.SaveFormat.PDF, **PdfOptions**)** method.

The following Python code sample shows how to include hidden slides in PPTX to PDF conversion.

{{< gist aspose-com-gists cbc95264bf51d082800eca055e38cc5c "pptx-to-pdf-hidden-slides.py" >}}

## Convert Selected Slides of PPT to PDF in Python {#Convert-Selected-Slides-in-PPTX-to-PDF}

Often, you may need to convert specific slides only to PDF instead of rendering the whole presentation. To achieve that, you can pass an array of slide numbers to the **Presentation.save()** method. The following are the steps to convert specific slides in a PPTX to PDF.

*   Load the PPTX presentation using **Presentation** class.
*   Create an array containing slide numbers, e.g. **slides\_numbers=\[ 1, 3 \]**.
*   Convert PPTX to PDF using **Presentation.save(string, slides\_numbers, export.SaveFormat.PDF)** method.

The following code sample converts the specific slides of a presentation to PDF in Python.

{{< gist aspose-com-gists cbc95264bf51d082800eca055e38cc5c "pptx-to-pdf-selected-slides.py" >}}

## Set PDF Compliance in PPT to PDF Conversion {#Set-PDF-Compliance-in-PPT-to-PDF-Conversion}

You can also specify a particular compliance level for the converted PDF document using the **PdfOptions.compliance** property. The following are the steps to achieve that.

*   Load the PPTX presentation using **Presentation** class.
*   Create an object of **PdfOptions** class.
*   Set **PdfOptions.compliance** property using **export.PdfCompliance** enum.
*   Convert PPTX to PDF using **Presentation.save(string, export.SaveFormat.PDF, **PdfOptions**)** method.

The following code sample shows how to specify compliance level in PPTX to PDF conversion in Python.

{{< gist aspose-com-gists cbc95264bf51d082800eca055e38cc5c "pptx-to-pdf-compliance.py" >}}

## Convert PPT to Password-protected PDF in Python {#Convert-PPT-to-Password-protected-PDF}

To ensure the security of the document, PDF supports password protection. Aspose.Slides for Python via .NET also allows you to set a password and specify access permissions for the converted PDF document. The following are the steps to convert a PowerPoint presentation to a password-protected PDF.

*   Load the PPTX presentation using **Presentation** class.
*   Create an object of **PdfOptions** class.
*   Set password using **PdfOptions.password** property.
*   Set access permissions using **PdfOptions.access\_permissions** property.
*   Convert PPTX to PDF using **Presentation.save(string, export.SaveFormat.PDF, PdfOptions)** method.

The following code sample converts a PowerPoint PPTX file to a password-protected PDF.

{{< gist aspose-com-gists cbc95264bf51d082800eca055e38cc5c "pptx-to-password-protected-pdf.py" >}}

## Get a Free License

You can use Aspose.Slides for Python via .NET for free by getting a [temporary license][17].

## Conclusion

In this article, you have learned how to convert PPT or PPTX files to PDF in Python. Furthermore, you have seen how to customize the PowerPoint to PDF conversion using different options in Python. The code samples have demonstrated how to include hidden slides, convert specific slides, specify PDF compliance, and set a password and access permissions for converted PDF. You can explore more about the Python presentation manipulation library using the [documentation][18]. In case you would have any questions, feel free to let us know via our [forum][19].

## See Also

*   [PowerPoint to PDF in C#][20]
*   [PowerPoint to PDF in Java][21]
*   [Create PowerPoint Files in Python][22]
*   [Convert PowerPoint PPT to HTML in Python][23]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/presentation/pptx/
[3]: https://docs.fileformat.com/presentation/ppt/
[4]: https://docs.fileformat.com/pdf/
[5]: https://docs.fileformat.com/presentation/ppt/
[6]: https://docs.fileformat.com/presentation/pptx/
[7]: #Python-PPTX-to-PDF-Converter-Library
[8]: #Convert-a-PowerPoint-PPTX-File-to-PDF
[9]: #Include-Hidden-Slides-in-PPTX-to-PDF-Conversion
[10]: #Convert-Selected-Slides-in-PPTX-to-PDF
[11]: #Set-PDF-Compliance-in-PPT-to-PDF-Conversion
[12]: #Convert-PPT-to-Password-protected-PDF
[13]: https://products.aspose.app/slides/conversion
[14]: https://products.aspose.com/slides/python-net/
[15]: https://pypi.org/project/aspose.slides/
[16]: https://docs.aspose.com/slides/python-net/system-requirements/
[17]: https://purchase.aspose.com/temporary-license
[18]: https://docs.aspose.com/slides/python-net
[19]: https://forum.aspose.com/
[20]: https://blog.aspose.com/2020/02/12/convert-powerpoint-ppt-pptx-to-pdf-in-csharp-net/
[21]: https://blog.aspose.com/2019/12/31/convert-powerpoint-ppt-pptx-to-pdf-in-java-using-aspose-slides/
[22]: https://blog.aspose.com/2021/12/31/create-powerpoint-presentations-in-python/
[23]: https://blog.aspose.com/2021/12/16/convert-ppt-to-html-in-python/




