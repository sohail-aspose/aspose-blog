---
title: 'Add or Remove Attachments in PDF Files using C++'
seoTitle: "C++ Add or Remove Attachments in PDF Files | C++ PDF API"
description: "Use C++ PDF API to access, add and remove attachments in PDF files using C++ from within your applications. Complete tutorial with C++ code samples."
date: Mon, 02 Nov 2020 23:38:54 +0000
draft: false
url: /2020/11/02/add-or-remove-pdf-attachments-using-cpp/
author: Usman Aziz
summary: '[PDF][1] has become a massively used file format because of its cross-platform support. You can create a PDF on the Windows platform, for example, and then transfer it to the Mac without any compatibility or formatting issues. One of the powerful features that PDF supports is adding attachments. You can embed other documents into a PDF file just like the email attachments. In this article, you are going to learn how to deal with PDF attachments programmatically. More specifically, you will come to know **how to get, add, and remove attachments in PDF files using C++**.'
tags: ['Cpp PDF API', 'add pdf attachment using cpp', 'get pdf attachment info using cpp', 'remove pdf attachment using cpp']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/add-remove-attachments-in-pdf-using-cpp-featimage.png" alt="add or remove attachments in pdf c++">}}


[PDF][2] has become a massively used file format because of its cross-platform support. You can create a PDF on the Windows platform, for example, and then transfer it to the Mac without any compatibility or formatting issues. One of the powerful features that PDF supports is adding attachments. You can embed other documents into a PDF file just like the email attachments. In this article, you are going to learn how to deal with PDF attachments programmatically. More specifically, you will come to know **how to get, add, and remove attachments in PDF files using C++**.

*   [C++ API for PDF Attachments - Free Download][3]
*   [Get PDF Attachment Information using C++][4]
*   [Add an Attachment to PDF in C++][5]
*   [Remove an Attachment from PDF in C++][6]

## C++ API for PDF Attachments - Free Download {#C++-API-to-Work-with-PDF-Attachments}

In order to work with PDF attachments seamlessly, you can leverage the capabilities of [Aspose.PDF for C++][7]. The API lets you add, remove, or access the PDF attachments within a few lines of code. You can [download][8] the API's package or get it installed using [NuGet][9].

```
PM> Install-Package Aspose.PDF.Cpp
```

## Get PDF Attachment Information using C++ {#Get-PDF-Attachment-Information-using-C++}

First of all, let's have a look at how to access the attachments' information from a PDF document. For this, you can follow the below steps.

*   Load the PDF document using [Document][10] class.
*   Use [Document->get\_EmbeddedFiles()->idx\_get(index)][11] method to access the attachment's information into [FileSpecification][12] object.
*   Retrieve name, description, and mime type of the attachment using _FileSpecification_ object.

The following code sample shows how to get PDF attachment's information using C++.

{{< gist aspose-com-gists 7795776c555f43ff518d434bdb47133c "get-pdf-attachment-info.cpp" >}}

## Add an Attachment to PDF in C++ {#Add-an-Attachment-to-PDF-in-C++}

Now, let's check out how to add an attachment to the PDF using Aspose.PDF for C++. The attachment could be any file such as DOCX, TXT, and etc. The following are the steps for adding a TXT file to PDF as an attachment.

*   Load the file to be attached using [FileSpecification][13] class.
*   Load the PDF file using [Document][14] class.
*   Add file as attachment using [Document->get\_EmbeddedFiles()->Add(FileSpecification)][15] method.
*   Save the PDF using [Document->Save(u"file.pdf")][16] method.

The following code sample shows how to add an attachment to a PDF using C++.

{{< gist aspose-com-gists 7795776c555f43ff518d434bdb47133c "add-pdf-attachment.cpp" >}}

## Remove an Attachment from PDF in C++ {#Remove-an-Attachment-from-PDF-in-C++}

You can also remove the selected or all the attachments from the PDF using Aspose.PDF for C++. The following are the steps to do so.

*   Load the PDF document using [Document][17] class.
*   Use [Document->get\_EmbeddedFiles()->Delete()][18] method to remove all attachments or [Document->get\_EmbeddedFiles()->Delete(String)][19] to remove a specific attachment by name.
*   Save the PDF using [Document->Save(u"file.pdf")][20] method.

The following code sample shows how to remove attachments from a PDF using C++.

{{< gist aspose-com-gists 7795776c555f43ff518d434bdb47133c "delete-pdf-attachment.cpp" >}}

## Conclusion

In this article, you have learned how to manipulate attachments in PDF files using C++. The code samples have demonstrated how to access, add and remove the attachments from PDF files programmatically. You can learn more about the C++ PDF API using the [documentation][21].

## See Also

*   [Create PDF Documents using C++ PDF API][22]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: #C++-API-to-Work-with-PDF-Attachments
[4]: #Get-PDF-Attachment-Information-using-C++
[5]: #Add-an-Attachment-to-PDF-in-C++
[6]: #Remove-an-Attachment-from-PDF-in-C++
[7]: http://products.aspose.com/pdf/cpp
[8]: http://downloads.aspose.com/pdf/cpp
[9]: https://www.nuget.org/packages/Aspose.pdf.cpp
[10]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[11]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a313099730894a9d9cff07917d8330a49
[12]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.file_specification
[13]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.file_specification
[14]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[15]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.embedded_file_collection#aa76ece4a8fa469ba40bbaff20ae38edf
[16]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a5f0d3a0eaf87e479ae2bf52f7eb438d7
[17]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[18]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.embedded_file_collection#ae52ed6f122b25127a52be1460af5b080
[19]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.embedded_file_collection#afff8b235b554a66c203464b61204b843
[20]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a5f0d3a0eaf87e479ae2bf52f7eb438d7
[21]: https://docs.aspose.com/pdf/cpp/
[22]: https://blog.aspose.com/2020/03/17/create-pdf-files-in-cpp-using-pdf-api/





