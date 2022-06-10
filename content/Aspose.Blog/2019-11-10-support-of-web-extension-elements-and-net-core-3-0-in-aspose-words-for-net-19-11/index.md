---
title: 'Support of Web Extension and .NET Core 3.0 in Aspose.Words for .NET 19.11'
date: Sun, 10 Nov 2019 06:53:16 +0000
draft: false
url: /2019/11/10/support-of-web-extension-elements-and-net-core-3-0-in-aspose-words-for-net-19-11/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

It is our pleasure to announce the November release of [Aspose.Words for .NET][1]. We have included quite exciting features and enhancements in this release. Now, you can add Web extension elements in Word document, format the horizontal rule, and use Aspose.Words with .NET Core 3.0. let’s check out how to use newly introduced features.

## Support of Web Extension Elements

Microsoft Office allows you to add more functionality through web extension. It extends Office applications and interacts with the content in Office documents. Web Extension adds additional functionality to Office client to improve the user experience and productivity.

How to work with Web extensions using Aspose.Words? Well, it is not magic.

We have added [Aspose.Words.WebExtensions][2] namespace in this release to work with Web extensions. This namespace allows you to customize elements and attributes that extend the XML vocabulary for representing Office Add-ins. Please read the following article about working with Web extensions.

Working with Web Extensions

## Format Horizontal Rule

Adding a horizontal line in the MS Word document is sometimes called a horizontal rule. We have added new feature in this release to format the horizontal rule. In previous versions of Aspose.Words, you can add it using DocumentBuilder.InsertHorizontalRule method. However, the formatting of the horizontal rule was not supported. We have added Shape.HorizontalRuleFormat property and public class HorizontalRuleFormat in this release to format the horizontal rule. Now, you can set height, width, color, alignment, and 3D shading of it using this release of Aspose.Words. Following code example shows how to format horizontal rule.

{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Programming-Documents-Document-DocumentBuilderHorizontalRule-DocumentBuilderHorizontalRuleFormat.cs" >}}

## Improved Macros Support

Aspose.Words already provides API to read and write the VBA Project. In this release, we have improved the macros support. Now, you can set the name of VBA project, read the VBA project’s code page, read and write VBA module name, add and remove VBA module. Following code example shows how to set properties of VbaProject and VbaModule classes.

{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Loading-and-Saving-WorkingWithVbaMacros-CreateVbaProject.cs" >}}

## Aspose.Words.MailMerging.MailMergeRtlCleanupMode was removed

We have removed obsolete enum Aspose.Words.MailMerging.MailMergeRtlCleanupMode from Aspose.Words' API.

When time allows you can check Aspose.Words' [API reference guide][3], [examples at Github][4], talk about this release and other API related issues in our [forum][5].

We recommend you please check the release notes of [Aspose.Words for .NET 19.11][6] for complete detail of API changes.




[1]: https://www.nuget.org/packages/Aspose.Words/19.11.0
[2]: https://apireference.aspose.com/net/words/aspose.words.webextensions/
[3]: https://apireference.aspose.com/net/words
[4]: https://github.com/aspose-words/Aspose.Words-for-.NET
[5]: https://forum.aspose.com/c/words
[6]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+19.11+Release+Notes




