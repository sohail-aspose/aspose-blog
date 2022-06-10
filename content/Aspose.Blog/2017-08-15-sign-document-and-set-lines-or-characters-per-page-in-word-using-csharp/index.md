---
title: 'Sign Document and Set Lines or Characters per Page in Word using C#'
date: Tue, 15 Aug 2017 09:17:39 +0000
draft: false
url: /2017/08/15/sign-document-and-set-lines-or-characters-per-page-in-word-using-csharp/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

We are pleased to announce our next version [Aspose.Words for .NET 17.8][1]. This month’s release contains over 85 useful new features, enhancements and bug fixes. Please see the [release notes][2] for more detail. If you are planning to upgrade from an older version of Aspose.Words to the current version, we would strongly suggest you to check the [Public API and Backward Incompatible Changes][3] section to know what APIs are changed so far.

Here is a look at just a few of the biggest features and API changes in this month’s release.

*   Significant optimization of PDF rendering engine has been carried out.
*   Compression of document structure data and cross-reference table in PDF 1.5 output. Now the output PDF documents with the logical structure are much smaller.
*   Image tag in Fixed HTML documents can now contain an alternative text string.
*   API for 'Mark Comment Done' option.
*   Sign the signature line in Word document.
*   Add feature to set/get "Specify line and character grid".
*   Detect comment resolved and comment replies and reply to which comment.
*   Added feature to format Data Labels of chart.

## Added Public Properties into PageSetup Class Allowing to Define Document Grid

We have added new feature in Aspose.Words for .NET 17.8 to control the behavior of document grid. The LayoutMode, CharactersPerLine, and LinesPerPage properties have added into PageSetup class. Now, you can set and get the number of characters per line and number of lines per page in the document grid.

PageSetup.LayoutMode property has added to get or set the layout mode of a section. Please refer to the following article for more detail:  
[Set Lines per Page and Number of Characters per Line][4]

```
/// <summary>
/// Gets or sets the layout mode of this section.
/// </summary>
public SectionLayoutMode LayoutMode { get; set; }
 
/// <summary>
/// Gets or sets the number of characters per line in the document grid.
/// </summary>
/// <remarks>
/// Minimum value of the property is 1. Maximum value depends on page width and font /// size of the Normal style. Minimum character pitch is 90 percent of the font size. /// For example, maximum number of characters per line of a Letter page with one-inch margins is 43.
/// By default, the property has a value, on which character pitch equals to font size /// of the Normal style.
/// </remarks>
public int CharactersPerLine { get; set; }
 
/// <summary>
/// Gets or sets the number of lines per page in the document grid.
/// </summary>
/// <remarks>
/// Minimum value of the property is 1. Maximum value depends on page height and font size /// of the Normal style. Minimum line pitch is 136 percent of the font size. /// For example, maximum number of lines per page of a Letter page with one-inch margins is 39.
/// By default, the property has a value, on which line pitch is in 1.5 times greater /// than font size of the Normal style.
/// </remarks>
public int LinesPerPage { get; set; }
```

Following public Enum has been added in Aspose.Words 17.8.

```
/// <summary>
/// Specifies the layout mode for a section allowing to define the /// document grid behavior.
/// </summary>
public enum SectionLayoutMode
{
    /// <summary>
    /// Specifies that no document grid shall be applied to the contents of the     /// corresponding section in the document.
    /// </summary>
    Default,
 
    /// <summary>
    /// Specifies that the corresponding section shall have both the additional line     /// pitch and character pitch added to
    /// each line and character within it in order to maintain a specific number of     /// lines per page and characters per line.
    /// Characters will not be automatically aligned with grid lines on typing.
    /// </summary>
    Grid,
 
    /// <summary>
    /// Specifies that the corresponding section shall have additional line pitch     /// added to each line within it in order
    /// to maintain the specified number of lines per page.
    /// </summary>
    LineGrid,
 
    /// <summary>
    /// Specifies that the corresponding section shall have both the additional line     /// pitch and character pitch added to
    /// each line and character within it in order to maintain a specific number of     /// lines per page and characters per line.
    /// Characters will be automatically aligned with grid lines on typing.
    /// </summary>
    SnapToChars
}
```

Note : The Document Grid tab becomes visible in the Page Setup dialog of MS Word if any Asian language is defined as editing language.

## Detect Comment Resolved and Comment Replies and Reply to Which Comment

