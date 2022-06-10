---
title: 'Support of One Bit Pixel Image Add Remove Comment Reply Footnote Layout Columns and Use Machine Fonts in HtmlFixed'
date: Fri, 13 Oct 2017 09:44:33 +0000
draft: false
url: /2017/10/13/aspose-words-for-net-release-17.10/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

[](https://www.aspose.com/products/words/net)We are pleased to announce our next version [Aspose.Words for .NET 17.10][1]. This month’s release contains over 76 useful new features, enhancements and bug fixes. Please see the [release notes][2] for more detail. If you are planning to upgrade from older version of Aspose.Words to the current version, we would strongly suggest you to check the [Public API and Backward Incompatible Changes][3] section to know what APIs are changed so far.

  
Here is a look at just a few of the biggest features and API changes in this month’s release.

*   "Don't add extra space for raised/lowered characters" compatibility option is supported.
*   Multiple improvements in RTL and Asian text handling.
*   LINQ Reporting Engine supports dynamic chart series removal.
*   ‘Black and white’ images with one bit per pixel format rendering implemented. PixelFormat.Format1bppIndexed was introduced.
*   An option to prevent the fonts embedding into HTML Fixed output implemented. Introduced HtmlFixedSaveOptions.UseTargetMachineFonts property.
*   Rendering of HTML fixed documents with “PRC” encoding fonts has been improved.
*   An algorithm, which mimics the behavior of MS Word when rendering of rotated VML shapes with text boxes.
*   Rendering of “Surface” and “Stock” DrawingML Charts has been improved.
*   Added CompareOptions.Target property and enumeration ComparisonTargetType.
*   Added public methods to add and remove replies to comment.
*   Ability to get and set the number of footnote layout columns.
*   Provide API similar to SignatureSet.AddSignatureLine Method (Office).
*   Expose Table.HorizontalAlignment property public.

## Added Public Property CompareOptions.Target and Enumeration ComparisonTargetType

A new feature has been added in this release to use the base document during comparison of documents. This feature is related to Microsoft Word _"Show changes in"_ option in _"Compare Documents"_ dialog box. We have added Public property CompareOptions.Target to the CompareOptions class to provide ability to determine base document upon documents comparison. Please read following article for more detail.  
[Set Target Document for Comparison Differences][4]

```
/// <summary>
/// Specifies which document shall be used as a target during comparison.
/// </summary>
public ComparisonTargetType Target
{
  get { return mTargetType; }
  set { mTargetType = value; }
} 
```
```
/// <summary>
/// Allows to specify base document which will be used during comparison.    
/// Default value is <see cref="Current" />.
/// </summary>
/// <remarks>
/// Relates to Microsoft Word "Show changes in" option in "Compare Documents" dialog box.
/// </remarks>
public enum ComparisonTargetType
{
  /// <summary>
  /// This document is used as a base during comparison.
  /// </summary>
  Current,
 
 
  /// <summary>
  /// Other document is used as a base during comparison.
  /// </summary>
  New
} 
```

## LINQ Reporting Engine Supports Dynamic Chart Series Removal

We have added a new feature in LINQ Reporting Engine to remove chart series dynamically. In particular, this feature is useful when you need to restrict access to sensitive data in chart series for some users of your application. Please read more detail from here.  
[Using Charts to Represent Sequential Data][5]

## Added Feature to Add and Remove Comment Reply

We have added public methods Comment.AddReply and Comment.RemoveReply in this version of Aspose.Words to add and remove comment's reply. Please refer to the following article for more detail.   
[How to Add and Remove Comment's Reply][6]

```
/// <summary>
/// Adds a reply to this comment.
/// </summary>
/// <param name="author">The author name for the reply.</param>
/// <param name="initial">The author initials for the reply.</param>
/// <param name="dateTime">The date and time for the reply.</param>
/// <param name="text">The reply text.</param>
/// <returns>The created <see cref="Comment"/> node for the reply.</returns>
/// <remarks>
/// Due to the existing MS Office limitations only 1 level of replies is allowed in the document.
/// An exception of type <see cref="InvalidOperationException"/> will be raised if this method is
/// called on the existing Reply comment.
/// </remarks>
public Comment AddReply(string author, string initial, DateTime dateTime, string text);
 
/// <summary>
/// Removes the specified reply to this comment.
/// </summary>
/// <param name="reply">The comment node of the deleting reply.</param>
/// <remarks>All constituent nodes of the reply will be deleted from the document.</remarks>
public void RemoveReply(Comment reply);
 
/// <summary>
/// Removes all replies to this comment.
/// </summary>
/// <remarks>All constituent nodes of the replies will be deleted from the document.</remarks>
public void RemoveAllReplies(); 
```

## Added Feature to Save Black and White Image with One Bit Per Pixel Format

A new enumeration value Format1bppIndexed has been added to ImagePixelFormat for ImageSaveOptions.PixelFormat property. Previously setting ImageSaveOptions.ImageColorMode as BlackAndWhite would produce black and white image but with more than one bit per pixel format. For now black and white image with one bit per pixel format could be produced using Aspose.Words 17.10. Please read following article for detail.  
[Save Black and White Image with One Bit Per Pixel Format][7]

## Added Feature to Get and Set Number of Footnote Layout Columns

We have added public property FootnoteOptions.Columns to set or get the number of columns with which the footnotes area is formatted. Please read following article for more detail.  
[Working with Footnote and Endnote][8]

```
/// <summary>
/// Specifies the number of columns with which the footnotes area is formatted.
/// </summary>
/// <remarks>
/// If this property has the value of 0, the footnotes area is formatted with a   
/// number of columns based on the number of columns on the displayed page.   
/// The default value is 0.
/// </remarks>
public int Columns { get; set; }
```

The Document.EndnoteOptions and PageSetup.EndnoteOptions properties have been changed to be of the EndnoteOptions type. This new EndnoteOptions class has the same properties as FootnoteOptions except the Columns property:

```
/// <summary>
/// Represents the endnote numbering options for a document or section.
/// </summary>
public class EndnoteOptions
{
    /// <summary>
    /// Specifies the endnotes position.
    /// </summary>
    public EndnotePosition Position { get; set; }
 
    /// <summary>
    /// Specifies the number format for automatically numbered endnotes.
    /// </summary>
    public NumberStyle NumberStyle { get; set; }
 
    /// <summary>
    /// Specifies the starting number or character for the first automatically numbered endnotes.
    /// </summary>
    public int StartNumber { get; set; }
 
    /// <summary>
    /// Determines when automatic numbering restarts.
    /// </summary>
    public FootnoteNumberingRule RestartRule { get; set; }
} 
```

The similar Position property of the FootnotePosition type is added into the FootnoteOptions class. The property should be used instead of the obsolete Location property. The new public enum types FootnotePosition and EndnotePosition have the following items:

```
/// <summary>
/// Defines the footnote position.
/// </summary>
public enum FootnotePosition
{
    /// <summary>
    /// Footnotes are output at the bottom of each page.
    /// </summary>
    BottomOfPage = 1,
 
    /// <summary>
    /// Footnotes are output beneath text on each page.
    /// </summary>
    BeneathText = 2
}
 
/// <summary>
/// Defines the endnote position.
/// </summary>
public enum EndnotePosition
{
    /// <summary>
    /// Endnotes are output at the end of the section.
    /// </summary>
    EndOfSection = 0,
 
    /// <summary>
    /// Endnotes are output at the end of the document.
    /// </summary>
    EndOfDocument = 3
}
```

## Added Feature to Sign Word document using Signature Provider Identifier

We have Added public properties SignOptions.ProviderId and SignatureLine.ProviderId in this version of Aspose.Words to sign Word document using signature provider identifier. Please refer to the following articles.  
[Signing Word Document using Signature Provider Identifier][9]  
[Create New Signature Line Sign Word Document using Provider Identifier][10]

## Added Feature to Get to Relative Alignment of Table

A new feature has been added in this release to get the table's alignment. You can get the relative table's alignment using Table.RelativeHorizontalAlignment and Table.RelativeVerticalAlignment properties when its text wrapping is "Around". Please read following article for more detail.  
[How to Get the Table Alignment][11]

```
// Gets table relative horizontal alignment.
public HorizontalAlignment RelativeHorizontalAlignment
 
// Gets table relative vertical alignment.
public VerticalAlignment RelativeVerticalAlignment 
```

## Prevent Embedding Fonts while Saving into HTML Fixed Format

We have introduced HtmlFixedSaveOptions.UseTargetMachineFonts property to use fonts from target machine when document is saved to HtmlFixed. For more detail, please check following link.   
[Prevent Embedding Fonts while saving Document into HtmlFixed][12]

```
 /// <summary>
/// Flag indicates whether fonts from target machine must be used to display the document.
/// If this flag is set to true, <see cref="FontFormat"/> and <see cref="ExportEmbeddedFonts"/> properties do not have effect,
/// also <see cref="ResourceSavingCallback"/> is not fired for fonts.
/// Default is false.
/// </summary>
public bool UseTargetMachineFonts 
```

## Aspose.Words for .NET Resources

The following resources will help you work with Aspose.Words for .NET:

*   [Home page of .NET API][13].
*   [Download Section][14].
*   [Install using NuGet Package][15]
*   [Documentation][16] – up-to-date documentation containing Programmer’s Guide, Knowledge Base and much more.
*   [API Reference Guide][17] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   Aspose.Words Product Family Forum – post your technical questions and queries, or any other problem you are facing while working with Aspose.Words APIs.
    *   [Free Support Forum][18]
    *   [Paid Support Forum][19]
*   [Enable Blog Subscription][20] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
*   [Examples][21] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/words/net/new-releases/aspose.words-for-.net-17.10/
[2]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+17.10+Release+Notes
[3]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET
[4]: https://docs.aspose.com/display/wordsnet/Working+with+Document#WorkingwithDocument-SetTargetDocumentforComparisonDifferences
[5]: https://docs.aspose.com/display/wordsnet/Template+Syntax#TemplateSyntax-UsingChartstoRepresentSequentialData
[6]: https://docs.aspose.com/display/wordsnet/Working+with+Comments#WorkingwithComments-HowtoAddandRemoveComment'sReply
[7]: https://docs.aspose.com/display/wordsnet/Saving+a+Document#SavingaDocument-SaveBlackandWhiteImagewithOneBitPerPixelFormat
[8]: https://docs.aspose.com/display/wordsnet/Working+with+Document#WorkingwithDocument-WorkingwithFootnoteandEndnote
[9]: https://docs.aspose.com/display/wordsnet/Working+with+Digital+Signatures#WorkingwithDigitalSignatures-SigningWordDocumentusingSignatureProviderIdentifier
[10]: https://docs.aspose.com/display/wordsnet/Working+with+Digital+Signatures#WorkingwithDigitalSignatures-CreateNewSignatureLineSignWordDocumentusingProviderIdentifier
[11]: https://docs.aspose.com/display/wordsnet/Applying+Formatting#ApplyingFormatting-HowtoGettheTable'sAlignment
[12]: https://docs.aspose.com/display/wordsnet/Saving+a+Document#SavingaDocument-PreventEmbeddingFontswhilesavingDocumentintoHtmlFixed
[13]: https://www.aspose.com/products/words/net
[14]: https://downloads.aspose.com/words/net
[15]: https://www.nuget.org/packages/Aspose.Words/
[16]: https://docs.aspose.com/display/wordsnet
[17]: https://apireference.aspose.com/net/words
[18]: https://forum.aspose.com/c/words
[19]: https://helpdesk.aspose.com/
[20]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[21]: https://github.com/aspose-words/Aspose.Words-for-.NET




