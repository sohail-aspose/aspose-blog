---
title: 'Set Prompt Text in PowerPoint Presentations using C++'
date: Sun, 10 Nov 2019 04:46:58 +0000
draft: false
url: /2019/11/10/support-for-font-fallback-and-prompt-text-using-aspose.slides-for-c/
author: Adnan Ahmad
summary: ''
tags: []
categories: ['Aspose.Slides Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Slides-for-net_100.png)Hello readers! I am grateful to share the release announcement for v19.10 of [Aspose.Slides for C++][2]. We have included the support for exciting new features, which include support for using Font FallBack and Prompt Text setting inside presentation files generated using Aspose.Slides.

## Set Prompt Text in a Placeholder in PowerPoint PPT {#AddingandFormattingText-SetPromptTextinaPlaceholder}

A **Prompt** Text is a content that shows up in a content field when it is the first load however that disappears when a client begins composing into the content field. This is essential for client straightforwardness to become more acquainted with what is to be entered in the chose to field. We know that Standard and pre-built layouts contain placeholders with default text like **Click to add a title** or **Click to add subtitle**. Now using Aspose.Slides you can now add custom Prompt Text manually by accessing the default placeholders.

The following code snippet below shows how to use this feature:

{{< gist aspose-com-gists 81aeb05e6d3a070aa76fdea22ed53bc7 "Examples-SlidesCPP-AddCustomPromptText-AddCustomPromptText.cpp" >}}

For more information about this feature, please visit the documentation article, [Setting Prompt Text in a Placeholder][3].

## Font FallBack in PowerPoint Presentations using C++

A Font Fallback is a reserve type containing symbols for as several Unicode characters as doable. When a display system encounters a character that's not a part of any available fonts, an alternative character from a Fallback font is used instead. Normally, a fallback font style will contain images illustrative of the different sorts of Unicode characters. For this purpose, a new method [IFontFallBackRule][4] has been added in Aspose.Slides for C++.

The following code example shows how to set font fallback using **FontFallBackRule** objects.

{{< gist aspose-com-gists 81aeb05e6d3a070aa76fdea22ed53bc7 "Examples-SlidesCPP-SetFontFallBack-SetFontFallBack.cpp" >}}

For more information about this feature, please visit the documentation article, [Setting Font FallBack][5].

Wait, there are many other features, enhancement, and bug fixes included in this [release][6].

When time allows you can check out API [examples at Github][7], talk about this release and other API related issues in our [forum][8].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Slides-for-net_100.png "Aspose.Slides or .NET logo"
[2]: https://products.aspose.com/slides/cpp
[3]: https://docs.aspose.com/display/slidescpp/Managing+Fonts#ManagingFonts-SetFontFallBack
[4]: https://apireference.aspose.com/net/slides/aspose.slides/ifontfallbackrule
[5]: https://docs.aspose.com/display/slidescpp/Managing+Fonts#ManagingFonts-SetFontFallBack
[6]: https://docs.aspose.com/display/slidescpp/Aspose.Slides+for+CPP+19.10+Release+Notes
[7]: https://github.com/aspose-slides/
[8]: https://forum.aspose.com/c/slides




