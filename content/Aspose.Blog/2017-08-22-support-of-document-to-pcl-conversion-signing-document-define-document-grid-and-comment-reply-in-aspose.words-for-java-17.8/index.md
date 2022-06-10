---
title: 'Convert Word Document to PCL using Java'
date: Tue, 22 Aug 2017 06:41:42 +0000
draft: false
url: /2017/08/22/support-of-document-to-pcl-conversion-signing-document-define-document-grid-and-comment-reply-in-aspose.words-for-java-17.8/
author: Tilal Ahmad
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose-Words-for-Java.png" alt="">}}


We are pleased to announce new release of [**Aspose.Words for Java 17.8**][1]. This month release consists of all the features, enhancements and fixes introduced in its corresponding .NET version along with a new feature of Document to PCL conversion support. Some of the other improvements are introduction of Signature line for signing Document, get and update Comment reply, enhanced compression of PDF documents along with other features. Please check the [detailed release notes][2] of this version to get an idea about all the new features/enhancements and fixes made in this release.

Furthermore, if you are planning to upgrade the API from any previous version, we strongly recommend you to check the [Public API Changes section of current release][3] and other intermediate releases from [release notes folder][4], to know what has been changed since your current revision of the API.

The following sections describe some details regarding these newly added features/enhancements.

## Convert Word Document to PCL using Java

We have introduced new saving format – PCL (Printer Command Language) in this version of Aspose.Words for Java. Aspose.Words can save documents to PCL 6 (PCL 6 Enhanced or PCL XL) format. There is one major feature of PCL that is unsupported in the current version of Aspose.Words i.e. custom fonts. It is a rather big and complex problem, but we will implement this feature in the future.

[Save Document to PCL][5]

## Defining Document Grid in Word Document

We have added new feature in Aspose.Words for .NET 17.8 to control behavior of document grid. The LayoutMode, CharactersPerLine, and LinesPerPage properties have added into PageSetup class. Now, you can set and get the number of characters per line and number of lines per page in the document grid.  
PageSetup.LayoutMode property has added to get or set the layout mode of a section. Please refer to the following article for more detail:

[Set Lines per Page and Number of Characters per Line][6]

## Detect Resolved Comments, Replies and Reply to Comment

We have added a read-only public API to get extended comment properties. You can read the comment and resolve it. Comment.Replies property returns a collection of Comment objects that are immediate children of the specified comment. Please check the following article for sample code snippet and details:

[How to Read Comment Reply][7]

## Detect Distance between Table and its Surrounding

A new feature has added in Aspose.Words 17.8 to get the distance between table and its surrounding text when text Wrapping of table is “Around”. We have introduced getDistanceTop, getDistanceBottom, getDistanceRight and getDistanceLeft properties for the purpose. Please check following article for sample code snippet and details:

[Get Distance between Table and Surrounding Text][8]

## PDF Document Compression

We have improved the compression of PDF in this release. Now document structure data and cross-reference table are written to Stream Object when saving to PDF 1.5 standard. This changes do not affect PDF/A-1 output due to limitations in specification.

## Format Number of Chart Data Label

We have added new feature in Aspose.Words for .NET 17.8 to format chart’s data label. New public property getNumberFormat is introduced in the ChartDataLabel class. ChartNumberFormat class represents number formatting of the parent element and contains getFormatCode, setFormatCode and isLinkedToSource public properties. Please refer to the following article for details:

[How to Format Number of Chart Data Label][9]

## Implementation of Signature Line in Document Signature

We have added new feature in Aspose.Words 17.8 to sign signature line in Word document. Please read following article:

[Signing Word Documents][10]

Please check the following API changes.

1\. Added new public property for SignatureLine class:

```
/// 
/// Gets or sets identifier for this signature line.
///This identifier can be associated with a digital signature, when signing document using .
/// This value must be unique and by default it is randomly generated with .
/// 
public java.util.UUID getId()
public void setId(java.util.UUID value)
```

2\. Added new public class SignOptions:

```
/// <summary>
/// Allows to specify options for document signing.
/// </summary>
public class SignOptions
```

It has the following public properties:

```
/// 
/// Specifies comments on the digital signature.
/// Default value is .
/// 
public java.lang.String getComments()
public void setComments(java.lang.String value)
 
/// 
/// The date of signing.
/// Default value is .
/// 
public java.util.Date getSignTime()
public void setSignTime(java.util.Date value)
 
/// 
/// Signature line identifier.
/// Default value is .
/// 
/// 
/// When set, it associates  with corresponding .
/// 
public java.util.UUID getSignatureLineId()
public void setSignatureLineId(java.util.UUID value)
 
/// 
/// The image that will be shown in associated .
/// Default value is null.
/// 
public byte[] getSignatureLineImage()
public void setSignatureLineImage(byte[] value)
 
/// 
/// The password to decrypt source document.
/// Default value is .
/// 
/// 
/// If OOXML document is encrypted, you should provide decryption password
/// to decrypt source document before it will be signed.
/// This is not required for documents in binary DOC format.
/// 
public java.lang.String getDecryptionPassword()
public void setDecryptionPassword(java.lang.String value)
```

3\. New public methods are introduced in DigitalSignatureUtil class for signing documents:

