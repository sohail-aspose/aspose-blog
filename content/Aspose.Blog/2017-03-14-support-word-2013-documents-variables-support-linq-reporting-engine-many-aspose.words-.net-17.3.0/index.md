---
title: 'Work with Word 2013 Documents and Use Variables in LINQ Reporting Engine with Aspose.Words for .NET 17.3.0'
date: Tue, 14 Mar 2017 06:19:29 +0000
draft: false
url: /2017/03/14/support-word-2013-documents-variables-support-linq-reporting-engine-many-aspose.words-.net-17.3.0/
author: Tahir Manzoor
summary: ''
tags: ['Remove Empty Table Rows in Word', 'Work with Word 2013 Docs']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose-Words-for-net-e1378287014402.png" alt="Aspose.Words for .NET logo">}}


We are pleased to announce our next version of [Aspose.Words 17.3.0][1]. This month’s release contains over 67 useful new features, enhancements and bug fixes. Please see the [release notes][2] for more detail. If you are planning to upgrade from an older version of Aspose.Words to the current version, we would strongly suggest you to check the [Public API and Backward Incompatible Changes][3] section to know what APIs are changed so far.

Here is a look at just a few of the biggest features and API changes in this month’s release.

*   Full support for Word 2013 documents (roundtrip to/from DOCX)
*   Variables support and more new features are introduced in LINQ Reporting Engine.
*   New Public OfficeMath properties: MathObjectType, Justification, DisplayType
*   The font substitution mechanism improved. Now Aspose.Words evaluate all related fields in FontInfo (Panose, Sig, etc) and finds the closest match among the available font sources.
*   Asian font rendering improved (more precise metrics calculation).
*   Stroke weight is now taken into account while rendering auto-sized Textboxes.
*   Implemented the next round of improvements in the table grid algorithm.
*   Improved table breaking logic in compatibility mode for tables with header rows.
*   Improved table breaking logic for tables with nested tables in a cell with the bottom margin set.
*   Improved tables breaking logic for tables with vertically merged cells having horizontal borders.
*   Implemented fitText option for table cells.

## Full Support for Word 2013 Documents

Starting from Aspose.Words 17.3.0, we have added the full support of MS Word 2013 documents. The full support of roundtrip to/from DOCX is available in this Aspose.Words version.

## Font Substitution Mechanism Improved

Previously, Aspose.Words performed font substitution only in cases when FontInfo in the document for the missing font doesn't contain the [PANOSE][4]. Now Aspose.Words evaluates all related fields in FontInfo (Panose, Sig etc) and finds the closest match among the available font sources. In case of font substitution the warning is issued with text:

"Font '' has not been found. Using '' font instead. Reason: closest match according to font info from the document."

Please note that now the font substitution mechanism will override the FontSettings.DefaultFontName in cases when FontInfo for the missing font is available in the document. FontSettings.DefaultFontName will be used only in cases when there are no FontInfo for the missing font.

Moreover, please note that the font substitution algorithm in MS Word is not documented So, the result of Aspose.Words font substitution may not match MS Word choice.

## Added a MailMergeCleanupOptions Option to Remove Empty Row

We have introduced MailMergeCleanupOptions.RemoveEmptyTableRows option in Aspose.Words 17.3.0 to remove empty rows that contain mail merge regions from the document. Please refer to the following article:  
[How to Remove Empty Rows with Cleanup Option][5]

{{< gist aspose-words 9a306a41bb6aea8adfcabf5a575c5718 "Examples-CSharp-Mail-Merge-RemoveRowsFromTable-RemoveRowsFromTable.cs" >}}

## Added Public Property OfficeMath.MathObjectType

We have introduced new property OfficeMath.MathObjectType in Aspose.Words 17.3.0. This property allows users to get type MathObjectType of this Office Math object. The MathObjectType enumeration is added in Aspose.Words 17.3.0 to specify the type of an Office Math object.

```
OfficeMath officeMath = GetOfficeMath();
if (officeMath.MathObjectType == MathObjectType.Matrix)
{
   // Do something useful with the Matrix object.
}
```

## Added Public Properties OfficeMath.Justification and OfficeMath.DisplayType

We have added new public properties Justification and DisplayType into the OfficeMath class. Please refer to the following article for more detail:  
[Working with OfficeMath][6]

