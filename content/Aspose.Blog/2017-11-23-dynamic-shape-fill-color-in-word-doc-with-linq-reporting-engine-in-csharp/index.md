---
title: 'Dynamic Shape Fill Color in Word Documents using LINQ Reporting Engine - C#'
date: Thu, 23 Nov 2017 10:54:47 +0000
draft: false
url: /2017/11/23/dynamic-shape-fill-color-in-word-doc-with-linq-reporting-engine-in-csharp/
author: Tahir Manzoor
summary: ''
tags: ['Dynamic Shape Fill Color in Word']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose-Words-for-net.png" alt="Aspose.Words for .NET logo">}}


We are pleased to announce our next version [Aspose.Words for .NET 17.11][1]. This month’s release contains over 102 useful new features, enhancements and bug fixes. Please see the [release notes][2] for more detail. If you are planning to upgrade from older version of Aspose.Words to the current version, we would strongly suggest you to check the [Public API and Backward Incompatible Changes][3] section to know what APIs are changed so far.

Here is a look at just a few of the biggest features and API changes in this month’s release.

*   LINQ Reporting Engine supports dynamic shape background coloring.
*   Improved optional hyphen handling and fixed related infinite loop issue.
*   Improved floating table re-breaking in specific scenarios where content of a table used to be lost outside of a page.
*   Improved table grid computation when cells contain tab characters.
*   Further improved character spacing control handling.
*   PCL documents rendering improved. UCS-2 symbol sets can now be mapped to the printer built-in fonts – it allows to print non-ascii symbols with built-in fonts if supported by printer.
*   A ‘cosmetic’ pen (i.e. pen with fixed 1-pixel width) rendering improved in metafile output documents.
*   Font metrics calculation affecting the vertical positioning of text for GDI+ output rendering improved.
*   Added fallback for strokes with unsupported binary raster operations in metafile rendering.
*   Gamma-correction flag is now taken into account while rendering metafiles brushes.
*   Metafile warnings improved:
    *   Added warnings for unsupported binary raster operations.
    *   Removed warnings about unsupported metafile records which do not affect the output.

## Supported Dynamic Shape Fill Color Setting for LINQ Reporting Engine

We have introduced a new feature in this version of Aspose.Words to set the fill color of the Shape node using LINQ Reporting. Please refer to the following article for more detail.

*   [Setting Background Color Dynamically][4]

## Added Word2016 Constant into MsWordVersion Enumeration Type

The following constant is added into the MsWordVersion enumeration type.

```
/// <summary>
/// Optimize Aspose.Words behavior to match MS Word 2016 version.
/// </summary>
Word2016
```

It can be passed into the CompatibilityOptions.OptimizeFor method to optimize the document contents as well as Aspose.Words behavior to match MS Word 2016 version. Please read the following article for more detail. 

*   [Optimize Document to Particular MS Word Version][5]

## Added Feature to Set File Name and Extension of Ole Object

We have added public property OleFormat.OlePackage to provide the ability to set the file name, extension, and display name for OLE Package when inserting ole object using MemoryStream. Please refer to the following article for more detail.

*   [Set File Name and Extension when Inserting Ole Object][6]

```
public class OlePackage
{
    /// <summary>
    /// Gets or sets OLE Package file name.
    /// </summary>
    public string FileName { get; set;}
 
    /// <summary>
    /// Gets or sets OLE Package display name.
    /// </summary>
    public string DisplayName { get; set;}
}
```

## Changed Behavior of Range.Replace Methods

Behaviour of the following methods of the Range class is changed.

```
public int Replace(string pattern, string replacement, FindReplaceOptions options);
public int Replace(Regex pattern, string replacement, FindReplaceOptions options);
```

Now headers/footers of a section are processed in this order:

*   If Section.PageSetup.DifferentFirstPageHeaderFooter is ‘True’:
    1.  First header
    2.  First footer
    3.  Even header
    4.  Even footer
    5.  Primary header
    6.  Primary footer
*   If Section.PageSetup.DifferentFirstPageHeaderFooter is ‘False’:
    1.  Primary header
    2.  Primary footer
    3.  Even header
    4.  Even footer

## Remove Obsolete Methods in DigitalSignatureUtil

We have removed following obsolete public methods from DigitalSignatureUtil class:

```
public static void Sign(string srcFileName, string dstFileName, System.Security.Cryptography.X509Certificates.X509Certificate2 certificate, string comments, DateTime signTime);
public static void Sign(string srcFileName, string dstFileName, CertificateHolder certHolder, string comments,DateTime signTime);
public static void Sign(string srcFileName, string dstFileName, CertificateHolder certHolder, string comments, DateTime signTime, string srcPassword);
public static void Sign(Stream srcStream, Stream dstStream, System.Security.Cryptography.X509Certificates.X509Certificate2 certificate, string comments, DateTime signTime);
public static void Sign(Stream srcStream, Stream dstStream, CertificateHolder certHolder, string comments, DateTime signTime);
public static void Sign(Stream srcStream, Stream dstStream, CertificateHolder certHolder, string comments, DateTime signTime, string srcPassword); 
```

Instead, the methods with SignOptions class should be used. Please refer to the following release notes.

*   [Implemented Signing Signature Line in Word Documents][7] (17.8 release notes)
*   [Provided API Similar to SignatureSet.AddSignatureLine Method in MS Office][8] (17.10 release notes)

## Metafile Warnings Improved

We have improved following metafile warnings in this version of Aspose.Words.

*   Added warnings for unsupported binary raster operations. Also added fallback to bitmap rendering in this case on .NET platform.
*   Removed warnings about unsupported metafile records which do not affect the output.
*   Changed type of warnings about unsupported metafile records from DataLoss/UnexpectedContent to more appropriate MinorFormattingLoss.

## Added Feature to Get Position of Floating Table

A new feature has been added in this release to get the position of the floating table. Please refer to the following article.

*   [Get Position of Floating Table][9]

We have added new public properties for floating tables in Table class:

```
/// <summary>
/// Gets the base object from which the horizontal positioning in the <see cref="AbsoluteHorizontalDistance"/>
/// and/or <see cref="RelativeHorizontalAlignment"/> attribute should be calculated.
/// Default value is <see cref="RelativeHorizontalPosition.Column"/>.
/// </summary>
public RelativeHorizontalPosition HorizontalAnchor
 
/// <summary>
/// Gets the base object from which the vertical positioning in the <see cref="AbsoluteVerticalDistance"/>
/// attribute should be calculated.
/// Default value is <see cref="RelativeVerticalPosition.Margin"/>.
/// </summary>
public RelativeVerticalPosition VerticalAnchor
 
/// <summary>
/// Gets table absolute horizontal position relative to the horizontal anchor
/// specified by the <see cref="HorizontalAnchor"/>, in points.
/// Default value is 0.
/// </summary>
public double AbsoluteHorizontalDistance
 
/// <summary>
/// Gets table absolute vertical position relative to the vertical anchor
/// specified by the <see cref="VerticalAnchor"/>, in points.
/// Default value is 0.
/// </summary>
public double AbsoluteVerticalDistance
 
/// <summary>
/// Gets whether a floating table shall allow other floating tables in the document
/// to overlap its extents when displayed.
/// Default value is <c>true</c>.
/// </summary>
public bool AllowOverlap
```

## Aspose.Words for .NET Resources

The following resources will help you work with Aspose.Words for .NET:

1.  [Home page of .NET API][10].
2.  [Download Section][11].
3.  [Install using NuGet Package][12].
4.  [Documentation][13] – up-to-date documentation containing Programmer’s Guide, Knowledge Base, and much more.
5.  [API Reference Guide][14] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
6.  Aspose.Words Product Family Forum – post your technical questions and queries, or any other problem you are facing while working with Aspose.Words APIs.
    *   [Free Support Forum][15]
    *   [Paid Support Forum][16]
7.  [Enable Blog Subscription][17] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
8.  [Examples][18] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/words/net/new-releases/aspose.words-for-.net-17.11/
[2]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+17.11+Release+Notes
[3]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET
[4]: https://docs.aspose.com/display/wordsnet/Template+Syntax#TemplateSyntax-SettingBackgroundColorDynamically
[5]: https://docs.aspose.com/display/wordsnet/Working+with+Document#WorkingwithDocument-OptimizeDocumenttoParticularMSWordVersion
[6]: https://docs.aspose.com/display/wordsnet/Use+DocumentBuilder+to+Insert+Document+Elements#UseDocumentBuildertoInsertDocumentElements-SetFileNameandExtensionwhenInsertingOleObject
[7]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+17.8+Release+Notes
[8]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+17.10+Release+Notes
[9]: https://docs.aspose.com/display/wordsnet/Applying+Formatting#ApplyingFormatting-GetPositionofFloatingTable
[10]: https://www.aspose.com/products/words/net
[11]: https://downloads.aspose.com/words/net
[12]: https://www.nuget.org/packages/Aspose.Words/
[13]: https://docs.aspose.com/display/wordsnet
[14]: https://apireference.aspose.com/net/words
[15]: https://forum.aspose.com/c/words
[16]: https://helpdesk.aspose.com/
[17]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[18]: https://github.com/aspose-words/Aspose.Words-for-.NET




