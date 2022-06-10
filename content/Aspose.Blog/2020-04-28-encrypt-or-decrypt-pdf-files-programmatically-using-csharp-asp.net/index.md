---
title: 'Encrypt and Decrypt PDF Files using C#'
seoTitle: "C# Encrypt and Decrypt PDF Files | Encrypt PDF with Password in C#"
description: "Steps to encrypt and decrypt PDF files in C# or VB.NET. Encrypt PDF documents with a password. Change security permissions in PDF using C# PDF Library."
date: Tue, 28 Apr 2020 11:03:33 +0000
draft: false
url: /2020/04/28/encrypt-or-decrypt-pdf-files-programmatically-using-csharp-asp.net/
author: Usman Aziz
summary: ''
tags: ['change security permissions of pdf in csharp', 'decrypt pdf documents in csharp', 'encrypt pdf document in csharp']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Excrypt-and-Decrypt-PDF-in-C.jpg" alt="Excrypt and Decrypt PDF in C#">}}


PDF encryption is used to secure the PDF document from unauthorized access. If a PDF document is encrypted, you have to decrypt it to access its content, otherwise, it will remain unreadable. Most often, the PDF documents are encrypted with a password that is required to open the document. On the other hand, you can also limit the access permissions to various operations such as printing, editing, copying, etc. Aspose' PDF library, [Aspose.PDF for .NET][1], provides some simple ways to **encrypt and decrypt PDF** files using C# and VB.NET. In this article, I'll show you how to perform PDF encryption and decryption operations using C#.

*   [Encrypt a PDF file using C#][2]
*   [Decrypt a PDF file using C#][3]
*   [Change security permissions in a PDF file][4]

## C# PDF Encryption and Decryption API - Installation

Aspose.PDF for .NET is hosted on [NuGet][5] and can easily be installed using the NuGet Package Manager. Alternatively, you can download the API's DLL from the [Downloads][6] section.

## Encrypt a PDF Files in C# {#Encrypt-a-PDF-document}

In order to encrypt a PDF file, you need to set a password that will be required to open and view the document. In addition, you have to specify the desired cryptographic algorithm as the encryption method. Aspose.PDF for .NET supports the following encryption methods:

*   RC4 with a 40-bit key.
*   RC4 with a 128-bit key.
*   AES with a 128-bit key.
*   AES with a 256-bit key.

### Steps to Encrypt a PDF File

The following are the simple steps to encrypt a PDF document using C#.

*   Load the PDF document using [Document][7] class.
*   Encrypt the PDF document with a password and cryptographic algorithm using [Document.Encrypt][8] method.
*   Save the encrypted PDF document using [Document.Save][9] method.

The following code sample shows how to encrypt a PDF document using C#.

{{< gist aspose-com-gists 6536573a3f7c04b581ea9fd9f480f12e "encrypt-pdf.cs" >}}

When you will open this encrypted PDF document in Adobe Reader, it will popup the following dialogue.



{{< figure align=center src="images/Encrypted-PDF-Document.jpg" alt="encrypted PDF document">}}


## Decrypt a PDF File using C# {#Decrypt-a-PDF-document}

In order to decrypt a PDF document, you must have the user or owner password of the document. The following are the simple steps to decrypt a PDF document:

*   Load PDF document using [Document][10] class by specifying the user's or owner's password.
*   Call [Document.Decrypt()][11] method.
*   Save the decrypted PDF document.

The following code sample shows how to decrypt a PDF document using C#.

{{< gist aspose-com-gists 6536573a3f7c04b581ea9fd9f480f12e "decrypt-pdf.cs" >}}

## Change Security Permissions of a PDF File in C# {#Change-security-permissions-in-a-PDF-document}

You can enhance the security of a PDF document by limiting the user's permission. In such a case, you can specify the operations which are allowed for the users. The following is the list of the permissions that you can set to allow for a user.

*   **Print Document** - Allows printing the document.
*   **Modify Content** - Allows modifying the contents of the document.
*   **Extract Content** - Allows copying the content from the document.
*   **Modify Text Annotations** - Allows adding or modifying text annotations.
*   **Fill Form** - Allows filling in the interactive form fields.
*   **Extract Content with Disabilities** - Allows extracting text and graphics (for users with disabilities).
*   **Assemble Document** - Allows to insert, rotate, or delete pages and create bookmarks or thumbnail images.
*   **Printing Quality** - Allows printing documents with high resolution.

### Steps to Change Security Permissions of a PDF File

The following are the steps to change the security permissions of a PDF document.

*   Load the PDF document.
*   Set security permissions using [Document.Encrypt][12] method.
*   Save the encrypted PDF document.

The following code sample shows how to change permissions of a PDF document using C#.

{{< gist aspose-com-gists 6536573a3f7c04b581ea9fd9f480f12e "encrypt-pdf-with-permissions.cs" >}}

Another way to set or modify the privileges of PDF documents is by using [DocumentPrivilege][13] class. The _DocumentPrivilege_ class lets you define the permissions or privileges for the users. The following code sample shows how to set the security permissions of a PDF document using _DocumentPrivilege_ class in C#.

{{< gist aspose-com-gists 6536573a3f7c04b581ea9fd9f480f12e "encrypt-pdf-with-privileges.cs" >}}

The following are the security details of the PDF document we have encrypted in this section.



{{< figure align=center src="images/Encrypt-PDF-C.jpg" alt="changed security permissions of PDF">}}


## Conclusion

In this article, you have gone through the steps of how to encrypt and decrypt PDF documents using C#. Furthermore, you have also learned how to set or modify the security permissions of a PDF document in C#. These security features let you protect the sensitive PDF documents using the password and cryptographic algorithms as well as limit the user's access to the document related operations. You may consult the [documentation][14] to learn more about our .NET PDF Library.

## See Also

*   [Add and Verify Digital Signatures in PDF Documents using C#][15]




[1]: https://products.aspose.com/pdf/net
[2]: #Encrypt-a-PDF-document
[3]: #Decrypt-a-PDF-document
[4]: #Change-security-permissions-in-a-PDF-document
[5]: https://nuget.org/packages/Aspose.pdf
[6]: https://downloads.aspose.com/pdf/net
[7]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[8]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/encrypt/methods/1
[9]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/4
[10]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[11]: https://apireference.aspose.com/pdf/net/aspose.pdf/document/methods/decrypt
[12]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/encrypt/methods/1
[13]: https://apireference.aspose.com/pdf/net/aspose.pdf.facades/documentprivilege
[14]: https://docs.aspose.com/display/pdfnet/Getting+Started
[15]: https://blog.aspose.com/2020/02/25/digitally-sign-pdf-documents-verify-digital-signatures-in-csharp-net/