{{< gist aspose-words 9a306a41bb6aea8adfcabf5a575c5718 "Examples-CSharp-Programming-Documents-Fields-UseOfficeMathProperties-SpecifylocaleAtFieldlevel.cs" >}}

Note that Aspose.Words mimics MS Word behavior. Following is the detail:

*   DisplayType cannot be changed for nested Office Math. The exception will be thrown.
*   Inline justification cannot be set to the Office Math displayed on its own line (DisplayType=OfficeMathDisplayType.Display). The exception will be thrown. OfficeMath.DisplayType property has to be used to change OfficeMathDisplayType first.
*   Justification cannot be set to the Office Math displayed inline with text. The exception will be thrown. OfficeMath.DisplayType property has to be used to change OfficeMathDisplayType first.

## Provided Ability to Specify Locale at Field Level

We have added a new public property Field.LocaleId in Aspose.Words 17.3.0 allows users to get/set field's locale. Please refer to the following article:

*   [Inserting Locale at Field Level][7]

```
/// <summary>
/// Gets or sets LCID of the field.
/// </summary>
/// <seealso cref="FieldUpdateCultureSource.FieldCode"/>
public int LocaleId
```

## Support of Variables, Dynamic Text Background Setting, and Image Size Fit Mode in LINQ Reporting Engine

We have added a new parameter -fitSizeLim for image tag to change the size of the textbox according to the size of the image without increasing the size of the textbox. Please read the detail here:

*   [Inserting Images Dynamically][8]

We have added the support of variables in Aspose.Words 17.3.0. LINQ Reporting Engine enables you to use variables in template documents. Variables are useful when you need to calculate an expensive value just once and access it multiple times in a template. Please read the detail from here:

*   [Using Variables][9]
*   [In-Table List Template with Running (Progressive) Total][10]Total)

We have added support of setting text background color dynamically in Aspose.Words 17.3.0. Please read the detail here:

*   [Setting Text Background Color Dynamically][11]

## Aspose.Words for .NET Resources

The following resources will help you work with Aspose.Words for .NET:

*   [Home of Aspose.Words for .NET API][12].
*   [Aspose.Words for .NET Download Section][13].
*   [Aspose.Words for .NET Documentation][14] – up-to-date documentation containing Programmer’s Guide, Knowledge Base and much more.
*   [Aspose.Words for .NET API Reference Guide][15] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Words Product Family Forum][16] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Words APIs.
*   [Enable Blog Subscription][17] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
*   [Aspose.Words for .NET Examples][18] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: http://downloads.aspose.com/words/net
[2]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+17.3.0+Release+Notes
[3]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+17.3.0+Release+Notes
[4]: https://en.wikipedia.org/wiki/PANOSE
[5]: https://docs.aspose.com/display/wordsnet/How+to+Remove+Unmerged+Fields%2C+Empty+Paragraphs+and+Unmerged+Regions#HowtoRemoveUnmergedFields,EmptyParagraphsandUnmergedRegions-HowtoRemoveEmptyRowswithCleanupOption
[6]: https://docs.aspose.com/display/wordsnet/Working+with+OfficeMath
[7]: https://docs.aspose.com/display/wordsnet/Use+DocumentBuilder+to+Insert+Document+Elements#UseDocumentBuildertoInsertDocumentElements-InsertingLocaleatFieldLevel
[8]: https://docs.aspose.com/display/wordsnet/Template+Syntax#TemplateSyntax-InsertingImagesDynamically
[9]: https://docs.aspose.com/display/wordsnet/Template+Syntax#TemplateSyntax-UsingVariables
[10]: https://docs.aspose.com/display/wordsnet/Typical+Templates#TypicalTemplates-In-TableListTemplatewithRunning(Progressive
[11]: https://docs.aspose.com/display/wordsnet/Template+Syntax#TemplateSyntax-SettingTextBackgroundColorDynamically
[12]: https://products.aspose.com/words/net
[13]: http://downloads.aspose.com/words/net
[14]: https://docs.aspose.com/display/wordsnet
[15]: https://apireference.aspose.com/net/words
[16]: http://forum.aspose.com
[17]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[18]: https://github.com/aspose-words/Aspose.Words-for-.NET




