---
title: 'Restart List using LINQ Reporting Engine in Word Documents'
date: Sat, 13 Jul 2019 09:09:21 +0000
draft: false
url: /2019/07/13/support-of-opentype-fonts-and-kerning-feature-detect-smartart-shape-restart-list-number-using-linq-reporting-dealing-with-linked-textboxes-and-basic-reader-and-writer-for-markdown/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Hi guys! We are gratified to announce the new version of Aspose.Words for .NET i.e. 19.7. You will be happy to know that we have added interesting features in this release e.g. restart list number using LINQ Reporting, working with linked text boxes, detect SmartArt in Word document, etc. This release is available for download and to be used where .NET is installed.

*   [Download Aspose.Words for .NET 19.7][1]

Let's check out what are the new features and how they work.

## Support of OpenType Fonts and Kerning Feature

OpenType is a font format for scalable computer fonts and introduced to provide better support for languages and writing systems as compared to PostScript and TrueType. We have added TextShaperFactory property in LayoutOptions class. This property is used to get or set [ITextShaperFactory][2] implementation used for Advanced Typography rendering features.

How does this feature work? It's very simple. Please check the code example and detail in the following article.

*   [How to Use OpenType Features][3]

## Detect SmartArt Shape

Starting from this release, you can detect the SmartArt shape in the Word document. You need to simply use the [Shape.HasSmartArt][4] property. This property returns _true_ if this Shape has a SmartArt object. Sounds good?

## Restart List Numbering using LINQ Reporting

With LINQ Reporting Engine, you can build reports using an extended set of reporting features. You can create lists using LINQ Reporting. In some cases, it is needed to restart the list numbers. Now, you can achieve it using Aspose.Words. We have added this exciting feature in this release.

How does it work? It is well explained in the following article. Please read it.

*   [Restarting List Numbering Dynamically][5]

How awesome is that? I hope you have liked it.

## Dealing With Linked Textboxes

This is another amazing feature that has been added in this release. Now, you can create a link between textboxes, check linked textboxes sequence, and break the link between them. We have added IsValidLinkTarget, Next, Previous, BreakForwardLink, and Parent properties in [TextBox][6] class. For more detail, please read the following article.

*   [Working with Linked TextBoxes][7]

Keep reading…

## Work with Revision Group {#WorkingwithDocument-RevisionGroupDetails}

A new property Revision.Group has been added in this release to get the revision group. It is used to get detail if the revision belongs to any group. For more detail and code example, please read the following article.

*   [Revision Group Details][8]

## Implemented Basic Reader and Writer for Markdown Features

Markdown is a simple way to format plain text that can easily be converted to HTML. In this release we have added support of headings, blockquotes, horizontal rules, bold emphasis, and italic emphasis Markdown features. For complete detail, please read the following article.

*   [Working with Markdown Features][9]

We suggest you please check the release notes of [Aspose.Words for .NET 19.7][10] for complete detail of API changes.

When time allows you can check Aspose.Words' API [examples at Github][11], talk about this release and other API related issues in our [forum][12].




[1]: https://www.nuget.org/packages/Aspose.Words/19.7.0
[2]: https://apireference.aspose.com/net/words/aspose.words.shaping/itextshaper
[3]: https://docs.aspose.com/display/wordsnet/Enable+OpenType+Features
[4]: https://apireference.aspose.com/net/words/aspose.words.drawing/shape/properties/hassmartart
[5]: https://docs.aspose.com/display/wordsnet/Template+Syntax#TemplateSyntax-RestartingListNumberingDynamically
[6]: https://apireference.aspose.com/net/words/aspose.words.drawing/textbox
[7]: https://docs.aspose.com/display/wordsnet/Working+with+TextBoxes
[8]: https://docs.aspose.com/display/wordsnet/Track+Changes+in+a+Document#TrackChangesinaDocument-RevisionGroupDetails
[9]: https://docs.aspose.com/display/wordsnet/Working+with+Markdown+Features
[10]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+19.7+Release+Notes
[11]: https://github.com/aspose-words/Aspose.Words-for-.NET
[12]: https://forum.aspose.com/c/words




