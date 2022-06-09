---
title: 'Add Digital Signature to PowerPoint PPT in Python'
seoTitle: "Python: Add Digital Signature in PowerPoint PPT | Verify Digital Signatures"
description: "Use Python PowerPoint library to add a digital signature to PPT or PPTX in Python. Verify digitally signed PPT to check if the content is modified."
date: Fri, 21 Jan 2022 09:46:15 +0000
draft: false
url: /2022/01/21/add-digital-signature-to-ppt-in-python/
author: Usman Aziz
summary: 'The [digital signature][1] is a well-known and commonly used way of protecting digital documents. It makes it easier to validate the authenticity of the content in a document. Thus, you can identify if someone attempted to tamper with the document. MS PowerPoint also allows you to sign the [PPT][2] or [PPTX][3] presentations with digital signatures. To automate this feature programmatically, this article covers **how to add digital signatures to PowerPoint PPT files in Python**.'
tags: ['Add Digital Signature to PPT in Python', 'Add Digital Signature to PowerPoint in Python', 'Python Library to Digitally Sign PowerPoint Files', 'Verify a Digitally Signed PPT in Python']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Add-and-Verify-Digital-Signatures-to-PPT.png" alt="">}}


The [digital signature][4] is a well-known and commonly used way of protecting digital documents. It makes it easier to validate the authenticity of the content in a document. Thus, you can identify if someone attempted to tamper with the document. MS PowerPoint also allows you to sign the [PPT][5] or [PPTX][6] presentations with digital signatures. To automate this feature programmatically, this article covers **how to add digital signatures to PowerPoint PPT files in Python**.

*   [Python Library to Digitally Sign PowerPoint Files][7]
*   [Add Digital Signature to PPT in Python][8]
*   [Verify a Digitally Signed PPT][9]

## Python Library to Digitally Sign PowerPoint PPT {#Python-Library-to-Digitally-Sign-PowerPoint-Files}

To add digital signatures in PowerPoint presentations, we will use [Aspose.Slides for Python via .NET][10]. It is a powerful Python library that allows you to create and manipulate PowerPoint presentations without writing complex code. You can install the library from [PyPI][11] using the following pip command.

```
> pip install aspose.slides 
```

## Add Digital Signature to PPT in Python {#Add-Digital-Signature-to-PPT-in-Python}

To sign a document with a digital signature, you first need to obtain a certificate from an authorized organization/person known as a certificate authority. This certificate is used to uniquely identify the person who owns it.

Once you have the digital certificate, you can follow the below steps to add digital signatures to a PowerPoint PPT in Python.

*   First, open the PPT/PPTX using [Presentation][12] class.
*   Then, load the digital signature using [DigitalSignature][13] class by providing file's path and password.
*   Add comments using **DigitalSignature.comments** property.
*   Add digital signature to presentation using [Presentation.digital\_signatures.add(DigitalSignature)][14] method.
*   Finally, save the presentation using **Presentation.save(string, SaveFormat)** method.

The following code sample shows how to add a digital signature to a PowerPoint PPT in Python.

{{< gist aspose-com-gists e85c3aff6d89f31923cc608394e28090 "add-digital-signature-ppt.py" >}}

## Verify a Digitally Signed PPT in Python {#Verify-a-Digitally-Signed-PPT}

Aspose.Slides also allows you to verify if a digitally signed PPT is modified or not. The following are the steps to validate digital signatures in a PowerPoint presentation in Python.

*   First, open the PPT/PPTX using [Presentation][15] class.
*   Then, check if PPT is digitally signed or not.
*   For each digital signature in **Presentation.digital\_signatures** collection, perform following steps.
    *   Use **DigitalSignature.is\_valid** to validate the signature.
    *   If it returns false, the presentation is modified otherwise it is not.

The following code sample shows how to validate digital signatures in a PowerPoint PPT in Python.

{{< gist aspose-com-gists e85c3aff6d89f31923cc608394e28090 "verify-digital-signature-ppt.py" >}}

## Get a Free License

You can get a [free temporary license][16] to use Aspose.Slides for Python via .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to add digital signatures to PowerPoint PPT or PPTX files in Python. Moreover, you have seen how to validate the digital signatures to check if the presentation is modified or not. You can explore other features of Aspose.Slides for Python using the [documentation][17]. Also, you can ask your questions on our [forum][18].

## See Also

*   [Create PowerPoint Files in Python][19]
*   [Convert PPTX to PDF in Python][20]
*   [Convert PPT to PNG in Python][21]
*   [PPT/PPTX to HTML in Python][22]




[1]: https://en.wikipedia.org/wiki/Digital_signature
[2]: https://docs.fileformat.com/presentation/ppt/
[3]: https://docs.fileformat.com/presentation/pptx/
[4]: https://en.wikipedia.org/wiki/Digital_signature
[5]: https://docs.fileformat.com/presentation/ppt/
[6]: https://docs.fileformat.com/presentation/pptx/
[7]: #Python-Library-to-Digitally-Sign-PowerPoint-Files
[8]: #Add-Digital-Signature-to-PPT-in-Python
[9]: #Verify-a-Digitally-Signed-PPT
[10]: https://products.aspose.com/slides/python-net
[11]: https://pypi.org/project/aspose.slides/
[12]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides/presentation/
[13]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides/digitalsignature/
[14]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides/idigitalsignaturecollection/
[15]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides/presentation/
[16]: https://purchase.aspose.com/temporary-license
[17]: https://docs.aspose.com/slides/python-net
[18]: https://forum.aspose.com/
[19]: https://blog.aspose.com/2021/12/31/create-powerpoint-presentations-in-python/
[20]: https://blog.aspose.com/2021/12/28/convert-pptx-ppt-to-pdf-python/
[21]: https://blog.aspose.com/2021/12/29/convert-ppt-to-png-in-python/
[22]: https://blog.aspose.com/2021/12/16/convert-ppt-to-html-in-python/




