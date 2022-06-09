---
title: 'Convert PowerPoint PPT to HTML in Python'
seoTitle: "Convert PowerPoint PPT to HTML in Python | Python PPTX Library"
description: "Use Python PowerPoint library to convert PPT or PPTX to HTML with high fidelity. Export PPT to responsive HTML and include slide notes in HTML."
date: Thu, 16 Dec 2021 07:08:00 +0000
draft: false
url: /2021/12/16/convert-ppt-to-html-in-python/
author: Usman Aziz
summary: 'In various cases, you have to convert the slides in PowerPoint presentations to [HTML][1]. For example, to view in browser, to index the content, etc. In this article, you will learn **how to convert PowerPoint [PPT][2] or [PPTX][3] to HTML in Python**. Moreover, we will cover how to convert PPT to responsive HTML and include slides notes in resultant HTML pages.'
tags: ['Convert a PPT to HTML in Python', 'Include Slide Notes in PPT to HTML Python', 'Python PPT to HTML Converter', 'Python PPT to Responsive HTML']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/PPTX-to-HTML-1.jpg" alt="Convert PPT to HTML in Python">}}


In various cases, you have to convert the slides in PowerPoint presentations to [HTML][4]. For example, to view in browser, to index the content, etc. In this article, you will learn **how to convert PowerPoint [PPT][5] or [PPTX][6] to HTML in Python**. Moreover, we will cover how to convert PPT to responsive HTML and include slide notes in resultant HTML pages.

*   [Python PowerPoint to HTML Converter][7]
*   [Convert a PowerPoint PPT to HTML][8]
*   [Convert PPT to Responsive HTML][9]
*   [Include Slide Notes in PPT to HTML][10]

**Info**: Aspose provides a free [PowerPoint to HTML][11] conversion service, which is a live implementation of the presentation to HTML conversion process.

## Python PowerPoint PPT to HTML Converter {#Python-PPT-to-HTML-Converter}

[Aspose.Slides for Python via .NET][12] is a powerful Python library that provides a wide range of presentation manipulation features. You can create new presentations from scratch or manipulate the existing ones seamlessly without MS Office. In addition, it provides a high fidelity conversion of PPT/PPTX to other formats. We will use this library to convert PPT to HTML. You can install it in your Python application from [PyPI][13] using the following command.

```
> pip install aspose.slides
```

## Convert a PowerPoint PPT/PPTX to HTML in Python {#Convert-a-PPT-to-HTML}

The following are the steps to convert a PowerPoint PPT to HTML in Python.

*   Load the PPT (or PPTX) file using [Presentation][14] class.
*   Convert PPT to HTML using **Presentation.save(string, export.SaveFormat.HTML)** method.

The following code sample shows how to convert a PowerPoint PPTX file to HTML in Python.

{{< gist aspose-com-gists 223609d1fb2c102aac36f1c4707834bb "ppt-to-html.py" >}}

The following is the HTML page that we get after converting a PPT having two slides.



{{< figure align=center src="images/pptx-to-html.jpg" alt="Converting a PowerPoint PPT to HTML in Python">}}


## Convert PPT or PPTX to Responsive HTML in Python {#Convert-PPT-to-Responsive-HTML}

You can also convert a PPT file to responsive HTML so that it appears properly on different browsers and screen sizes. The following are the steps to achieve this.

*   Load the PPT (or PPTX) file using [Presentation][15] class.
*   Create an object of [HtmlOptions][16] class.
*   Create an object of [ResponsiveHtmlController][17] class.
*   Assign controller to **HtmlOptions.html\_formatter** property.
*   Convert PPT to HTML using **Presentation.save(string, export.SaveFormat.HTML, HtmlOptions)** method.

The following code sample shows how to convert a PPTX to responsive HTML in Python.

{{< gist aspose-com-gists 223609d1fb2c102aac36f1c4707834bb "ppt-to-responsive-html.py" >}}

The following screenshot shows how the converted HTML appears on a mobile screen.



{{< figure align=center src="images/ppt-to-responsive-html.png" alt="Conversion of PowerPoint PPTX to responsive HTML">}}


## Include Slide Notes in PowerPoint to HTML Conversion {#Include-Slide-Notes-in-PPT-to-HTML}

By default, the slide notes are not included in the converted HTML pages. However, if you want to include them, you can do it by assigning a value from [export.NotesPositions][18] enum to **HtmlOptions.notes\_comments\_layouting.notes\_position** property. The following code sample shows how to include slide notes at bottom of the HTML pages.

{{< gist aspose-com-gists 223609d1fb2c102aac36f1c4707834bb "ppt-to-html-slide-notes.py" >}}

The following screenshot shows how the slide notes appear on the converted HTML page.



{{< figure align=center src="images/ppt-to-html-slide-notes.png" alt="Rendering Slides Notes in PPT to HTML in Python">}}


## Get a Free License

You can use Aspose.Slides for Python via .NET without evaluation limitations by getting a [temporary license][19].

## Conclusion

In this article, you have learned how to convert PowerPoint PPT or PPTX to HTML in Python. Furthermore, we have seen how to convert a presentation to responsive HTML and include slide notes in the resultant HTML pages. You can read more about Aspose.Slides for Python via .NET using the [documentation][20]. In case of any questions, reach us at our [forum][21].

## See Also

*   [Convert PPTX to PDF in Python][22]
*   [Convert PPT to PNG in Python][23]




[1]: https://docs.fileformat.com/web/html/
[2]: https://docs.fileformat.com/presentation/ppt/
[3]: https://docs.fileformat.com/presentation/pptx/
[4]: https://docs.fileformat.com/web/html/
[5]: https://docs.fileformat.com/presentation/ppt/
[6]: https://docs.fileformat.com/presentation/pptx/
[7]: #Python-PPT-to-HTML-Converter
[8]: #Convert-a-PPT-to-HTML
[9]: #Convert-PPT-to-Responsive-HTML
[10]: #Include-Slide-Notes-in-PPT-to-HTML
[11]: https://products.aspose.app/slides/conversion/ppt-to-html
[12]: https://products.aspose.com/slides/python-net/
[13]: https://pypi.org/project/aspose.slides/
[14]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides/presentation/
[15]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides/presentation/
[16]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides.export/htmloptions/
[17]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides.export/responsivehtmlcontroller/
[18]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides.export/notespositions/
[19]: https://purchase.aspose.com/temporary-license
[20]: https://docs.aspose.com/slides/python-net
[21]: https://forum.aspose.com/
[22]: https://blog.aspose.com/2021/12/28/convert-pptx-ppt-to-pdf-python/
[23]: https://blog.aspose.com/2021/12/29/convert-ppt-to-png-in-python/




