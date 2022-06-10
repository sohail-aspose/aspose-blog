---
title: 'Convert PowerPoint PPT/PPTX to PDF using Python'
date: Sun, 24 Apr 2016 05:22:00 +0000
draft: false
url: /2016/04/24/convert-powerpoint-to-pdf-using-python/
author: Fahad Adeel
summary: 'In this article, you will learn **how to convert PowerPoint PPT/PPTX presentations using Python**. For this, we will use “Aspose.Slides Java for Python”, a new project for Python developers. The project is aimed to provide useful examples for [Python][1] developers who want to utilize [Aspose.Slides for Java API][2] in their Python applications to create and manipulate PowerPoint presentations.'
tags: ['powerpoint to pdf python', 'ppt to pdf python', 'pptx to pdf python']
categories: ['Aspose.Slides Product Family']
---

In this article, you will learn **how to convert PowerPoint PPT/PPTX presentations using Python**. For this, we will use “Aspose.Slides Java for Python”, a new project for Python developers. The project is aimed to provide useful examples for [Python][3] developers who want to utilize [Aspose.Slides for Java API][4] in their Python applications to create and manipulate PowerPoint presentations.

## Python PowerPoint PPTX/PPT to PDF Converter

Please check the links below to find instructions on downloading, installing, and using Aspose.Slides Java for Python.

*   [Downloads and Installation][5]

OR

You can download the latest version from:

*   [Pypi][6]
*   [CodePlex][7]
*   [GitHub][8]

**Note:** Aspose provides a simple, [free online PowerPoint editor.][9]

## Convert PowerPoint PPTX/PPT to PDF in Python

The following steps show how to convert a PowerPoint PPTX/PPT presentation to PDF using Python:

*   Load a presentation using Presentation class.
*   Specify the output format as PDF.
*   Convert presentation to PDF using Presentation.save() method.

The following code sample shows how to convert a PowerPoint presentation to PDF.

```
# Instantiate a Presentation object that represents a PPTX file
pres = self.Presentation(self.dataDir + "Aspose.pptx")
# Saving the PPTX presentation to Pdf format
save_format = self.SaveFormat
pres.save(self.dataDir + "Aspose.pdf", save_format.Pdf)
print "Document has been converted, please check the output file.
```

## Learn More

[Aspose.Slides Java for Python Documentation][10] is available to guide developers to get familiar with the specific resources and operations within the Aspose.Slides Java for Python.

## Get a Free API License {#Get-a-Free-API-License}

You can [get a free temporary license][11] in order to use the API without evaluation limitations.

## Conclusion

IIn this article, you have learned how to convert the PowerPoint PPTX or PPT presentations to PDF using Python. You can simply install the API and integrate the provided code sample to enrich your Python applications with PPTX/PPT to PDF conversion.

## See Also

[Create, Edit, Convert PowerPoint PPT/PPTX using Python][12]




[1]: http://www.python.org/
[2]: https://products.aspose.com/slides/java
[3]: http://www.python.org/
[4]: https://products.aspose.com/slides/java
[5]: http://docs.aspose.com/display/slidesjava/Aspose.Slides+Java+for+Python
[6]: https://pypi.python.org/pypi/aspose-slides-java-for-python/1.0
[7]: https://docs.aspose.com/
[8]: https://github.com/asposeslides/Aspose_Slides_Java/releases/tag/Aspose.Slides_Java_for_Python-v1.0
[9]: https://products.aspose.app/slides/editor
[10]: http://docs.aspose.com/display/slidesjava/Aspose.Slides+Java+for+Python
[11]: https://purchase.aspose.com/temporary-license
[12]: https://blog.aspose.com/2016/04/24/python-code-examples-to-deal-with-presentation-documents-using-aspose.slides-for-java




