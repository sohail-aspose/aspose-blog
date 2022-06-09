---
title: 'Lock or Unlock PowerPoint Presentations in Python'
seoTitle: "Lock or Unlock PowerPoint Presentations in Python | Protect PPT/PPTX"
description: "Use Python PowerPoint library to lock or unlock PPT/PPTX presentations in Python. Protect presentations by preventing their editing programmatically."
date: Mon, 27 Dec 2021 13:23:00 +0000
draft: false
url: /2021/12/27/lock-or-unlock-powerpoint-ppt-in-python/
author: Usman Aziz
summary: 'Digital documents are always prone to be tampered with by unauthorized entities. Therefore, various protection mechanisms are used to ensure the security of the documents. In this article, we will particularly target the protection of MS PowerPoint presentations. So you will learn **how to lock and unlock PowerPoint presentations programmatically in Python**.'
tags: ['Lock a PowerPoint Presentation in Python', 'Python Library to Lock PowerPoint Presentations', 'Remove Protection from PowerPoint PPT in Python', 'Unlock a PowerPoint Presentation in Python']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Protect-PowerPoint-Files.jpg" alt="Protect PowerPoint Files in Python">}}


Digital documents are always prone to be tampered with by unauthorized entities. Therefore, various protection mechanisms are used to ensure the security of the documents. In this article, we will particularly target the protection of MS PowerPoint presentations. So you will learn **how to lock and unlock PowerPoint presentations programmatically in Python**.

*   [Python Library to Lock PowerPoint Presentations][1]
*   [Lock a PowerPoint Presentation in Python][2]
*   [Unlock a PowerPoint Presentation in Python][3]

## Python Library to Lock PowerPoint Presentations {#Python-Library-to-Lock-PowerPoint-Presentations}

To lock and unlock PowerPoint presentations, we will use [Aspose.Slides for Python via .NET][4]. The library provides a range of features to create and manipulate PowerPoint presentations. You can install the library in your applications from [PyPI][5] using the following command.

```
> pip install aspose.slides 
```

## Lock a PowerPoint Presentation in Python {#Lock-a-PowerPoint-Presentation-in-Python}

A PowerPoint presentation may contain a variety of elements such as text, images, shapes, audio, etc. Aspose.Slides for Python represents each element as a Shape or an abject derived from Shape. So in order to protect the content from being edited, we need to lock all the shapes in the presentation. These shapes could be of the following types:

*   Auto Shape
*   Group Shape
*   Connector
*   Picture Frame

Let's see how to lock a PowerPoint PPTX file in Python.

*   First, load the presentation file using **Presentation** class.
*   Then, get reference of slides in the presentation using **Presentation.slides** property.
*   For each slide, access its shapes using **ISlide.shapes** collection.
*   For each shape in the collection, perform the following steps:
    *   Check type of the shape.
    *   Use appropriate lock according to type of the shape.
*   Finally, save the updated presentation using **Presentation.save(string, SaveFormat)** method.

The following code sample shows how to protect a presentation by locking its shapes in Python.

{{< gist aspose-com-gists 091486327848348c105b79e1bf2b16a7 "lock-ppt.py" >}}

## Unlock PowerPoint Presentations in Python {#Remove-Protection-from-PowerPoint-PPT-in-Python}

To unlock a PowerPoint presentation, you need to remove the locks from each shape. Please note that if you have locked the presentation using Aspose.Slides for Python then you will have to use the same library for unlocking. To remove the locks, repeat the steps mentioned in the previous section and set lock values to false.

The following code sample shows how to unlock a PPTX presentation in Python.

{{< gist aspose-com-gists 091486327848348c105b79e1bf2b16a7 "unlock-ppt.py" >}}

## Get a Free License

Use Aspose.Slides for Python via .NET without evaluation limitations by getting a [free temporary license][6].

## Conclusion

Protection of digital documents has become essential to avoid the tampering of the content. Therefore, the documents are protected before they are shared over the internet. Accordingly, this article covered how to lock PowerPoint presentations programmatically in Python. Furthermore, you have seen how to unprotect the presentations by unlocking their elements. Apart from that, you can explore more about Aspose.Slides for Python by visiting the [documentation][7]. Also, you can post your queries to our [forum][8].

## See Also

*   [Create PowerPoint Files in Python][9]
*   [Convert PPTX to PDF in Python][10]
*   [Convert PPT to PNG in Python][11]
*   [PPT/PPTX to HTML in Python][12]




[1]: #Python-Library-to-Lock-PowerPoint-Presentations
[2]: #Lock-a-PowerPoint-Presentation-in-Python
[3]: #Remove-Protection-from-PowerPoint-PPT-in-Python
[4]: https://products.aspose.com/slides/python-net
[5]: https://pypi.org/project/aspose.slides/
[6]: https://purchase.aspose.com/temporary-license
[7]: https://docs.aspose.com/slides/python-net
[8]: https://forum.aspose.com/
[9]: https://blog.aspose.com/2021/12/31/create-powerpoint-presentations-in-python/
[10]: https://blog.aspose.com/2021/12/28/convert-pptx-ppt-to-pdf-python/
[11]: https://blog.aspose.com/2021/12/29/convert-ppt-to-png-in-python/
[12]: https://blog.aspose.com/2021/12/16/convert-ppt-to-html-in-python/




