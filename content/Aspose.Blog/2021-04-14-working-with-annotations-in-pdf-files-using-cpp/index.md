---
title: 'Working with Annotations in PDF Files using C++'
seoTitle: "Working with Annotations in PDF Files using C++ | PDF Annotation C++"
description: "Working with annotations in PDF documents using C++. Read, add, update and delete annotations from PDF documents within your C++ applications."
date: Wed, 14 Apr 2021 09:52:20 +0000
draft: false
url: /2021/04/14/working-with-annotations-in-pdf-files-using-cpp/
author: Muhammad Ahmad
summary: 'Annotations are additional objects that can be added to [PDF][1] documents. Annotations can be helpful in scenarios such as adding contextual information to the document. As PDF files are not easily editable, annotations provide an option to add additional information to the document. In this article, you will learn **how to work with annotations in PDF files using C++**.'
tags: ['Add Annotation to PDF File C++', 'Modify Annotation in PDF File C++', 'Read Annotations in PDF Files C++', 'Remove Annotations from PDF File C++']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Add-or-Remove-Annotation-in-PDF-2.jpg" alt="Working with Annotations in PDF Files using C++">}}


Annotations are additional objects that can be added to [PDF][2] documents. Annotations can be helpful in scenarios such as adding contextual information to the document. As PDF files are not easily editable, annotations provide an option to add additional information to the document. In this article, you will learn **how to work with annotations in PDF files using [C++][3]**.

*   [C++ API for Working with Annotations in PDF Files][4]
*   [Read Annotations in PDF Files][5]
*   [Add Annotations to PDF Files][6]
*   [Modify Annotations in PDF Files using C++][7]
*   [Remove Annotations from PDF Files][8]
*   [Get a Free License][9]

## C++ API for Working with Annotations in PDF Files {#CPP-API-for-Working-with-Annotations-in-PDF-Files}

[Aspose.PDF for C++][10] is a C++ library that allows you to create, read and update PDF documents. Furthermore, the API supports working with annotations in PDF files. You can either install the API through [NuGet][11] or download it directly from the [downloads][12] section.

```
PM> Install-Package Aspose.PDF.Cpp
```

## Read Annotations in PDF Files {#Read-Annotations-in-PDF-Files}

The following are the steps to read annotations in [PDF][13] files.

*   Firstly, create an instance of the [PdfAnnotationEditor][14] class.
*   Load the PDF file using the [PdfAnnotationEditor->BindPdf (System::SharedPtr<Aspose::Pdf::Document> srcDoc)][15] method.
*   Retrieve the annotations using the [PdfAnnotationEditor->ExtractAnnotations (int32\_t start, int32\_t end, System::ArrayPtr<Aspose::Pdf::Annotations::AnnotationType> annotTypes)][16] method.
*   Loop through the annotations and print their content.

The following is the sample code to read annotations in PDF files using [C++][17].

{{< gist aspose-com-gists 31c3fc7129c753b563f05dd29e91fc5b "Read-Annotations-In-PDF-File.cpp" >}}

## Add Annotations to PDF Files {#Add-Annotations-to-PDF-Files}

The following are the steps to add annotations to PDF files.

*   Firstly, create an instance of the [PdfContentEditor][18] class.
*   Load the PDF file using the [PdfContentEditor->BindPdf (System::SharedPtr<Aspose::Pdf::Document> srcDoc)][19] method.
*   Create the annotation using the [PdfContentEditor->CreateText (System::Drawing::Rectangle rect, System::String title, System::String contents, bool open, System::String icon, int32\_t page)][20] method.
*   Finally, save the PDF using the [PdfContentEditor->Save (System::String destFile)][21] method.

The following is the sample code to add annotations to PDF files using C++.

{{< gist aspose-com-gists 31c3fc7129c753b563f05dd29e91fc5b "Add-Annotations-To-PDF-File.cpp" >}}

The following is the image of the file saved by the sample code.



{{< figure align=center src="images/AnnotationAddedToPdfCpp.png" alt="Annotation added to the PDF file" caption="Image showing the annotation">}}


## Modify Annotations in PDF Files using C++ {#Modify-Annotations-in-PDF-Files-using-CPP}

The following are the steps to modify annotations in PDF files.

*   Firstly, create an instance of the [PdfAnnotationEditor][22] class.
*   Load the PDF file using the [PdfAnnotationEditor->BindPdf (System::SharedPtr<Aspose::Pdf::Document> srcDoc)][23] method.
*   Create an instance of the [TextAnnotation][24] class.
*   Set the content of the annotation.
*   Use the [PdfAnnotationEditor->ModifyAnnotations (int32\_t start, int32\_t end, System::SharedPtr<Aspose::Pdf::Annotations::Annotation> annotation)][25] method to modify the annotation.
*   Finally, save the updated PDF file using the [PdfAnnotationEditor->Save (System::String destFile)][26] method.

The following is the sample code to modify annotations in PDF files using C++.

{{< gist aspose-com-gists 31c3fc7129c753b563f05dd29e91fc5b "Modify-Annotations-In-PDF-File.cpp" >}}

## Remove Annotations from PDF Files {#Remove-Annotations-from-PDF-Files}

Aspose.PDF for C++ provides the following options for removing the annotations from PDF files.

*   [Remove a Specific Annotation][27]
*   [Removing Annotations by Type][28]
*   [Remove All Annotations][29]

### Remove a Specific Annotation {#Remove-a-Specific-Annotation}

The following are the steps to remove a specific annotation from a PDF file.

