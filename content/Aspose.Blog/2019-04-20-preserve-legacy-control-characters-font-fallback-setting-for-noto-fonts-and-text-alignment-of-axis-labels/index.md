---
title: 'Preserve Legacy Control Characters while Exporting Word Documents using C#'
date: Sat, 20 Apr 2019 09:42:08 +0000
draft: false
url: /2019/04/20/preserve-legacy-control-characters-font-fallback-setting-for-noto-fonts-and-text-alignment-of-axis-labels/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Hi guys! Do you want to preserve legacy control characters in Word documents? Many of you must want to work with font fallback for Google Noto fonts? You will love to export the list labels of Word document into TXT file format with specific character and change the text alignment of axis tick labels of chart. So what's the solution?

It is [Aspose.Words for .NET 19.3][1]. You can work with these features using it.

So how to work these features? Let’s talk about these one by one.

## Preserve Legacy Control Characters while Exporting Document to OOXML

Some document formats support legacy control characters. MS Word does not save these symbols to DOCX format (more accurately in OOXML formats). However, we added new property KeepLegacyControlChars in OoxmlSaveOptions class to preserve such control characters. So far only one legacy character (ShortDateTime) is supported which declared in the "DOC" format.

Here's how you can use this property:

{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Loading-and-Saving-WorkingWithOoxml-KeepLegacyControlChars.cs" >}}

## Predefined Font Fallback Settings for Google Noto Fonts

You may know about [Noto][2]. It is a font family comprising over a hundred individual fonts. We have added predefined font fallback settings for Google Noto fonts. These are free fonts licensed under SIL OFL.

Let me clarify two things here:

*   The predefined settings uses only Sans style Noto fonts with regular weight.
*   Aspose.Words does not support advanced typography. So, the Noto fonts that use advanced typography may be rendered inaccurately

The following code example shows how to use predefined font fallback settings.

{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Rendering-Printing-SetFontSettings-SetPredefinedFontFallbackSettings.cs" >}}

Don’t stop reading now! There are more Aspose.Words' features for you. Amazing, isn’t it?

## Text Alignment of Axis Tick Labels

By default, MS Word aligns Chart Label to the center. However, you can change it using ChartAxis.TickLabelAlignment property. We have simple example for you here:

{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Programming-Documents-Charts-WorkingWithChartAxis-TickMultiLineLabelAlignment.cs" >}}

Sound good? Yes, it is!

## Indentation of List Levels When Exporting Word Document to Plain Text Format

Starting from Aspose.Words 19.3, you can get the ListIndentation object and specify how many and which character to use for indentation of list levels. By default, no indentation is exported to text file format.

Here's how to work with list indentation.

### Using Tab Character{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Loading-and-Saving-WorkingwithTxt-UseTabCharacterPerLevelForListIndentation.cs" >}}

### Using Space Character{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Loading-and-Saving-WorkingwithTxt-UseSpaceCharacterPerLevelForListIndentation.cs" >}}

### Using Default Indentation{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Loading-and-Saving-WorkingwithTxt-DefaultLevelForListIndentation.cs" >}}

Wait, there are many other features, enhancement, and bug fixes included in this release. [Here you can get the detail!][3]

When time allows you can check out API [examples at Github][4], talk about this release and other API related issues in our [forum][5].




[1]: https://www.nuget.org/packages/Aspose.Words/19.3.0
[2]: https://www.google.com/get/noto/
[3]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+19.3+Release+Notes
[4]: https://github.com/aspose-words/Aspose.Words-for-.NET
[5]: https://forum.aspose.com/c/words




