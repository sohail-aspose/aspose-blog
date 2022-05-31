---
title: 'Work with VBA Macros in PowerPoint PPT/PPTX in Python'
date: Mon, 21 Feb 2022 15:11:00 +0000
draft: false
url: /2022/02/21/work-with-vba-macros-in-powerpoint-in-python/
author: 'Usman Aziz'
summary: 'VBA macros allow you to automate various types of operations in PowerPoint presentations. You can use them for generating charts, unhiding the hidden objects, and performing different repetitive tasks in the presentations. While working with PowerPoint presentations from within your Python applications, you may need to manipulate VBA macros. Therefore, in this article, you will learn **how to add, extract and remove VBA Macros in PowerPoint using Python**.'
tags: ['Add VBA Macros in a PowerPoint Presentation Python', 'Extract VBA Macros from a Presentation Python', 'Python Library to Work with PowerPoint VBA Macros', 'Remove VBA Macros from a Presentation Python']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Add-Remove-VBA-Module.jpg" alt="PPTX in Python">}}


VBA macros allow you to automate various types of operations in PowerPoint presentations. You can use them for generating charts, unhiding the hidden objects, and performing different repetitive tasks in the presentations. While working with PowerPoint presentations from within your Python applications, you may need to manipulate VBA macros. Therefore, in this article, you will learn **how to add, extract and remove VBA Macros in PowerPoint using Python**.

*   [Python Library to Work with VBA Macros][1]
*   [Add VBA Macros in a PowerPoint Presentation][2]
*   [Extract VBA Macros from a Presentation][3]
*   [Remove VBA Macros from a Presentation][4]

## Python Library to Work with VBA Macros in PowerPoint {#Library-for-VBA-Macros-in-PowerPoint}

To work with VBA macros in PowerPoint presentations, we will use [Aspose.Slides for Python][5]. The library provides a rich set of features to create, edit and convert PowerPoint presentations. You can install the library from [PyPI][6] using the following command.

```
> pip install aspose.slides
```

## Add VBA Macro in PowerPoint Presentations in Python {#Add-VBA-Macros-in-PowerPoint-Presentations}

The following are the steps to add a VBA macro in a PowerPoint presentation using Python.

*   First, use **Presentation** class to load or create the PowerPoint presentation.
*   Then, create a new **VbaProject** and assign it to **Presentation.vba\_project** property.
*   After that, add an empty VBA module using **Presentation.vba\_project.modules.add\_empty\_module(string)** method.
*   Add source code to the VBA module using **IVbaModule.source\_code** property.
*   Associate the references and add them to **Presentation.vba\_project.references** collection.
*   Finally, save the presentation file using **Presentation.save(string, SaveFormat.PPTM)** method.

The following code sample shows how to add VBA macro in a PowerPoint presentation using Python.

{{< gist aspose-com-gists 41f3b1d61a73dadd899491b6e0e6af2b "add-vba-macro-in-powerpoint.py" >}}

## Extract VBA Macros from PowerPoint in Python {#Extract-VBA-Macros-in-PowerPoint-Presentations}

You can also access VBA macros added to a PowerPoint presentation and extract their information. The following steps demonstrate how to extract VBA macros and print their name and source code in Python.

*   First, load the macro-enabled presentation using the **Presentation** class.
*   Then, check if presentation contains the VBA projects using **Presentation.vba\_project** property.
*   Access each VBA module in **Presentation.vba\_project.modules** collection.
*   Finally, extract source code and name of VBA module.

The following code sample shows how to extract PowerPoint VBA macros in Python.

{{< gist aspose-com-gists 41f3b1d61a73dadd899491b6e0e6af2b "extract-vba-macro-in-powerpoint.py" >}}

## Remove VBA Macros from a PowerPoint Presentation {#Remove-VBA-Macros-in-PowerPoint-Presentations}

To remove a VBA macro, you need to access it using its index. Once you have the macro's reference, you can remove it from the collection. The following are the steps to remove a VBA macro from a PowerPoint presentation.

*   First, load the macro-enabled PowerPoint presentation using the **Presentation** class.
*   Then, remove VBA macro using **Presentation.vba\_project.modules.remove(Presentation.vba\_project.modules\[index\])** method.
*   Finally, save the updated presentation using **Presentation.save(string, SaveFormat.PPTM)** method.

The following code sample shows how to remove a VBA macro in Python.

{{< gist aspose-com-gists 41f3b1d61a73dadd899491b6e0e6af2b "remove-vba-macro-in-powerpoint.py" >}}

## Get a Free License {#Get-a-Free-API-License}

You can use Aspose.Slides for Python without evaluation limitations by getting a [free temporary license][7].

## Conclusion

In this article, you have learned how to work with VBA macros in PowerPoint presentations using Python. With the help of code samples, we have demonstrated how to add, extract and remove VBA macros in PowerPoint presentations. In addition, you may visit the [documentation][8] to explore more about Aspose.Slides for Python. Also, you can ask your question and queries via our [forum][9].

## See Also

*   [Create PowerPoint Files in Python][10]
*   [Convert PPTX to PDF in Python][11]
*   [Convert PPT to PNG in Python][12]
*   [Add Watermark in PowerPoint PPT in Python][13]
*   [Apply 3D Effects in PowerPoint PPT using Python][14]




[1]: #Library-for-VBA-Macros-in-PowerPoint
[2]: #Add-VBA-Macros-in-PowerPoint-Presentations
[3]: #Extract-VBA-Macros-in-PowerPoint-Presentations
[4]: #Remove-VBA-Macros-in-PowerPoint-Presentations
[5]: https://products.aspose.com/slides/python-net
[6]: https://pypi.org/project/aspose.slides/
[7]: https://purchase.aspose.com/temporary-license
[8]: https://docs.aspose.com/slides/python-net/
[9]: https://forum.aspose.com/
[10]: https://blog.aspose.com/2021/12/31/create-powerpoint-presentations-in-python/
[11]: https://blog.aspose.com/2021/12/28/convert-pptx-ppt-to-pdf-python/
[12]: https://blog.aspose.com/2021/12/29/convert-ppt-to-png-in-python/
[13]: https://blog.aspose.com/2022/02/09/add-watermark-to-powerpoint-ppt-in-python/
[14]: https://blog.aspose.com/2022/01/08/create-three-d-effects-in-ppt-python/




