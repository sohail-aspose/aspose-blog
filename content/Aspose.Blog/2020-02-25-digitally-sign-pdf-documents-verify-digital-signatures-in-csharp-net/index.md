---
title: 'Add and Verify Digital Signatures in PDF Documents using C#'
seoTitle: ""
description: ""
date: Tue, 25 Feb 2020 16:38:29 +0000
draft: false
url: /2020/02/25/digitally-sign-pdf-documents-verify-digital-signatures-in-csharp-net/
author: Usman Aziz
summary: ''
tags: ['add digital signature to PDF in csharp', 'digitally sign PDF documents', 'verify digital signatures in PDF']
categories: ['Aspose.PDF Product Family']
---

**Digital Signatures** are used to secure PDF documents before they are shared with third parties. **Digitally signing a PDF** document makes it possible to detect tampering by verifying the document using the digital signature. In order to secure the PDF documents programmatically using digital signatures, this article will show you how to **add and verify digital signatures in a PDF document** using **C#**. Ultimately, you will learn how to:

*   [Add digital signatures in PDF documents using C#][1]
*   [Digitally sign PDF documents with a Timestamp server in C#][2]
*   [Verify digital signature in PDF using C#][3]

## C# Library for Digital Signatures in PDF

In order to add and verify digital signatures in PDF documents, we'll use [Aspose.PDF for .NET][4] API which is a powerful PDF manipulation API for creating, editing, converting and digitally signing PDF documents. You can [download][5] _Aspose.PDF for .NET_ or install it using one of the following ways in Visual Studio:

### NuGet Package Manager



{{< figure align=center src="images/Aspose.PDF-NPM.png" alt="Digitally Sign PDF in C#">}}


### Package Manager Console```
PM> Install-Package Aspose.PDF
```

## Add Digital Signature to a PDF Document in C# {#Add-digital-signatures-in-PDF-documents-using-CSharp}

The following are the steps to sign a PDF document using _Aspose.PDF for .NET_.

*   Create an object of the [Document][6] class and initialize it with the PDF document's path.
*   Create an object of [PdfFileSignature][7] class and initialize it with the _Document_ class's object.
*   Create an object of [PKCS7][8] class and initialize it with a certificate path and password.
*   Create and initialize the object of [DocMDPSignature][9] class for the MDP signature type.
*   Create a [Rectangle][10] for signature placement.
*   Digitally sign PDF document using [PdfFileSignature.Certify()][11] method.
*   Save the document using [PdfFileSignature.Save()][12] method.

The following code sample shows how to add a digital signature to a PDF document in C#.

{{< gist aspose-com-gists 03c3ca31623750822d7c80438a76d786 "digitally-sign-PDF.cs" >}}

## Add Digital Signature to PDF using Timestamp Server in C# {#Add-Digital-Signature-to-PDF-using-Timestamp-Server-in-CSharp}

You can also add a digital signature to a PDF document with the TimeStamp server by providing its details using the [TimestampSettings][13] class. The following code sample shows how to digitally sign a PDF document with a TimeStamp server in C#.

{{< gist aspose-com-gists 03c3ca31623750822d7c80438a76d786 "digitally-sign-PDF-timestamp-server.cs" >}}

## Verify Digital Signatures in PDF using C# {#Verify-digital-signature-in-PDF-using-CSharp}

The following are the steps to verify the digital signature in a PDF document:

*   Create an object of the [Document][14] class and initialize it with the PDF document's path.
*   Create an object of [PdfFileSignature][15] class and initialize it with the _Document_ class's object.
*   Access all the signatures of the PDF document.
*   Verify the validity of the signature using [PdfFileSignature.VerifySigned()][16] method.

The following code sample shows how to verify the digital signature in PDF using C#.

{{< gist aspose-com-gists 03c3ca31623750822d7c80438a76d786 "verify-digital-signature.cs" >}}

## Try Aspose.PDF for .NET for Free

You can get a [free temporary license][17] to try and use _Aspose.PDF for .NET_.

## Related Articles

*   [Encrypt or Decrypt PDF Documents using C#][18]




[1]: #Add-digital-signatures-in-PDF-documents-using-CSharp
[2]: #Add-Digital-Signature-to-PDF-using-Timestamp-Server-in-CSharp
[3]: #Verify-digital-signature-in-PDF-using-CSharp
[4]: https://products.aspose.com/pdf/net
[5]: https://downloads.aspose.com/pdf/net
[6]: https://apireference.aspose.com/net/pdf/aspose.pdf/document
[7]: https://apireference.aspose.com/net/pdf/aspose.pdf.facades/pdffilesignature
[8]: https://apireference.aspose.com/net/pdf/aspose.pdf.forms/pkcs7
[9]: https://apireference.aspose.com/net/pdf/aspose.pdf.forms/docmdpsignature
[10]: https://docs.microsoft.com/en-us/dotnet/api/system.drawing.rectangle.-ctor?view=netframework-4.8#System_Drawing_Rectangle__ctor_System_Int32_System_Int32_System_Int32_System_Int32_
[11]: https://apireference.aspose.com/net/pdf/aspose.pdf.facades/pdffilesignature/methods/certify
[12]: https://apireference.aspose.com/net/pdf/aspose.pdf.facades.pdffilesignature/save/methods/2
[13]: https://apireference.aspose.com/net/pdf/aspose.pdf/timestampsettings
[14]: https://apireference.aspose.com/net/pdf/aspose.pdf/document
[15]: https://apireference.aspose.com/net/pdf/aspose.pdf.facades/pdffilesignature
[16]: https://apireference.aspose.com/net/pdf/aspose.pdf.facades/pdffilesignature/methods/verifysigned
[17]: https://purchase.aspose.com/temporary-license
[18]: https://blog.aspose.com/2020/04/28/encrypt-or-decrypt-pdf-files-programmatically-using-csharp-asp.net/