```
 /// 
/// Signs source document using given  and 
/// with digital signature and writes signed document to destination stream.
///Document should be either  or .
///Output will be written to the start of stream and stream size will be updated with content length.
/// 
///The stream which contains the document to sign.
///The stream that signed document will be written to.
/// object with certificate that used to sign file.
/// The certificate in holder MUST contain private keys and have the X509KeyStorageFlags.Exportable flag set.
/// object with various signing options.
 public static void sign(InputStream srcStream, InputStream dstStream, CertificateHolder certHolder, SignOptions signOptions)
 
/// 
/// Signs source document using given  and 
/// with digital signature and writes signed document to destination file.
///Document should be either  or .
/// 
///The file name of the document to sign.
///The file name of the signed document output.
/// object with certificate that used to sign file.
/// The certificate in holder MUST contain private keys and have the X509KeyStorageFlags.Exportable flag set.
/// object with various signing options.
public static void sign(string srcFileName, string dstFileName, CertificateHolder certHolder, SignOptions signOptions)
 
/// 
/// Signs source document using given  with digital signature
/// and writes signed document to destination stream.
///Document should be either  or .
///Output will be written to the start of stream and stream size will be updated with content length.
/// 
///The stream which contains the document to sign.
///The stream that signed document will be written to.
/// object with certificate that used to sign file.
/// The certificate in holder MUST contain private keys and have the X509KeyStorageFlags.Exportable flag set.
public static void sign(InputStream srcStream, InputStream dstStream, CertificateHolder certHolder)
 
/// 
/// Signs source document using given  with digital signature
/// and writes signed document to destination file.
///Document should be either  or .
/// 
///The file name of the document to sign.
///The file name of the signed document output.
/// object with certificate that used to sign file.
/// The certificate in holder MUST contain private keys and have the X509KeyStorageFlags.Exportable flag set.
public static void sign(string srcFileName, string dstFileName, CertificateHolder certHolder)
```

4\. Old signing methods in DigitalSignatureUtil are marked as 'Obsolete'

```
public static void sign(string srcFileName, string dstFileName, System.Security.Cryptography.X509Certificates.X509Certificate2 certificate, string comments, DateTime signTime);
public static void sign(string srcFileName, string dstFileName, CertificateHolder certHolder, string comments,DateTime signTime);
public static void sign(string srcFileName, string dstFileName, CertificateHolder certHolder, string comments, DateTime signTime, string srcPassword);
public static void sign(InputStream srcStream, InputStream dstStream, System.Security.Cryptography.X509Certificates.X509Certificate2 certificate, string comments, DateTime signTime);
public static void sign(InputStream srcStream, InputStream dstStream, CertificateHolder certHolder, string comments, DateTime signTime);
public static void sign(InputStream srcStream, InputStream dstStream, CertificateHolder certHolder, string comments, DateTime signTime, string srcPassword);
```

## Other Improvements

There are 104 improvements and fixes in this regular monthly release. The most notable are:

*    Rendering into PCL format (Printer Command Language) was implemented.
*    A significant optimization of PDF rendering engine has been carried out.
*    Performance and heap space optimizations.
*    Compression of document structure data and cross-reference table in PDF 1.5 output. Now the output PDF documents with the logical structure are much smaller.
*    Image tag in Fixed HTML documents can now contain an alternative text string.
*    API for 'Mark Comment Done' option.
*    Sign the signature line in Word document.
*    Add feature to set/get "Specify line and character grid".
*    Detect comment resolved and comment replies and reply to which comment.
*    Added feature to format Data Labels of chart.

## Aspose.Words for Java Resources

The following resources will help you work with Aspose.Words for Java:

*   [Home page for Aspose.Words for Java][11]
*   [Download Aspose.Words for Java][12]
*   [Install Aspose.Words for Java from Maven][13]
*   Aspose.Words product family forum – Post your technical questions and queries, or any other problem you faced while running Aspose.Words APIs.
    *   [Free Support Forum][14]
    *   [Paid Support Forum][15]
*   [Aspose.Words for Java online documentation][16] – Help documentation.
*   [Aspose.Words for Java online API reference][17] - API reference documents.
*   [Enable Blog Subscription][18] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words, APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
*   [Aspose.Words for Java Examples][19] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/words/java/new-releases/aspose.words-for-java-17.8/
[2]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+17.8+Release+Notes
[3]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+17.8+Release+Notes
[4]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java
[5]: https://docs.aspose.com/display/wordsjava/Saving+a+Document#SavingaDocument-SaveDocumenttoPCL
[6]: https://docs.aspose.com/display/wordsjava/Working+with+Document#WorkingwithDocument-SetLinesperPageandNumberofCharactersperLine
[7]: https://docs.aspose.com/display/wordsjava/Working+with+Comments#WorkingwithComments-HowtoReadCommentReply
[8]: https://docs.aspose.com/display/wordsjava/Applying+Formatting+to+Table%2C+Row+and+Cell#ApplyingFormattingtoTable,RowandCell-GetDistancebetweenTableandSurroundingText
[9]: https://docs.aspose.com/display/wordsjava/Working+with+Charts#WorkingwithCharts-HowtoFormatNumberofChartDataLabel
[10]: https://docs.aspose.com/display/wordsjava/Working+with+Digital+Signatures#WorkingwithDigitalSignatures-SigningWordDocuments
[11]: https://www.aspose.com/products/words/java
[12]: https://downloads.aspose.com/words/java
[13]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-words/
[14]: https://forum.aspose.com/c/words
[15]: https://helpdesk.aspose.com/
[16]: https://docs.aspose.com/display/wordsjava/Home
[17]: https://apireference.aspose.com/java/words
[18]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[19]: https://github.com/aspose-words/Aspose.Words-for-Java




