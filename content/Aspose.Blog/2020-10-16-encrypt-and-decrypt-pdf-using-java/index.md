---
title: 'Encrypt and Decrypt PDF Files using Java'
seoTitle: ""
description: ""
date: Fri, 16 Oct 2020 22:03:17 +0000
draft: false
url: /2020/10/16/encrypt-and-decrypt-pdf-using-java/
author: Usman Aziz
summary: 'In various cases, PDF documents are encrypted before they are shared among the stakeholders. The encryption makes the document secure from unauthorized access as well as the content tampering. There are a couple of popular ways of securing the PDF documents – encrypting PDF with a password or limiting the user’s access permissions such as printing, editing, copying, etc. This article demonstrates how to encrypt or decrypt a PDF document using Java. In addition, you will learn how to limit the user’s privileges in a PDF document.'
tags: ['change permissions in pdf using java', 'decrypt pdf using java', 'encrypt pdf using java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Excrypt-and-Decrypt-PDF-Java.jpg" alt="encrypt or decrypt pdf java">}}


In various cases, [PDF][1] documents are encrypted before they are shared among the stakeholders. The encryption makes the document secure from unauthorized access as well as content tampering. There are a couple of popular ways of securing PDF documents - encrypting PDF with a password or limiting the user's access permissions such as printing, editing, copying, etc. This article demonstrates **how to encrypt or decrypt a PDF using Java**. In addition, you will learn how to limit the user's privileges in a PDF document.

*   [Java API to Encrypt or Decrypt PDF][2]
*   [Encrypt a PDF File using Java][3]
*   [Decrypt a PDF File using Java][4]
*   [Change Security Permissions in a PDF using Java][5]

## Encrypt or Decrypt PDF Java API - Free Download {#Java-API-to-Encrypt-or-Decrypt-PDF}

[Aspose.PDF for Java][6] is a feature-rich PDF manipulation API that lets you work with PDF encryption and decryption seamlessly. In addition, it lets you modify the user's privileges in the PDF documents programmatically. You can [download][7] the API for free or get it installed using the following Maven configurations.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
```
```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-pdf</artifactId>
    <version>20.9</version>
    <classifier>jdk17</classifier>
</dependency>
```

## Encrypt a PDF File using Java {#Encrypt-a-PDF-File-using-Java}

Encryption of a PDF document requires you to set a password that will be used to open and access the document. Along with this, you can choose one of the following cryptographic algorithms to be used in the encryption.

*   [RC4 with a 40-bit key][8]
*   [RC4 with a 128-bit key][9]
*   [AES with a 128-bit key][10]
*   [AES with a 256-bit key][11]

The following are the steps to encrypt a PDF document using Aspose.PDF for Java.

*   Load the PDF document using [Document][12] class.
*   Encrypt PDF using [Document.encrypt("user\_password", "owner\_password", 0, CryptoAlgorithm)][13] method.
*   Save the encrypted PDF using the [Document.save(string)][14] method.

The following code sample shows how to encrypt a PDF document using Java.

{{< gist aspose-pdf 474c352a71ac9477aa0d604fd32e1c6a "Examples-src-main-java-com-aspose-pdf-examples-NewDocumentObject-securityandsignatures-EncryptPDFDocumentUsingEncryptionTypes-.java" >}}

The following dialog appears when you open the encrypted PDF.



{{< figure align=center src="images/Encrypted-PDF-Document.jpg" alt="encrypted pdf ">}}


## Decrypt a PDF File using Java {#Decrypt-a-PDF-file-using-Java}

The decryption of an encrypted PDF document requires the user's or owner's password. The following are the steps to decrypt a PDF document using Aspose.PDF for Java.

*   Load the encrypted PDF using the [Document][15] class by specifying the password in the constructor.
*   Call [Document.decrypt()][16] method to decrypt the PDF.
*   Save the decrypted PDF document using the [Document.save(string)][17] method.

The following code sample shows how to decrypt an encrypted PDF using Java.

{{< gist aspose-pdf 474c352a71ac9477aa0d604fd32e1c6a "Examples-src-main-java-com-aspose-pdf-examples-NewDocumentObject-securityandsignatures-DecryptPDFFileUsingOwnerPassword-.java" >}}

## Change Security Permissions in a PDF using Java {#Change-Security-Permissions-in-a-PDF-using-Java}

You can also limit the user's access to perform different operations while encrypting the PDF documents. The following are the permissions you can set.

*   **Print Document** – Allows document's printing.
*   **Modify Content** – Allows modification in the content.
*   **Extract Content** – Allows copying the content from the document.
*   **Modify Text Annotations** – Allows adding or updating text annotations.
*   **Fill Form** – Allows filling in the interactive form fields.
*   **Extract Content with Disabilities** – Allows extracting text and graphics (for users with disabilities).
*   **Assemble Document** – Allows inserting, rotating, or deleting pages and creating bookmarks or thumbnail images.
*   **Printing Quality** – Allows high-resolution printing of documents.

The following are the steps to set or modify permissions in a PDF document.

*   Load the PDF using the [Document][18] class.
*   Use the [DocumentPrivilege][19] class to set the permissions.
*   Encrypt the PDF and save it as you have done in the previous examples.

The following code sample shows how to modify permissions in a PDF document using Java.

{{< gist aspose-pdf 474c352a71ac9477aa0d604fd32e1c6a "Examples-src-main-java-com-aspose-pdf-examples-NewDocumentObject-securityandsignatures-SetPrivilegesOnAnExistingPDFFile-.java" >}}

The following are the permissions in the encrypted PDF file.



{{< figure align=center src="images/Encrypt-PDF-C.jpg" alt="encrypted pdf">}}


## Conclusion

In this article, you have learned how to encrypt or decrypt PDF files using Java. In addition, you have seen how to modify the user's privileges in a PDF document programmatically. You can explore and learn more about the Java PDF API using [documentation][20].

## See Also

*   [Add and Verify Digital Signatures in PDF using Java][21]




[1]: https://docs.fileformat.com/pdf/
[2]: #Java-API-to-Encrypt-or-Decrypt-PDF
[3]: #Encrypt-a-PDF-File-using-Java
[4]: #Decrypt-a-PDF-file-using-Java
[5]: #Change-Security-Permissions-in-a-PDF-using-Java
[6]: https://products.aspose.com/pdf/java
[7]: https://downloads.aspose.com/pdf/java
[8]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/CryptoAlgorithm#RC4x40
[9]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/CryptoAlgorithm#RC4x128
[10]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/CryptoAlgorithm#AESx128
[11]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/CryptoAlgorithm#AESx256
[12]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[13]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#encrypt-java.lang.String-java.lang.String-int-int-
[14]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[15]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[16]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#decrypt--
[17]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[18]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[19]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.facades/DocumentPrivilege
[20]: https://docs.aspose.com/pdf/java/
[21]: https://blog.aspose.com/2020/07/15/add-and-verify-digital-signatures-in-pdf-documents-using-java/





