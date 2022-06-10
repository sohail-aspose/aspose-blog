---
title: 'Insert Hyperlinks and Shapes Dynamically in Word Documents using C#'
date: Thu, 14 Jun 2018 09:46:59 +0000
draft: false
url: /2018/06/14/insert-hyperlinks-and-shapes-dynamically-in-word-documents-using-csharp-asp.net/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose-Words-for-net.png" alt="Aspose.Words for .NET logo">}}


We are pleased to announce our next version [Aspose.Words for .NET 18.6][1]. This month’s release contains over 62 useful new features, enhancements, and bug fixes. Please see the [release notes][2] for more detail. If you are planning to upgrade from an older version of Aspose.Words to the current version, we would strongly suggest you to check the [Public API and Backward Incompatible Changes][3] section to know what APIs are changed so far.

Here is a look at just a few of the biggest features and API changes in this month’s release.

*   Exposed Title and Description properties into Table class
*   Added feature to insert shapes through the DocumentBuilder using ShapeType
*   Changed public properties of AxisScaling class
*   Implemented API allowing to set up language preferences
*   Added IsMoveFromRevision and IsMoveToRevision properties
*   Exposed properties for Asian typography into ParagraphFormat class
*   Public TXT save option AddBidiMarks is added
*   Implemented "left" and "right" alignment support for Ruby objects rendering
*   Improved rendering of DrawingML chart data labels with percentage values and the specified format
*   Flat shapes that are perpendicular to the projection plane are not rendered now
*   Zero-width characters in DrawingML textboxes no longer cause an exception during rendering
*   Fixed an issue with font fallback rendering for 1F600 - 1F64F (Emoticons) Unicode range
*   Fixed a bug with the rendering of the chart data labels, when label text and SpPr are specified
*   Fixed a bug with the maximum value of the chart axis when rendering DrawingML charts
*   Fixed a problem with rendering of subscript and superscript text in DrawingML charts
*   Fixed a bug where the shadowed shapes with compound outline lost their fill
*   Fixed MathML alignment issue inside text boxes
*   Fixed layout when large inline shape is attached to a paragraph with space after overflowing page
*   Fixed issue with preferred width of vertically merged table cells accounted for during width computation
*   Fixed exception when revision balloons are displayed in certain cases
*   Enhanced logic which handles page breaks inside text frames
*   LINQ Reporting Engine supports dynamic insertion of hyperlinks

## Insert Hyperlink Dynamically in Word Documents

A new feature has been introduced in this version of Aspose.Words to insert hyperlink dynamically using LINQ Reporting engine. Please read the following article for more detail.

*   [Inserting Hyperlinks Dynamically][4]

## Insert Shapes in Word Documents

We have added the following methods in the DocumentBuilder class to insert inline and free-floating shapes. These methods allow inserting DML shape into the document model. For more detail, please read the following article.

*   [Inserting Inline and Free-floating Shapes][5]

```
 /// <summary>
/// Inserts inline shape with specified type and size.
/// </summary>
/// <param name="shapeType">The shape type to insert into the document.</param>
/// <param name="width">The width of the shape in points.</param>
/// <param name="height">The height of the shape in points.</param>
/// <returns>The shape node that was inserted.</returns>
public Shape InsertShape(ShapeType shapeType, double width, double height)

/// <summary>
/// Inserts free-floating shape with specified position, size and text wrap type.
/// </summary>
/// <param name="shapeType">The shape type to insert into the document</param>
/// <param name="horzPos">Specifies where the horizontal distance to the shape is measured from.</param>
/// <param name="left">Distance in points from the origin to the left side of the shape.</param>
/// <param name="vertPos">Specifies where the vertical distance to the shape is measured from.</param>
/// <param name="top">Distance in points from the origin to the top side of the shape.</param>
/// <param name="width">The width of the shape in points.</param>
/// <param name="height">The width of the shape in points.</param>
/// <param name="wrapType">Specifies how to wrap text around the shape.</param>
/// <returns>The shape node that was inserted.</returns>
public Shape InsertShape(ShapeType shapeType, RelativeHorizontalPosition horzPos, double left, RelativeVerticalPosition vertPos, double top, double width, double height, WrapType wrapType)
```

## Added Title and Description Properties into Table Class

Starting from Aspose.Words 18.6, you can set the alternative text of table. We have added Title and Description properties into Table class. Please refer to the following article for more detail.

*   [Working with Alternative Text of Table][6]

