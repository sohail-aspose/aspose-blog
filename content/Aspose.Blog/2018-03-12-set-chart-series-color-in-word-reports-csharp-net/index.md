---
title: 'Set Chart Series Color in Word Reports using LINQ Reporting Engine in C# .NET'
date: Mon, 12 Mar 2018 11:29:57 +0000
draft: false
url: /2018/03/12/set-chart-series-color-in-word-reports-csharp-net/
author: Tahir Manzoor
summary: ''
tags: ['Dynamically generate chart series in Word reports', 'Set chart series color in the Word reports']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose-Words-for-net.png" alt="Aspose.Words for .NET logo">}}


We are pleased to announce our next version [Aspose.Words for .NET 18.3][1]. This month’s release contains over 67 useful new features, enhancements and bug fixes. Please see the [release notes][2] for more detail. If you are planning to upgrade from older version of Aspose.Words to the current version, we would strongly suggest you to check the [Public API and Backward Incompatible Changes][3] section to know what APIs are changed so far.

Here is a look at just a few of the biggest features and API changes in this month’s release.

*   LINQ Reporting Engine supports dynamic coloring of chart series and individual series points
*   Add support of CssClassNamesPrefix in HtmlSaveOptions
*   A number of obsolete properties were removed from PdfSaveOptions class. Please refer to public API changes section for details
*   PdfSaveOptions.EscapeUri property was added to allow the usage of custom URI strings without the automatic escape while rendering into PDF
*   The automatic font color calculation now takes the fill of the background shape into account while rendering
*   Added fallback rendering for Unicode range \[U+1F300; U+1F5FF\] - Miscellaneous Symbols and Pictographs; This range includes such symbols as Emoji and alike
*   Implemented processing of empty EMR\_EXTTEXTOUTW records in metafiles rendering
*   Improved rendering of DML Chart plot area with a manual layout. The additional offset is calculated for the rotated labels of horizontal axis
*   Fixed a bug where the gradient brush with transformation would mess up the texture upon rendering. Texture scaling improved
*   Fixed a problem of axis scaling when rendering DML Charts with Arial Narrow font
*   Fixed a bug causing freezes when converting to PDF a document with DML Charts with a huge number of data points
*   Fixed a symbol positioning bug when rendering MathML equations
*   A reflection effect is now applied correctly for 3D rotated WordArt objects

## Set Chart Series Color and Individual Series Points

In this version of Aspose.Words, we have added the support to set the color of chart series and individual series points using LINQ Reporting. Please read the following article for more detail.

*   [Using Charts to Represent Sequential Data][4]

## Added Property PdfSaveOptions.EscapeUri

In some cases, you may want to encode the URI e.g. encode "/" character to the "%2F". Starting from Aspose.Words 18.3, we have added support to escape the URI before writing it into PDF. Please refer to the following article for more detail:

*   [Escape the URI in Output PDF][5]

```
/// <summary>
/// A flag specifying whether URI should be escaped before writing.
/// </summary>
/// <remarks>
/// Note that if this option is set to <c>false</c> hyperlinks are written "as is",
/// so valid (escaped) URI should be provided in document's model.
/// <para>The default value is <c>true</c>.</para>
/// </remarks>
public bool EscapeUri
{get;set;}
```

## Added Property HtmlSaveOptions.CssClassNamePrefix

We have added a new feature in this release to add a prefix to all CSS class names when the document is exported to HTML. A new property HtmlSaveOptions.CssClassNamePrefix has been added in Aspose.Words 18.3. Please read the following article for more detail.

*   [Add Prefix to CSS Class Name][6]