*   Firstly, create an instance of the [PdfAnnotationEditor][30] class.
*   Load the PDF file using the [PdfAnnotationEditor->BindPdf (System::SharedPtr<Aspose::Pdf::Document> srcDoc)][31] method.
*   Delete the annotation by name using the [PdfAnnotationEditor->DeleteAnnotation (System::String annotName)][32] method.
*   Finally, save the updated PDF file using the [PdfAnnotationEditor->Save (System::String destFile)][33] method.

The following is the sample code to remove a specific annotation from a PDF file using C++.

{{< gist aspose-com-gists 31c3fc7129c753b563f05dd29e91fc5b "Delete-Specific-Annotation-In-PDF-File.cpp" >}}

### Removing Annotations by Type {#Removing-Annotations-by-Type}

The following are the steps to remove annotations by type from PDF files.

*   Firstly, create an instance of the [PdfAnnotationEditor][34] class.
*   Load the PDF file using the [PdfAnnotationEditor->BindPdf (System::SharedPtr<Aspose::Pdf::Document> srcDoc)][35] method.
*   Delete the annotation by type using the [PdfAnnotationEditor->DeleteAnnotations (System::String annotType)][36] method.
*   Finally, save the updated PDF file using the [PdfAnnotationEditor->Save (System::String destFile)][37] method.

The following is the sample code to remove annotations by type from PDF files using C++.

{{< gist aspose-com-gists 31c3fc7129c753b563f05dd29e91fc5b "Delete-Annotations-By-Type-In-PDF-File.cpp" >}}

### Remove All Annotations {#Remove-All-Annotations}

The following are the steps to remove all annotations from PDF files.

*   Firstly, create an instance of the [PdfAnnotationEditor][38] class.
*   Load the PDF file using the [PdfAnnotationEditor->BindPdf (System::SharedPtr<Aspose::Pdf::Document> srcDoc)][39] method.
*   Delete all the annotations using the [PdfAnnotationEditor->DeleteAnnotations()][40] method.
*   Finally, save the updated PDF file using the [PdfAnnotationEditor->Save (System::String destFile)][41] method.

The following is the sample code to remove all annotations from PDF files using C++.

{{< gist aspose-com-gists 31c3fc7129c753b563f05dd29e91fc5b "Delete-All-Annotations-In-PDF-File.cpp" >}}

## Get a Free License {#Get-a-Free-License}

You can try the API without evaluation limitations by requesting [a free temporary license][42].

## Conclusion

In this article, you have learned how to work with annotations in PDF files using C++. Specifically, you have seen how to read, add, edit and delete annotations from PDF files. Furthermore, you have learned how to delete a specific annotation, annotations by type, or all annotations using Aspose.PDF for C++ API. The API provides a bunch of additional features for working with PDF files. You can explore the API in detail by using the [official documentation][43]. In case of any questions, please feel free to reach us on our [free support forum][44].

## See Also

*   [Split a PDF File using C++][45]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: https://docs.fileformat.com/programming/cpp/
[4]: #CPP-API-for-Working-with-Annotations-in-PDF-Files
[5]: #Read-Annotations-in-PDF-Files
[6]: #Add-Annotations-to-PDF-Files
[7]: #Modify-Annotations-in-PDF-Files-using-CPP
[8]: #Remove-Annotations-from-PDF-Files
[9]: #Get-a-Free-License
[10]: https://products.aspose.com/pdf/cpp
[11]: https://www.nuget.org/packages/Aspose.Pdf.cpp
[12]: https://downloads.aspose.com/pdf/cpp
[13]: https://docs.fileformat.com/pdf/
[14]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.pdf_annotation_editor
[15]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.facade#af78eeeca28cdc85d0341f6f2adb79878
[16]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.pdf_annotation_editor#ad908d77d01291e45e85349f0cab0f319
[17]: https://docs.fileformat.com/programming/cpp/
[18]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.pdf_content_editor
[19]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.facade#af78eeeca28cdc85d0341f6f2adb79878
[20]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.pdf_content_editor#a58e72132847b2673c24cb7f96e9668d4
[21]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.saveable_facade#a2b2bd2613b7cacf148c3cc37490ea969
[22]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.pdf_annotation_editor
[23]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.facade#af78eeeca28cdc85d0341f6f2adb79878
[24]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.annotations.text_annotation
[25]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.pdf_annotation_editor#a6902e9940771daad159bd58b8bdda04a
[26]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.saveable_facade#a2b2bd2613b7cacf148c3cc37490ea969
[27]: #Remove-a-Specific-Annotation
[28]: #Removing-Annotations-by-Type
[29]: #Remove-All-Annotations
[30]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.pdf_annotation_editor
[31]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.facade#af78eeeca28cdc85d0341f6f2adb79878
[32]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.pdf_annotation_editor#a8434c03a5e37a910d9f8129e5c443903
[33]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.saveable_facade#a2b2bd2613b7cacf148c3cc37490ea969
[34]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.pdf_annotation_editor
[35]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.facade#af78eeeca28cdc85d0341f6f2adb79878
[36]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.pdf_annotation_editor#a7097b2ba1a1ebc51c2fe75ed9557ed6e
[37]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.saveable_facade#a2b2bd2613b7cacf148c3cc37490ea969
[38]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.pdf_annotation_editor
[39]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.facade#af78eeeca28cdc85d0341f6f2adb79878
[40]: //apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.pdf_annotation_editor#a43088ed22371b19df22b3a42736cd4b7
[41]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.saveable_facade#a2b2bd2613b7cacf148c3cc37490ea969
[42]: https://purchase.aspose.com/temporary-license
[43]: https://docs.aspose.com/pdf/cpp/
[44]: https://forum.aspose.com/c/pdf/10
[45]: https://blog.aspose.com/2021/03/19/split-a-pdf-file-using-cpp/





