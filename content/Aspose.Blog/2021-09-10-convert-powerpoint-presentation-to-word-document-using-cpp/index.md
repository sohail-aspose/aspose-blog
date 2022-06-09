---
title: 'Convert PowerPoint Presentation to Word Document using C++'
seoTitle: "Convert PowerPoint Presentation to Word Document using C++"
description: "Convert PowerPoint Presentations to Word documents using C++. Use the C++ APIs to perform the PPTX/PPT to DOCX conversion."
date: Fri, 10 Sep 2021 14:45:39 +0000
draft: false
url: /2021/09/10/convert-powerpoint-presentation-to-word-document-using-cpp/
author: Muhammad Ahmad
summary: 'There may be cases where you have a PowerPoint presentation and want to create a document that describes its contents in detail. For that, you can convert your [PPTX][1]/[PPT][2] files to Word format and modify the Word file to enter the details for each slide. In this article, you will learn **how to convert PowerPoint PPTX/PPT files to Word format programmatically using C++**.'
tags: ['PowerPoint to Word C++', 'ppt to docx c++', 'pptx to docx C++']
categories: ['Aspose.Words Product Family', 'Aspose.Slides Product Family']
---



{{< figure align=center src="images/PPTX-to-DOCX.jpg" alt="Convert PowerPoint Presentation to Word Document using C++">}}


There may be cases where you have a PowerPoint presentation and want to create a document that describes its contents in detail. For that, you can convert your [PPTX][3]/[PPT][4] files to Word format and modify the Word file to enter the details for each slide. In this article, you will learn **how to convert PowerPoint PPTX/PPT files to Word format programmatically using C++**.

*   [C++ API for Converting PowerPoint Files to Word Format][5]
*   [Convert PowerPoint PPTX/PPT Files to DOCX Format using C++][6]

**Note**: You may want to check out Aspose [PowerPoint to Word Converter][7], which is a live implementation of the primary procedure in this article.

## C++ API for Converting PowerPoint Files to Word Format {#CPP-API-for-Converting-PowerPoint-Files-to-Word-Format}

In order to convert PowerPoint presentations to Word documents, we will use the [Aspose.Slides for C++][8] and [Aspose.Words for C++][9] APIs. The former is an API for working with PowerPoint files, whereas the latter is used to create, read and modify Word documents. We will use the Aspose.Slides for C++ API to convert the PowerPoint file to HTML format and the Aspose.Words for C++ API to convert the generated HTML to Word format. You can either install the APIs through NuGet or download them directly from the [Downloads][10] section.

```
PM> Install-Package Aspose.Slides.Cpp
PM> Install-Package Aspose.Words.Cpp
```

## Convert PowerPoint PPTX/PPT Files to DOCX Format using C++ {#Convert-PowerPoint-PPTX-PPT-Files-to-DOCX-Format-using-CPP}

The following are the steps to convert PowerPoint PPTX/PPT Files to DOCX Format using C++.

*   Load the PowerPoint file using the [Aspose::Slides::Presentation][11] class.
*   Create an instance of the [MemoryStream][12] class.
*   Save the presentation to the stream.
*   Create an instance of the [Aspose::Words::Document][13] class using the stream object.
*   Save the DOCX file using the [Aspose::Words::Document->Save(const System::String & fileName, Aspose::Words::SaveFormat saveFormat)][14] method.

The following sample code shows how to convert PowerPoint PPTX/PPT Files to DOCX Format using C++.

{{< gist aspose-com-gists 70bb50b808674e49279057d1f02c3f0c "Convert_PowerPoint_To_Word.cpp" >}}

## Get a Free License

In order to try the API without evaluation limitations, you can request [a free temporary license][15].

## Conclusion

In this article, you have learned how to convert PowerPoint PPTX/PPT files to Word documents using C++. We used the Aspose.Slides for C++ API to convert PPTX/PPT files to HTML format and Aspose.Words for C++ API to convert the generated HTML to DOCX format. To learn more about these APIs, you can visit their official documentation. In case of any queries, please feel free to reach us at our [free support forum][16].

*   [Aspose.Slides for C++ Documentation][17]
*   [Aspose.Words for C++ Documentation][18]

## See Also

*   [Convert PowerPoint PPTX/PPT to TIFF using C++][19]
*   [Convert PowerPoint to PDF using C++][20]




[1]: https://docs.fileformat.com/presentation/pptx/
[2]: https://docs.fileformat.com/presentation/ppt/
[3]: https://docs.fileformat.com/presentation/pptx/
[4]: https://docs.fileformat.com/presentation/ppt/
[5]: #CPP-API-for-Converting-PowerPoint-Files-to-Word-Format
[6]: #Convert-PowerPoint-PPTX-PPT-Files-to-DOCX-Format-using-CPP
[7]: https://products.aspose.app/slides/conversion/ppt-to-word
[8]: https://products.aspose.com/slides/cpp
[9]: https://products.aspose.com/words/cpp/
[10]: https://downloads.aspose.com/total
[11]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[12]: https://apireference.aspose.com/slides/cpp/class/system.i_o.memory_stream
[13]: https://apireference.aspose.com/words/cpp/class/aspose.words.document
[14]: https://apireference.aspose.com/words/cpp/class/aspose.words.document#save_string_saveformat
[15]: https://purchase.aspose.com/temporary-license
[16]: https://forum.aspose.com/
[17]: https://docs.aspose.com/slides/cpp/
[18]: https://docs.aspose.com/words/cpp/
[19]: https://blog.aspose.com/2021/09/08/convert-powerpoint-pptx-ppt-to-tiff-using-cpp/
[20]: https://blog.aspose.com/2021/03/03/convert-powerpoint-to-pdf-using-cpp/




