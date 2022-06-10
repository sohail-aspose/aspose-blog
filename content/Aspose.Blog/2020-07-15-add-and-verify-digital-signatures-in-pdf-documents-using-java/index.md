---
title: 'Add and Verify Digital Signatures in PDF Documents using Java'
seoTitle: "Digitally Sign PDF using Java | Add and Verify Digital Signatures in PDF"
description: "Digitally sign PDF documents using Java. Verify, or validate the digitally sign PDFs using Java Swing or any Java-based application with Java PDF Library."
date: Wed, 15 Jul 2020 23:03:00 +0000
draft: false
url: /2020/07/15/add-and-verify-digital-signatures-in-pdf-documents-using-java/
author: Usman Aziz
summary: ''
tags: ['add digital signature to PDF using Java', 'certify digital signature in PDF using Java', 'digitally sign PDF using Java', 'verify digitally signed PDF using Java']
categories: ['Aspose.PDF Product Family']
---

**Digital Signature in PDF** lets you secure the document before it is shared with the stakeholders. Forging in the content of a digitally signed PDF document can easily be detected and verified. In order to digitally sign the PDF documents programmatically, I'll show you **how to add and verify digital signatures in PDF using Java**. We'll cover the following scenarios related to digital signatures in PDFs.

*   [Java Library to Digitally Sign PDF][1]
*   [Add Digital Signatures to PDF using Java][2]
*   [Digitally Sign PDF with a Timestamp Server using Java][3]
*   [Verify Digital Signature in a PDF using Java][4]

## Java Library to Digitally Sign PDF {#Java-Library-to-Digitally-Sign-PDF}

For adding and verifying digital signatures in PDF, we'll be using [Aspose.PDF for Java][5]. Along with other PDF manipulation features, Aspose.PDF for Java lets you add and verify digital signatures in PDFs seamlessly. You can [download][6] the JAR of the API or get it installed in your Maven-based application.

### Repository```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
```

### Dependency```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-pdf</artifactId>
    <version>20.6</version>
</dependency>
```

## Add Digital Signature to a PDF using Java {#Add-Digital-Signatures-to-PDF-using-Java}

The following are the steps to add a digital signature to a PDF document using Aspose.PDF for Java.

*   Create an instance of the [Document][7] class and initialize it with the PDF document’s path.
*   Initialize the [PdfFileSignature][8] class and pass to it the _Document_ object.
*   Create an instance of [PKCS7][9] class and initialize it with a certificate's path and the password.
*   Initialize [DocMDPSignature][10] class for the MDP signature type.
*   Define a [Rectangle][11] to place the signature on the document's page.
*   Digitally sign PDF document using [PdfFileSignature.Certify()][12] method.
*   Save the signed PDF using [PdfFileSignature.Save()][13] method.

The following code sample shows how to digitally sign a PDF using Java.

{{< gist aspose-com-gists 0d8ebf3a10027842cebb1b6aa775520a "digitally-sign-PDF.java" >}}

## Digitally Sign PDF with a Timestamp Server using Java {#Digitally-Sign-PDF-with-a-Timestamp-Server-using-Java}

Aspose.PDF for Java also lets you add digital signatures to PDF with the TimeStamp server. The [TimestampSettings][14] class is used for this purpose. The following code sample shows how to add digital signature to a PDF with a TimeStamp server using Java.

{{< gist aspose-com-gists 0d8ebf3a10027842cebb1b6aa775520a "digitally-sign-PDF-timestamp.java" >}}

## Verify Digital Signature in a PDF using Java {#Verify-Digital-Signature-in-a-PDF-using-Java}

When you receive a digitally signed PDF, you can verify its signature quite easily. The following are the steps to verify a digitally signed PDF.

*   Create an instance of the [PdfFileSignature][15] class.
*   Bind the PDF file using [PdfFileSigntature.bindPdf(string)][16] method.
*   Verify the validity of the signature using [PdfFileSignature.verifySigned()][17] method.

The following code sample shows how to verify a digitally signed PDF document using Java.

{{< gist aspose-com-gists 0d8ebf3a10027842cebb1b6aa775520a "verify-digitally-sign-PDF.java" >}}

## Conclusion

In this article, you have learned how to add digital signature to a PDF using Java. In addition, we have seen how to verify a digitally signed PDF file within a few steps. You can learn more about Java PDF API using the [documentation][18] as well as the source code samples hosted on [GitHub][19].

## See Also

*   [Digitally Sign and Verify PDF Files using C#][20]




[1]: #Java-Library-to-Digitally-Sign-PDF
[2]: #Add-Digital-Signatures-to-PDF-using-Java
[3]: #Digitally-Sign-PDF-with-a-Timestamp-Server-using-Java
[4]: #Verify-Digital-Signature-in-a-PDF-using-Java
[5]: https://products.aspose.com/pdf
[6]: https://downloads.aspose.com/pdf/java
[7]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[8]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.facades/PdfFileSignature
[9]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/PKCS7
[10]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/DocMDPSignature
[11]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Rectangle
[12]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.facades/PdfFileSignature#certify-int-java.lang.String-java.lang.String-java.lang.String-boolean-java.awt.Rectangle-com.aspose.pdf.DocMDPSignature-
[13]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.facades/PdfFileSignature#save-java.lang.String-
[14]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TimestampSettings
[15]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.facades/PdfFileSignature
[16]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.facades/PdfFileSignature#bindPdf-java.lang.String-
[17]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.facades/PdfFileSignature#verifySigned-java.lang.String-
[18]: https://docs.aspose.com/display/pdfjava/Home
[19]: https://github.com/aspose-pdf/Aspose.PDF-for-Java
[20]: https://blog.aspose.com/2020/02/25/digitally-sign-pdf-documents-verify-digital-signatures-in-csharp-net/