```
/// <summary>
/// Gets or sets title of this table. It provides an alternative text representation of the information contained in the table.
/// </summary>
/// <remarks>
/// The default value is an empty string.
/// This property is meaningful for ISO/IEC 29500 compliant DOCX documents (see the OoxmlCompliance class).
/// When saved to pre-ISO/IEC 29500 formats, the property is ignored.
/// </remarks>
public string Title
{
    get; set;
}
 
/// <summary>
/// Gets or sets description of this table. It provides an alternative text representation of the information contained in the table.
/// </summary>
/// <remarks>
/// The default value is an empty string.
/// This property is meaningful for ISO/IEC 29500 compliant DOCX documents (see the OoxmlCompliance class).
/// When saved to pre-ISO/IEC 29500 formats, the property is ignored.
/// </remarks>
public string Description
{
    get; set;
}
```

## Changed Public Properties of AxisScaling Class

We have removed MinimumIsAuto and MaximumIsAuto properties from the AxisScaling class. The type of the Minimum and Maximum properties has been changed from double to AxisBound. A new class AxisBound has been added in the latest API that allows specifying axis bound as a numeric, datetime or "auto" value. Please check the code examples from the following article

*   [How to Set Chart Axis Properties][7]

```
/// <summary>
/// Gets or sets minimum value of the axis.
/// </summary>
/// <remarks>
/// The default value is "auto".
/// </remarks>
public AxisBound Minimum
{
    get; set;
}
 
/// <summary>
/// Gets or sets the maximum value of the axis.
/// </summary>
/// <remarks>
/// The default value is "auto".
/// </remarks>
public AxisBound Maximum
{
    get; set;
} 
```
```
namespace Aspose.Words.Drawing.Charts
{
    /// Represents minimum or maximum bound of axis values.
    /// Bound can be specified as a numeric, datetime or a special "auto" value.
    /// The instances of this class are immutable.
    public class AxisBound
    {
        /// Creates a new instance indicating that axis bound should be determined         /// automatically by a word-processing application.
        public AxisBound();
        /// Creates an axis bound represented as a number.
        public AxisBound(double value);
        /// Creates an axis bound represented as datetime value.
        public AxisBound(DateTime datetime);
 
        /// Returns a flag indicating that axis bound should be determined automatically.
        public bool IsAuto
        {
            get;
        }
 
        /// Returns numeric value of axis bound.
        public double Value
        {
            get;
        }
 
        /// Returns value of axis bound represented as datetime.
        public DateTime ValueAsDate
        {
            get;
        }
    }
}
```

## Setup Language Preferences

We have added a new feature in this release to [setup language preferences][8]. In MS Word, you can setup it from 'Set the Office Language Preferences' dialog. Please read the following article for more detail.

*   [Allowing to Setup Language Preferences][9]

The LanguagePreferences class has been added for this feature.

```
/// <summary>
/// Allows to set up language preferences.
/// </summary>
/// <remarks>
/// Implements 'Set the Office Language Preferences' dialog in Word.
/// </remarks>
public class LanguagePreferences
```

This class implements the following public members:

```
/// <summary>
/// Adds additional editing language.
/// </summary>
public void AddEditingLanguage(EditingLanguage language)
 
/// <summary>
/// Adds additional editing languages.
/// </summary>
public void AddEditingLanguages(EditingLanguage[] languages)
 
/// <summary>
/// Sets default editing language.
/// </summary>
public void SetAsDefault(EditingLanguage language)

/// <summary>
/// <para>Gets or sets default editing language.</para>
/// <para>The default value is <see cref="EditingLanguage.EnglishUS"/>.</para>
/// </summary>
public EditingLanguage DefaultEditingLanguage 
```

Also added a new public enumeration:

```
/// <summary>
/// Specifies the editing language.
/// </summary>
public enum EditingLanguage
```

And finally, a new public property is added to LoadOptions class:

```
/// <summary>
/// Gets language preferences that will be used when document is loading.
/// </summary>
public LanguagePreferences LanguagePreferences
```

## Support of Move From and Move To Revisions

We have added following public properties into the Inline, Paragraph, ShapeBase and InlineStory classes to work with 'move from' and 'move to ' revisions. For more detail, please read the following article.

*   [Programmatically Access Revisions][10]

```
/// <summary>
/// Returns true if this object was moved (deleted) in Microsoft Word while change tracking was enabled.
/// </summary>
public bool IsMoveFromRevision
{
    get;
}
 
/// <summary>
/// Returns true if this object was moved (inserted) in Microsoft Word while change tracking was enabled.
/// </summary>
public bool IsMoveToRevision
{
    get;
}
```

## Support of Line Break Options for Asian Typography

In this release, we have added support of line break options for Asian Typography. The following public properties have been added into the ParagraphFormat class. Please read the following article for more detail.

*   [Set Line Break Options][11]