```
/// <summary>
/// Specifies a prefix which is added to all CSS class names.
/// Default value is an empty string and generated CSS class names have no common prefix.
/// </summary>
/// <remarks>
/// <para>If this value is not empty, all CSS classes generated by Aspose.Words will start with the specified prefix.
/// This might be useful, for example, if you add custom CSS to generated documents and want to prevent class
/// name conflicts.</para>
/// <para>If the value is not <c>null</c> or empty, it must be a valid CSS identifier.</para>
/// </remarks>
/// <exception cref="ArgumentException">The value is not empty and is not a valid CSS identifier.</exception>
public string CssClassNamePrefix
{
    get { return mCssClassNamesPrefix; }
    set
    {
        if (StringUtil.HasChars(value) && !CssEscape.IsValidIdentifier(value))
            throw new ArgumentException("The class name prefix must be a valid CSS identifier.");
        mCssClassNamesPrefix = value;
    }
}
```

## Obsolete Properties and Methods

The following obsolete properties and methods have been removed:

*   Obsolete method FormFieldCollection.Remove was removed. Please use the FormField.RemoveField method instead.
*   Obsolete property MailMerge.RemoveEmptyParagraphs was removed. Please use the MailMerge.CleanupOptions property instead.
*   Obsolete property MailMerge.RemoveEmptyRegions was removed. Please use the MailMerge.CleanupOptions property instead.
*   Obsolete property MailMerge.RtlCleanupMode was removed.
*   Obsolete value GeneralFormat.Auieo was removed. Please use the GeneralFormat.Aiueo value instead.

## Removed Obsolete Properties from PdfSaveOptions

The following obsolete properties have been removed from the PdfSaveOptions class:

<figure class="wp-block-table"><table class=""><tbody><tr><td>**Removed property</strong></td><td><strong>Property to use instead**</td></tr><tr><td>HeadingsOutlineLevels</td><td>OutlineOptions.HeadingsOutlineLevels</td></tr><tr><td>ExpandedOutlineLevels</td><td>OutlineOptions.ExpandedOutlineLevels</td></tr><tr><td>BookmarksOutlineLevel</td><td>OutlineOptions.DefaultBookmarksOutlineLevel</td></tr><tr><td>EmbedStandardWindowsFonts</td><td>FontEmbeddingMode</td></tr><tr><td>ExportCustomPropertiesAsMetadata</td><td>CustomPropertiesExport</td></tr><tr><td>MetafileRenderingMode</td><td>MetafileRenderingOptions.RenderingMode</td></tr><tr><td>DownsampleImages</td><td>DownsampleOptions.DownsampleImages</td></tr><tr><td>DownsampleResolution</td><td>DownsampleOptions.Resolution</td></tr></tbody></table></figure>

We have also removed obsolete PdfDigitalSignatureDetails constructor and PdfDigitalSignatureDetails.Certificate property which works System.Security.Cryptography.X509Certificates.X509Certificate2. Please use CertificateHolder instead.

## Aspose.Words for .NET Resources

The following resources will help you work with Aspose.Words for .NET:

1.  [Home page of .NET API][7].
2.  [Install using NuGet Package][8]
3.  [Documentation][9] – up-to-date documentation containing Programmer’s Guide, Knowledge Base and much more.
4.  [API Reference Guide][10] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
5.  Aspose.Words Product Family Forum – post your technical questions and queries, or any other problem you are facing while working with Aspose.Words APIs.
    *   [Free Support Forum][11]
    *   [Paid Support Forum][12]
6.  [Enable Blog Subscription][13] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
7.  [Examples][14] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Words/
[2]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+18.3+Release+Notes
[3]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET
[4]: https://docs.aspose.com/display/wordsnet/Template+Syntax#TemplateSyntax-UsingChartstoRepresentSequentialData
[5]: https://docs.aspose.com/display/wordsnet/Rendering#Rendering-EscapetheURIinOutputPDF
[6]: https://docs.aspose.com/display/wordsnet/Saving+a+Document#SavingaDocument-AddPrefixtoCSSClassName
[7]: https://products.aspose.com/words/net
[8]: https://www.nuget.org/packages/Aspose.Words/
[9]: https://docs.aspose.com/display/wordsnet
[10]: https://apireference.aspose.com/net/words
[11]: https://forum.aspose.com/c/words
[12]: https://helpdesk.aspose.com/
[13]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[14]: https://github.com/aspose-words/Aspose.Words-for-.NET




