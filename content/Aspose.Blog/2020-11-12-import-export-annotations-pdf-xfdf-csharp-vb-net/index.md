---
title: 'Import or Export Annotations from PDF to XFDF using C# VB.NET'
seoTitle: "Import or Export Annotations from PDF to XFDF using C# VB.NET"
description: "Import or Export Annotations from PDF or XFDF files Programmatically using C# or VB.NET in your .NET framework based applications."
date: Thu, 12 Nov 2020 00:56:26 +0000
draft: false
url: /2020/11/12/import-export-annotations-pdf-xfdf-csharp-vb-net/
author: Farhan Raza
summary: 'Annotations are often used to add clarifications, explanations, details, or comments to some documents. In PDF files, annotations are frequently used and you might need to import or export them to XFDF format. You can easily import or export annotations programmatically using C# or VB.NET.'
tags: ['Export annotations', 'Import annotations', 'PDF to XFDF', 'XFDF to PDF']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/import-export-annotations-pdf-xfdf-1.png" alt="import export pdf xfdf annotations">}}


Annotations are often used to add clarifications, explanations, details, or comments to some documents. In [PDF][1] files, annotations are frequently used and you might need to import or export them to XFDF format. You can easily import or export annotations programmatically using [C#][2] or [VB.NET][3]. Let us go through the following contents:

*   [Annotations Importer or Exporter API – Installation][4]
*   [Import Annotations from XFDF to PDF using C# or VB.NET][5]
*   [Export Annotations from PDF to XFDF using C# or VB.NET][6]

## Annotations Importer or Exporter API – Installation {#section1}

[Aspose.PDF for .NET][7] API exposes different classes, properties, and methods to work with PDF files. Likewise, you can import or export annotations from PDF documents to the [XFDF][8] file with [PDFAnnotationEditor][9] class. It exposes different methods that can be used to import or export annotations programmatically. You need to install the API by downloading it from [New Releases][10], or via NuGet solution manager in Microsoft Visual Studio IDE. The following command can be used to install the API:

```
PM> Install-Package Aspose.Pdf
```

## Import Annotations from XFDF to PDF using C# or VB.NET {#section2}

You can import annotations into PDF file from existing XFDF file in your .NET based applications using C# or VB.NET programming languages. The API supports importing different types of annotations as listed under the [AnnotationType][11] Enumeration in API references. Let us follow the following steps to import annotations from XFDF to PDF using C# or VB.NET programming languages in your .NET framework based applications.

1.  Initialize [PdfAnnotationEditor][12] class object
2.  Load the input PDF document
3.  Load the XFDF file to import annotations
4.  Specify the annotation types that you want to import
5.  Import annotations from XFDF to PDF file
6.  Save the output PDF file

The code snippet below shows how to import annotations from XFDF file to PDF file using C# or VB.NET:

{{< gist aspose-com-gists f9cb92721e6cb98cbed3f2bc3bac72a5 "ImportAnnotationsPDF.cs" >}}

## Export Annotations from PDF to XFDF File using C# or VB.NET {#section3}

Exporting of annotations from PDF files can be helpful for making the file presentable or for keeping intact only a specific type of annotations. For example, when someone is reviewing a feasibility report or a thesis submission, let us assume, they may highlight some text, add comments or text. Later they want to keep only the text before sending the PDF back to the author. In such scenarios, exporting of annotations to XFDF can help because it lets you export specific annotations as per your requirements. The following steps show how to export annotations from PDF to XFDF format:

1.  Initialize [PdfAnnotationEditor][13] object
2.  Load input PDF file
3.  Create XFDF file to save exported annotations
4.  Specify annotation type to Export
5.  Export the annotations with the [ExportAnnotationsXfdf][14] method

The code snippet below shows how to export annotations from PDF file to XFDF file using C# or VB.NET:

{{< gist aspose-com-gists f9cb92721e6cb98cbed3f2bc3bac72a5 "ExportAnnotationsPDF.cs" >}}

## Conclusion

In this article, we have explored how to import and export annotations from PDF to XFDF format. We have explored different examples and scenarios where importing or exporting the annotations can be helpful. Likewise, there are many use cases and scenarios where this feature is valuable. If you want to discuss any scenario then feel free to contact us at [Free Support Forum][15]. You can also explore the API by learning from [API Documentation][16] as well as [API References][17]. We look forward to hearing from you!

## See Also

[Rotate PDF Pages, the Text or Image with C# or VB.NET][18]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/programming/cs/
[3]: https://docs.fileformat.com/programming/vb/
[4]: #section1
[5]: #section2
[6]: #section3
[7]: https://products.aspose.com/pdf/net
[8]: https://docs.fileformat.com/pdf/x/
[9]: https://apireference.aspose.com/pdf/net/aspose.pdf.facades/pdfannotationeditor
[10]: https://releases.aspose.com/
[11]: https://apireference.aspose.com/pdf/net/aspose.pdf.annotations/annotationtype
[12]: https://apireference.aspose.com/pdf/net/aspose.pdf.facades/pdfannotationeditor
[13]: https://apireference.aspose.com/pdf/net/aspose.pdf.facades/pdfannotationeditor
[14]: https://apireference.aspose.com/pdf/net/aspose.pdf.facades/pdfannotationeditor/methods/exportannotationsxfdf/index
[15]: https://forum.aspose.com/c/pdf
[16]: https://docs.aspose.com/pdf/net/
[17]: https://apireference.aspose.com/pdf/net
[18]: https://blog.aspose.com/2020/10/18/rotate-pdf-text-image-page-with-csharp-vb-net/