```
/// <summary>
/// Gets or sets a flag indicating whether East Asian line-breaking rules are applied to the current paragraph.
/// </summary>
public bool FarEastLineBreakControl
{
    get; set;
}
 
/// <summary>
/// If this property is <b>false</b>, Latin text in the middle of a word can be wrapped for
/// the current paragraph. Otherwise Latin text is wrapped by whole words.
/// </summary>
public bool WordWrap
{
    get; set;
}
 
/// <summary>
/// Gets or sets a flag indicating whether hanging punctuation is enabled for the current paragraph.
/// </summary>
public bool HangingPunctuation
{
    get; set;
} 
```

## Support of "Add bi-directional marks" for TXT Format

We have added TxtSaveOptions.AddBidiMarks property in this version of Aspose.Words to support the insertion of bi-directional marks in output TXT file format. Please read the following article for more detail.

*   [How to Add Bi-Directional Marks][12]

```
/// <summary>
/// <para>Specifies whether to add bi-directional marks before each BiDi run when exporting in plain text format.</para>
/// <para>The default value is <b>true</b>.</para>
/// </summary>
public bool AddBidiMarks
```

## Obsolete Enum RowAlignment was Removed

Obsolete enum RowAlignment was Removed from API. Please use TableAlignment enum instead.

## Obsolete Method InvalidateFieldTypes was Removed from Document and Range Classes

Obsolete method InvalidateFieldTypes was removed from Document and Range classes. Please use NormalizeFieldTypes method instead.

## Obsolete Properties were Removed from RowFormat Class

Obsolete property RowFormat.PreferredWidth was removed. Please use the Table.PreferredWidth property instead.

Obsolete property RowFormat.RowAlignment was removed. Please use the Table.RowAlignment property instead.

Obsolete property RowFormat.AllowAutoFit was removed. Please use the Table.AllowAutoFit property instead.

Obsolete property RowFormat.Bidi was removed. Please use the Table.Bidi property instead.

Obsolete properties RowFormat.LeftPadding/RightPadding/TopPadding/BottomPadding was removed. Please use these properties from Table class instead.

Obsolete property RowFormat.CellSpacing was removed. Please use the Table.CellSpacing property instead.

Obsolete property RowFormat.LeftIndent was removed. Please use the Table.LeftIndent property instead.

Obsolete method RowFormat.ClearCellPadding() was removed. Please use padding properties on the Table instead.

## Aspose.Words for .NET Resources

The following resources will help you work with Aspose.Words for .NET:

1.  [Home page of .NET API][13].
2.  [Install using NuGet Package][14]
3.  [Documentation][15] – up-to-date documentation containing Programmer’s Guide, Knowledge Base and much more.
4.  [API Reference Guide][16] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
5.  Aspose.Words Product Family Forum – post your technical questions and queries, or any other problem you are facing while working with Aspose.Words APIs.
    *   [Free Support Forum][17]
    *   [Paid Support Forum][18]
6.  [Enable Blog Subscription][19] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
7.  [Examples][20] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Words/
[2]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+18.6+Release+Notes
[3]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET
[4]: https://docs.aspose.com/display/wordsnet/Template+Syntax#TemplateSyntax-InsertingHyperlinksDynamically
[5]: https://docs.aspose.com/display/wordsnet/Use+DocumentBuilder+to+Insert+Document+Elements#UseDocumentBuildertoInsertDocumentElements-InsertingInlineandFree-floatingShapes
[6]: https://docs.aspose.com/display/wordsnet/Applying+Formatting#ApplyingFormatting-WorkingwithAlternativeTextofTable
[7]: https://docs.aspose.com/display/wordsnet/Working+with+Charts#WorkingwithCharts-HowtoSetChartAxisProperties
[8]: https://support.office.com/en-us/article/add-an-editing-language-or-set-language-preferences-in-office-663d9d94-ca99-4a0d-973e-7c4a6b8a827d?ui=en-US&rs=en-US&ad=US
[9]: https://docs.aspose.com/display/wordsnet/Working+with+Document#WorkingwithDocument-AllowingtoSetupLanguagePreferences
[10]: https://docs.aspose.com/display/wordsnet/Working+with+Document#WorkingwithDocument-ProgrammaticallyAccessRevisions
[11]: https://docs.aspose.com/display/wordsnet/Using+DocumentBuilder+to+Modify+a+Document+Easily#UsingDocumentBuildertoModifyaDocumentEasily-SetLineBreakOptions
[12]: https://docs.aspose.com/display/wordsnet/Working+with+Text+Document#WorkingwithTextDocument-HowtoAddBi-DirectionalMarks
[13]: https://products.aspose.com/words/net
[14]: https://www.nuget.org/packages/Aspose.Words/
[15]: https://docs.aspose.com/display/wordsnet
[16]: https://apireference.aspose.com/net/words
[17]: https://forum.aspose.com/c/words
[18]: https://helpdesk.aspose.com/
[19]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[20]: https://github.com/aspose-words/Aspose.Words-for-.NET




