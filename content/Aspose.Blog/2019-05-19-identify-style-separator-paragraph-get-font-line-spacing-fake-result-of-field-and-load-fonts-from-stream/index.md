---
title: 'Identify Style Separator Paragraph in Word Documents using C#'
date: Sun, 19 May 2019 16:15:14 +0000
draft: false
url: /2019/05/19/identify-style-separator-paragraph-get-font-line-spacing-fake-result-of-field-and-load-fonts-from-stream/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Hi guys! We are pleased to announce the new release of [Aspose.Words for .NET 19.5][1]. After reading this blog, you will be able to work with paragraph style separator, smart style behavior while joining documents, line spacing of font, get the field's result that has no field separator node, load fonts from stream, and DML text effect. Interesting, isn't it?

Let's check out these features one by one.

## Added Overload of AppendDocument Method With Additional ImportFormatOptions Parameter

We added ImportFormatOptions.SmartStyleBehavior property in [Aspose.Words 19.4][2] to specify how styles will be imported while importing one document into another. In this release, we added overload of Document.AppendDocument method that uses this property while joining documents. The additional options will affect the formatting of result document. Here is a simple code example for you.

{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Programming-Documents-Joining-Appending-AppendWithImportFormatOptions-AppendWithImportFormatOptions.cs" >}}

## Identify Style Separator Paragraph

The style separator can be added to the end of a paragraph using the Ctrl + Alt + Enter Keyboard Shortcut into MS Word. This feature allows for two different paragraph styles used in one logical printed paragraph. Starting from Aspose.Words 19.5, you will be able to identify either paragraph break is a Style Separator or not. The Paragraph.BreakIsStyleSeparator property has been added in this release. Below code example shows how to use it.

{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Programming-Documents-Document-ParagraphStyleSeparator-ParagraphStyleSeparator.cs" >}}

## How to Get Font Line Spacing

In typography, leading (line spacing of a font) refers to the distance between adjacent lines of type. It is the vertical distance between the baselines of two consecutive lines of text. Thus, the line spacing includes the blank space between lines along with the height of the character itself.

The solution to get the font line space is simple. It is Font.LineSpacing property that has been added in this release. Please check the following code example.  
  

{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Programming-Documents-Document-GetFontLineSpacing-GetFontLineSpacing.cs" >}}

## Obtain Fake Result of Field

Starting from Aspose.Words 19.5, you can get the result of field that has no field separator node. We added Field.DisplayResult property to achieve it. Note that MS Word displays it in the document by calculating the field's value on the fly. You can use this property as shown below.

{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Programming-Documents-Fields-FieldDisplayResults-FieldDisplayResults.cs" >}}

## Add feature to Load Fonts from Stream

In some cases, you need to load fonts from stream instead of disk. Now, you do not need to worry about it. We added new feature in this release to load the fonts from stream that will be used during Document import and rendering document to fixed file formats. Please refer to the following article for more detail.  
Loading Fonts from Stream

## How to Check DML Text Effect

MS Word allows user to set the text effect e.g. Glow, Fill, Shadow etc. To get this text effect, we added Font.HasDmlEffect method in this release. Below code example shows how to use it.

{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Programming-Documents-Document-CheckDMLTextEffect-CheckDMLTextEffect.cs" >}}

## Obsolete Properties and Methods Related to Font Substitution Settings were Removed from FontSettings class

You may be wondering about deleted API. Here is the detail of deleted properties and methods.

Obsolete property DefaultFontName was removed from FontSettings class. Please use SubstitutionSettings.DefaultFontSubstitution instead.

Obsolete property EnableFontSubstitution was removed from FontSettings class. Please use SubstitutionSettings.FontInfoSubstitution instead.

Obsolete methods GetFontSubstitutes, SetFontSubstitutes, AddFontSubstitutes was removed from FontSettings class. Please use SubstitutionSettings.TableSubstitution instead.  
  

There are many other features, enhancement, and bug fixes included in this release. Please check the release notes of [Aspose.Words for .NET 19.5][3].

When time allows you can check Aspose.Words' API [examples at Github][4], talk about this release and other API related issues in our [forum][5].




[1]: https://www.nuget.org/packages/Aspose.Words/19.5.0
[2]: https://blog.aspose.com/2019/05/01/flexible-control-over-importing-tasks-resolve-fonts-while-loading-html-or-svg-improved-importing-behavior-for-list-number-and-textbox/
[3]: https://docs.aspose.com/words/net/aspose-words-for-net-19-5-release-notes/
[4]: https://github.com/aspose-words/Aspose.Words-for-.NET
[5]: https://forum.aspose.com/c/words