We have added read-only public API to get extended comment properties.  You can read the comment and resolve it. Comment.Replies property returns a collection of Comment objects that are immediate children of the specified comment. Please refer to the following article:  
[How to Read Comment's Reply][5]

Following methods have added to the Comment class.

```
// Returns the parent Comment object. Returns null for top-level comments.
public Comment Ancestor
 
// Returns a collection of  objects that are immediate children of the specified comment.
public CommentCollection Replies
 
// Gets or sets flag indicating that the comment has been marked done.
public bool Done
```

## DistanceLeft, DistanceRight, DistanceTop, DistanceBottom Properties Added in Table Class

A new feature has added in Aspose.Words 17.8 to get the distance between table and its surrounding text when text Wrapping of table is "Around". Please refer to the following article:  
[Get Distance between Table and Surrounding Text][6]

```
// Gets distance between table left and the surrounding text, in points.
public double DistanceLeft
 
// Gets distance between table right and the surrounding text, in points.
public double DistanceRight
 
// Gets distance between table top and the surrounding text, in points.
public double DistanceTop
 
// Gets distance between table bottom and the surrounding text, in points.
public double DistanceBottom
```

## Compression of Document Structure Data and Cross-Reference Table in PDF 1.5 Output

Now document structure data and cross-reference table are compressed when saving to PDF 1.5. This changes do not affect PDF/A-1 output due to limitations in specification.

## Added Public Property ChartDataLabel.NumberFormat

We have added new feature in Aspose.Words for .NET 17.8 to format chart's data label. Please refer to the following article:  
[How to Format Number of Chart Data Label][7]

```
/// Returns number format of the parent element.
public ChartNumberFormat NumberFormat
```

ChartNumberFormat class represents number formatting of the parent element and contains the following public properties

```
 /// <summary>
/// Gets or sets the format code applied to a data label.
/// </summary>
/// <remarks>
/// Number formatting is used to change the way a value appears in data label and can be used in some very creative ways.
/// The examples of number formats:
/// <para>Number - "#,##0.00"</para>
/// <para>Currency - "\"$\"#,##0.00"</para>
/// <para>Time - "\[$-x-systime\]h:mm:ss AM/PM"</para>
/// <para>Date - "d/mm/yyyy"</para>
/// <para>Percentage - "0.00%"</para>
/// <para>Fraction - "# ?/?"</para>
/// <para>Scientific - "0.00E+00"</para>
/// <para>Text - "@"</para>
/// <para>Accounting - "_-\"$\"\* #,##0.00_-;-\"$\"\* #,##0.00_-;_-\"$\"\* \"-\"??_-;_-@_-"</para>
/// <para>Custom with color - "\[Red\]-#,##0.0"</para>
/// </remarks>
public string FormatCode

/// <summary>
/// Specifies whether the format code is linked to a source cell.
/// Default is true.
/// </summary>
/// <remarks>The NumberFormat will be reset to general if format code is linked to source.</remarks>
public bool IsLinkedToSource 
```

## Implemented Signing Signature Line in Word Documents

We have added new feature in Aspose.Words 17.8 to sign signature line in Word document. Please read following article:  
[Signing Word Documents][8]

Please check the following API changes.

1\. Added new public property for SignatureLine class:

```
 /// <summary>
/// Gets or sets identifier for this signature line.
/// This identifier can be associated with a digital signature, when signing document using <see cref="DigitalSignatureUtil"/>.
/// This value must be unique and by default it is randomly generated with <see cref="Guid.NewGuid"/>.
/// </summary>
public Guid Id
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
 /// <summary>
/// Specifies comments on the digital signature.
/// Default value is <see cref="string.Empty"/>.
/// </summary>
public string Comments
 
/// <summary>
/// The date of signing.
/// Default value is <see cref="DateTime.Now"/>.
/// </summary>
public DateTime SignTime
 
/// <summary>
/// Signature line identifier.
/// Default value is <see cref="Guid.Empty"/>.
/// </summary>
/// <remarks>
/// When set, it associates <see cref="SignatureLine"/> with corresponding <see cref="DigitalSignature"/>.
/// </remarks>
public Guid SignatureLineId
 
/// <summary>
/// The image that will be shown in associated <see cref="SignatureLine"/>.
/// Default value is <c>null</c>.
/// </summary>
public byte[] SignatureLineImage
 
/// <summary>
/// The password to decrypt source document.
/// Default value is <see cref="string.Empty"/>.
/// </summary>
/// <remarks>
/// If OOXML document is encrypted, you should provide decryption password
/// to decrypt source document before it will be signed.
/// This is not required for documents in binary DOC format.
/// </remarks>
public string DecryptionPassword 
```

3\. New public methods are introduced in DigitalSignatureUtil class for signing documents:

```
 /// <summary>
 /// Signs source document using given <see cref="CertificateHolder"/> and <see cref="SignOptions"/>
 /// with digital signature and writes signed document to destination stream.
 /// Document should be either <see cref="LoadFormat.Doc"/> or <see cref="LoadFormat.Docx"/>.
 /// <b>Output will be written to the start of stream and stream size will be updated with content length.</b>
 /// </summary>
 /// <param name="srcStream">The stream which contains the document to sign.</param>
 /// <param name="dstStream">The stream that signed document will be written to.</param>
 /// <param name="certHolder"><see cref="CertificateHolder"/> object with certificate that used to sign file.
 /// <ms>The certificate in holder MUST contain private keys and have the X509KeyStorageFlags.Exportable flag set.</ms></param>
 /// <param name="signOptions"><see cref="SignOptions"/> object with various signing options.</param>
 public static void Sign(Stream srcStream, Stream dstStream, CertificateHolder certHolder, SignOptions signOptions)
 
/// <summary>
/// Signs source document using given <see cref="CertificateHolder"/> and <see cref="SignOptions"/>
/// with digital signature and writes signed document to destination file.
/// Document should be either <see cref="LoadFormat.Doc"/> or <see cref="LoadFormat.Docx"/>.
/// </summary>
/// <param name="srcFileName">The file name of the document to sign.</param>
/// <param name="dstFileName">The file name of the signed document output.</param>
/// <param name="certHolder"><see cref="CertificateHolder"/> object with certificate that used to sign file.
/// <ms>The certificate in holder MUST contain private keys and have the X509KeyStorageFlags.Exportable flag set.</ms></param>
/// <param name="signOptions"><see cref="SignOptions"/> object with various signing options.</param>
public static void Sign(string srcFileName, string dstFileName, CertificateHolder certHolder, SignOptions signOptions)
 
/// <summary>
/// Signs source document using given <see cref="CertificateHolder"/> with digital signature
/// and writes signed document to destination stream.
/// Document should be either <see cref="LoadFormat.Doc"/> or <see cref="LoadFormat.Docx"/>.
/// <b>Output will be written to the start of stream and stream size will be updated with content length.</b>
/// </summary>
/// <param name="srcStream">The stream which contains the document to sign.</param>
/// <param name="dstStream">The stream that signed document will be written to.</param>
/// <param name="certHolder"><see cref="CertificateHolder"/> object with certificate that used to sign file.
/// <ms>The certificate in holder MUST contain private keys and have the X509KeyStorageFlags.Exportable flag set.</ms></param>
public static void Sign(Stream srcStream, Stream dstStream, CertificateHolder certHolder)
 
/// <summary>
/// Signs source document using given <see cref="CertificateHolder"/> with digital signature
/// and writes signed document to destination file.
/// Document should be either <see cref="LoadFormat.Doc"/> or <see cref="LoadFormat.Docx"/>.
/// </summary>
/// <param name="srcFileName">The file name of the document to sign.</param>
/// <param name="dstFileName">The file name of the signed document output.</param>
/// <param name="certHolder"><see cref="CertificateHolder"/> object with certificate that used to sign file.
/// <ms>The certificate in holder MUST contain private keys and have the X509KeyStorageFlags.Exportable flag set.</ms></param>
public static void Sign(string srcFileName, string dstFileName, CertificateHolder certHolder) 
```

4\. Old signing methods in DigitalSignatureUtil are marked as 'Obsolete'

```
public static void Sign(string srcFileName, string dstFileName, System.Security.Cryptography.X509Certificates.X509Certificate2 certificate, string comments, DateTime signTime);
public static void Sign(string srcFileName, string dstFileName, CertificateHolder certHolder, string comments,DateTime signTime);
public static void Sign(string srcFileName, string dstFileName, CertificateHolder certHolder, string comments, DateTime signTime, string srcPassword);
public static void Sign(Stream srcStream, Stream dstStream, System.Security.Cryptography.X509Certificates.X509Certificate2 certificate, string comments, DateTime signTime);
public static void Sign(Stream srcStream, Stream dstStream, CertificateHolder certHolder, string comments, DateTime signTime);
public static void Sign(Stream srcStream, Stream dstStream, CertificateHolder certHolder, string comments, DateTime signTime, string srcPassword);
```

## Aspose.Words for .NET Resources

The following resources will help you work with Aspose.Words for .NET:

*   [Home page of .NET API][9].
*   [Download Section][10].
*   [Install using NuGet Package][11]
*   [Documentation][12] – up-to-date documentation containing Programmer’s Guide, Knowledge Base and much more.
*   [API Reference Guide][13] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   Aspose.Words Product Family Forum – post your technical questions and queries, or any other problem you are facing while working with Aspose.Words APIs.
    *   [Free Support Forum][14]
    *   [Paid Support Forum][15]
*   [Enable Blog Subscription][16] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
*   [Examples][17] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/words/net/new-releases/aspose.words-for-.net-17.8/
[2]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+17.8+Release+Notes
[3]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET
[4]: https://docs.aspose.com/display/wordsnet/Working+with+Document#WorkingwithDocument-SetLinesperPageandNumberofCharactersperLine
[5]: https://docs.aspose.com/display/wordsnet/Working+with+Comments#WorkingwithComments-HowtoReadComment'sReply
[6]: https://docs.aspose.com/display/wordsnet/Applying+Formatting#ApplyingFormatting-GetDistancebetweenTableandSurroundingText
[7]: https://docs.aspose.com/display/wordsnet/Working+with+Charts#WorkingwithCharts-HowtoFormatNumberofChartDataLabel
[8]: https://docs.aspose.com/display/wordsnet/Working+with+Digital+Signatures#WorkingwithDigitalSignatures-SigningWordDocuments
[9]: https://www.aspose.com/products/words/net
[10]: https://downloads.aspose.com/words/net
[11]: https://www.nuget.org/packages/Aspose.Words/
[12]: https://docs.aspose.com/display/wordsnet
[13]: https://apireference.aspose.com/net/words
[14]: https://forum.aspose.com/c/words
[15]: https://helpdesk.aspose.com/
[16]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[17]: https://github.com/aspose-words/Aspose.Words-for-.NET




