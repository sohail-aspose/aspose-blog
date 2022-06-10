---
title: 'Encrypt or Decrypt PDF Files using C++'
seoTitle: "Encrypt and Decrypt PDF Files in C++ | C++ PDF Encryption in AES, RC4"
description: "C++ code to encrypt and decrypt PDF files. Set password and user's privileges while encrypting PDF files with AES128, 256, or RC4 cryptography using C++."
date: Fri, 25 Sep 2020 01:17:29 +0000
draft: false
url: /2020/09/25/encrypt-or-decrypt-pdf-files-using-cpp/
author: Usman Aziz
summary: "PDF Encryption is the process of protecting the document using a password as well as some cryptographic algorithms including AES or RC4. You can also set different privileges to limit user's access to different operations. For example, you can only allow printing, adding annotation, filling forms, and etc. In this article, you will learn how to encrypt PDF files using C++. Furthermore, this article also covers how to set different privileges and decrypt password-protected PDF files using C++."
tags: ['decrypt pdf using cpp', 'encrypt pdf using cpp', 'set password for pdf using cpp']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose_pdf-for-cpp.png" alt="encrypt decrypt pdf C++">}}


PDF encryption is the process of protecting the document using a password as well as some cryptographic algorithms including [AES][1] or [RC4][2]. You can also set different privileges to limit user's access to different operations. For example, you can only allow printing, adding annotation, filling forms, and etc. In this article, you will learn **how to encrypt PDF files using C++**. Furthermore, this article also covers how to set different privileges and **decrypt password-protected PDF files using C++**.

*   [C++ API to Encrypt or Decrypt PDF Files][3]
*   [Encrypt PDF Files using C++][4]
*   [Decrypt PDF Files using C++][5]

## C++ API to Encrypt or Decrypt PDF Files {#C++-API-to-Encrypt-or-Decrypt-PDF-Files}

[Aspose.PDF for C++][6] is a native C++ API that lets you create, read, and manipulate PDF documents. In addition, it also allows you to encrypt PDFs with passwords and decrypt the encrypted PDFs within a few lines of code. You can download the API from the [downloads][7] section or get it installed using [NuGet][8].

## Encrypt PDF Files using C++ {#Encrypt-PDF-Files-using-C++}

The following are the steps to encrypt a PDF file using Aspose.PDF for C++.

*   Load the PDF document using [Document][9] class.
*   Use [DocumentPrivilege][10] class to set different privileges such as allow printing, allow modifying content and etc.
*   Call [Document.Encrypt(String, String, SharedPtr<DocumentPrivilege>, CryptoAlgorithm, bool)][11] method to encrypt the PDF.
*   Save the PDF using the [Document->Save(String)][12] method.

The following code sample shows how to encrypt a PDF file using C++.

{{< gist aspose-pdf e5fb9ddf5bd6460bb13d47fe5a83d86d "Examples-PdfCPP-SecurityAndSignatures-SetPrivileges-Priveleges.cpp" >}}

## Decrypt PDF Files using C++ {#Decrypt-PDF-Files-using-C++}

The following are the steps to decrypt a PDF file using Aspose.PDF for C++.

*   Load the PDF file using the [Document][13] class and provide the document's path and password.
*   Decrypt the file using [Document->Decrypt()][14] method.
*   Save the decrypted PDF using the [Document->Save(String)][15] method.

The following code sample shows how to decrypt a PDF using C++.

{{< gist aspose-pdf e5fb9ddf5bd6460bb13d47fe5a83d86d "Examples-PdfCPP-SecurityAndSignatures-DecryptPDFFile-1.cpp" >}}

## Conclusion

In this article, you have learned how to encrypt or decrypt PDF files using C++. The code sample has also shown how to set different privileges when encrypting a PDF file. You can explore more about the C++ PDF API using [documentation][16].

## See Also

*   [Create PDF Files Programmatically using C++][17]




[1]: https://en.wikipedia.org/wiki/Advanced_Encryption_Standard
[2]: https://en.wikipedia.org/wiki/RC4
[3]: #C++-API-to-Encrypt-or-Decrypt-PDF-Files
[4]: #Encrypt-PDF-Files-using-C++
[5]: #Decrypt-PDF-Files-using-C++
[6]: https://products.aspose.app/pdf/cpp
[7]: https://downloads.aspose.com/pdf/cpp
[8]: https://www.nuget.org/packages/Aspose.pdf.cpp
[9]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[10]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.facades.document_privilege
[11]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a009045819e0517cf0ba85bf48920ccee
[12]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a5f0d3a0eaf87e479ae2bf52f7eb438d7
[13]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[14]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a9c26014465f4368edc6fc62b7ef3d76a
[15]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a5f0d3a0eaf87e479ae2bf52f7eb438d7
[16]: https://docs.aspose.com/pdf/cpp/get-started/
[17]: https://blog.aspose.com/2020/03/17/create-pdf-files-in-cpp-using-pdf-api/





