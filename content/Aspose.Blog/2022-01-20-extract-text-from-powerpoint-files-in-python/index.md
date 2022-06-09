---
title: 'Extract Text from PowerPoint Files in Python'
seoTitle: "Extract Text from PowerPoint Files in Python | Python Text Extractor Library"
description: "Use Python PowerPoint library to extract text from PPT or PPTX files in Python. Extract text from a specific slide or all the slides in the presentation."
date: Thu, 20 Jan 2022 14:40:51 +0000
draft: false
url: /2022/01/20/extract-text-from-powerpoint-files-in-python/
author: Usman Aziz
summary: 'In various scenarios, the text is extracted from the documents for further processing such as in text analysis, classification, etc. Among other documents such as PDF and Word, PowerPoint files are also used in text extraction. Therefore, this article aims to show you **how to extract text from PowerPoint files in Python**. We will cover how to extract text from a specific slide or the whole presentation.'
tags: ['Extract Text from PowerPoint Files', 'Extract Text from a PowerPoint Slide Python', 'Python Library to Extract Text from PowerPoint Files', 'Python Text Extractor for PowerPoint']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Extract-Text-from-PowerPoint.jpg" alt="Extract Text from PowerPoint Files in Python">}}


In various scenarios, the text is extracted from the documents for further processing such as in text analysis, classification, etc. Among other documents such as PDF and Word, PowerPoint files are also used in text extraction. Therefore, this article aims to show you **how to extract text from PowerPoint files in Python**. We will cover how to extract text from a specific slide or the whole presentation.

*   [Python Library to Extract Text from PowerPoint Files][1]
*   [Extract Text from PowerPoint Files][2]
    *   [Extract Text from a Slide][3]
    *   [Text Extraction from a Presentation][4]

## Python Library to Extract Text from PowerPoint Files {#Python-Library-to-Extract-Text-from-PowerPoint-Files}

To extract text from PowerPoint files, we will use [Aspose.Slides for Python via .NET][5]. It is a feature-rich Python library to create and update PowerPoint presentations. Furthermore, it allows you to manipulate and convert the presentations seamlessly. You can install this library from [PyPI][6] using the following pip command.

```
> pip install aspose.slides 
```

## Extract Text from PowerPoint Files in Python {#Extract-Text-from-PowerPoint-Files}

Depending upon the scenario, you may need to extract text either from the whole PowerPoint presentation or some specific slide(s). In the following sections, we will demonstrate how to perform text extraction in both of the above-mentioned cases. So let's proceed.

### Extract Text from a Specific Slide {#Extract-Text-from-a-Slide}

The following are the steps to extract text from a specific slide in PPT in Python.

*   First, use [PresentationFactory().get\_presentation\_text(string, TextExtractionArrangingMode)][7] method to get all types of text in the presentation.
*   After that, use index to extract text of a sepcific slide from **slides\_text** array.
*   The following are the types of text you can extract:
    
    *   Slide's Text
    *   Notes
    *   Slide layout text
    
    *   Slide master text

The following code sample shows how to extract text from a specific PPT slide in Python.

{{< gist aspose-com-gists 58a8371b5bb52eff43b8bd441c67e412 "extract-text-from-slide.py" >}}

### Text Extraction from Whole PowerPoint File in Python {#Text-Extraction-from-a-Presentation}

The following steps demonstrate how to extract text from all the slides of a PowerPoint presentation.

*   First, use [PresentationFactory().get\_presentation\_text(string, TextExtractionArrangingMode)][8] method to get all types of text in presentation.
*   Load presentation in a [Presentation][9] object.
*   Iterate through the number of slides in the presentation.
*   Extract text from each slide using **slides\_text** array.

The following code sample shows how to extract text from a PPTX (or PPT) file in Python.

{{< gist aspose-com-gists 58a8371b5bb52eff43b8bd441c67e412 "extract-text-from-presentation.py" >}}

## Get a Free License

You can use Aspose.Slides for Python via .NET without evaluation limitations by getting a [temporary license][10].

## Conclusion

In this article, you have learned how to extract text from PowerPoint files in Python. You have seen how to extract text from a specific slide or all the slides in a PowerPoint presentation. Besides, you can explore other features of Aspose.Slides for Python using the [documentation][11]. Also, you can share your queries with us via our [forum][12].

## See Also

*   [Create PowerPoint Files in Python][13]
*   [Convert PPTX to PDF in Python][14]
*   [Convert PPT to PNG in Python][15]
*   [PPT/PPTX to HTML in Python][16]




[1]: #Python-Library-to-Extract-Text-from-PowerPoint-Files
[2]: #Extract-Text-from-PowerPoint-Files
[3]: #Extract-Text-from-a-Slide
[4]: #Text-Extraction-from-a-Presentation
[5]: https://products.aspose.com/slides/python-net
[6]: https://pypi.org/project/aspose.slides/
[7]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides/presentationfactory/
[8]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides/presentationfactory/
[9]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides/presentation/
[10]: https://purchase.aspose.com/temporary-license
[11]: https://docs.aspose.com/slides/python-net
[12]: https://forum.aspose.com/
[13]: https://blog.aspose.com/2021/12/31/create-powerpoint-presentations-in-python/
[14]: https://blog.aspose.com/2021/12/28/convert-pptx-ppt-to-pdf-python/
[15]: https://blog.aspose.com/2021/12/29/convert-ppt-to-png-in-python/
[16]: https://blog.aspose.com/2021/12/16/convert-ppt-to-html-in-python/




