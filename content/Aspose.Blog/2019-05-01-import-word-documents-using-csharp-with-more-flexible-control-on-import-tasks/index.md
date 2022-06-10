---
title: 'Import Word Documents with More Flexible Control using Aspose.Words for .NET'
date: Wed, 01 May 2019 16:01:24 +0000
draft: false
url: /2019/05/01/import-word-documents-using-csharp-with-more-flexible-control-on-import-tasks/
author: Tahir Manzoor
summary: ''
tags: ['Import of Word documents using csharp']
categories: ['Aspose.Words Product Family']
---

Hi guys! Whenever you want to do document processing tasks, the name of Aspose comes to everyone's mind. As you know we add new features and enhancement in every release of Aspose.Words. You will be happy to know that we released a new version of [Aspose.Words for .NET 19.4][1]. Let me walk you through the new features and API changes in this release.

## Added More Flexible Control Over Document Import

We added ImportFormatOptions class with public property SmartStyleBehavior in Aspose.Words 19.4. This property is used to specify how styles will be imported when they have equal names in source and destination documents. You can enable or disable this feature while importing one document into another.

What will happen when this option is enabled or disabled?

If KeepSourceFormatting importing mode is used and this option is **enabled**, the source style will be expanded into direct attributes inside a destination document. When this option is **disabled**, a source style will be expanded only if it is numbered. Existing destination attributes will not be overridden, including lists.

Note that at the moment, this option can be used only with a new public method [DocumentBuilder.InsertDocument][2].

The usage of this property is very simple. Here it is:

{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Programming-Documents-Document-WorkingWithImportFormatOptions-SmartStyleBehavior.cs" >}}

## Resolve Fonts While Loading HTML or SVG

In old versions of Aspose.Words, font families were resolved against fonts installed in the local system while loading HTML or SVG. So, if a font family could not be resolved to an installed font, it was stored in the Aspose.Words' model as is. As a result, FontSettings specified by users have not affected the resolved font names depending on the local system.

Let me make it easy for your understanding with an example.

Please check the following HTML. If ‘UnknownFont1’ is not installed on the system, the following font-family declaration resolved to "Arial" ("Arial" is the font name we use for "san-serif" generic font name.)

```
<p style='font-family:UnknownFont1, sans-serif;'>This is a paragraph.
```

  
Starting from Aspose.Words 19.4, FontSettings are taken into account while importing HTML and SVG documents and you can set up FontSettings before loading a document (add substitution rule, specify fonts folder, etc.) in order to change fonts available for font resolution.

Here is a sample code example that shows how to add a font substitution rule while loading a document.

{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Rendering-Printing-WorkingWithFontResolution-FontSettingsWithLoadOptions.cs" >}}

## Set Vertically Aligned Text Within Text Box

If you want to set the text alignment of textbox vertically, the solution is simple. You can use [TextBox.VerticalAnchor][3] property. We added this property in Aspose.Words 19.4.

The following code example shows how to use this property.

{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Programming-Documents-Shapes-WorkingWithShapes-SpecifyVerticalAnchor.cs" >}}

Please note that saving warnings will be thrown for unsupported formats (WordML) and for incompatible Word versions above 2007 (DOC, DOT).

## Write Additional Text Positioning Operators

We have added PdfSaveOptions.AdditionalTextPositioning property in this version of Aspose.Words to overcome the issue with text position with some printers. Please read the following article for more detail.

*   [Additional Text Positioning][4]

## Improved Importing Behavior for List Numbers

When you import one document into another, there can be a situation where source and destination documents have the same list identifiers. In such cases, MS Word uses formatting from the destination lists. We have added new property ImportFormatOptions.KeepSourceNumbering in Aspose.Words for .NET 19.4 to control this behavior. Please read the following article for more detail.

*   [Set Keep Source Numbering][5]

Moreover, we added a new public method that accepts the new KeepSourceNumbering option.

```
/// <summary>
/// Initializes a new instance of the <see cref="NodeImporter"/> class.
/// </summary>
/// <param name="srcDoc">The source document.</param>
/// <param name="dstDoc">The destination document that will be the owner of imported nodes.</param>
/// <param name="importFormatMode">Specifies how to merge style formatting that clashes.</param>
/// <param name="importFormatOptions">Specifies various options to format imported node.</param>
public NodeImporter(DocumentBase srcDoc, DocumentBase dstDoc, ImportFormatMode importFormatMode, ImportFormatOptions importFormatOptions)
```

## Improved Importing Behavior for TextBox

When you import a text box between different documents, the formatting of the destination document is applied to it. This corresponds to the behavior of MS Word. To allow users to choose an appropriate behavior, we have added ImportFormatOptions.IgnoreTextBoxes property in this release. For more detail, please read the following article.

*   [Ignore TextBoxes while Importing Document][6]

There are many other features, enhancement, and bug fixes included in this release. Please check the release notes of [Aspose.Words for .NET 19.4][7].

When time allows you can check Aspose.Words' API [examples at Github][8], talk about this release and other API related issues in our [forum][9].




[1]: https://www.nuget.org/packages/Aspose.Words/19.4.0
[2]: https://apireference.aspose.com/net/words/aspose.words.documentbuilder/insertdocument/methods/1
[3]: https://apireference.aspose.com/net/words/aspose.words.drawing/textbox/properties/verticalanchor
[4]: https://docs.aspose.com/display/wordsnet/Rendering#Rendering-AdditionalTextPositioning
[5]: https://docs.aspose.com/display/wordsnet/Working+with+Document#WorkingwithDocument-SetKeepSourceNumbering
[6]: https://docs.aspose.com/display/wordsnet/Working+with+Document#WorkingwithDocument-SetIgnoreTextBoxes
[7]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+19.4+Release+Notes
[8]: https://github.com/aspose-words/Aspose.Words-for-.NET
[9]: https://forum.aspose.com/c/words




