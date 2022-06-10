---
title: 'Use for Font FallBack and Prompt Text using Aspose.Slides for .NET and Java'
date: Sun, 03 Nov 2019 09:44:42 +0000
draft: false
url: /2019/11/03/support-for-font-fallback-and-prompt-text-using-aspose.slides/
author: Adnan Ahmad
summary: ''
tags: []
categories: ['Aspose.Slides Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Slides-for-net_100.png)Hello readers! I am grateful to share the release announcement for v19.10 of [Aspose.Slides][2] for .NET and Java. We have included the support for exciting new features, which include support for using Font FallBack and Prompt Text setting inside presentation files generated using Aspose.Slides.

## Support For Font FallBack

Almost for all symbols of Unicode characters, a reserve typeface is used that we can call Font Fallback. If any Unicode character is used in any application by selecting a particular font and that character is not part of the repertoire of used font, then, in this case, a symbol from Fallback font is used as a replacement for rendering. Aspose.Slides now offers the same support in API.

In the following code example, we have demonstrated the use of setting Font Fallback using **FontFallBackRule** objects.

{{< gist aspose-com-gists a56eda38c01ad33dc653116c7bae4293 "Examples-CSharp-Text-SetFontFallBack-SetFontFallBack.cs" >}}

The equivalent Java based example for this is:

{{< gist aspose-com-gists 1f55f0222bc39a382d831900e8de7400 "Examples-src-main-java-com-aspose-slides-examples-Text-FallBackRulesCollection-FallBackRulesCollection.java" >}}

## Set Prompt Text in a Placeholder {#AddingandFormattingText-SetPromptTextinaPlaceholder}

When working with PowerPoint placeholders for text, the text field highlights what is to be entered in that. This phenomenon is called support for **Prompt Text** for a placeholder in PowerPoint. Prompt Text is only information string and vanishes as soon as you start writing your custom text to the placeholder. For example, you can observe Prompt Text fields like **Click to add a title** or **Click to add subtitle** when working with PowerPoint slides. Using Aspose.Slides you can now add custom Prompt Text manually by accessing the default placeholders.

In the following example, we have demonstrated the use of this new feature:

{{< gist aspose-com-gists a56eda38c01ad33dc653116c7bae4293 "Examples-CSharp-Text-AddCustomPromptText-AddCustomPromptText.cs" >}}

The Java-based implemented for this is as under:

{{< gist aspose-com-gists 1f55f0222bc39a382d831900e8de7400 "Examples-src-main-java-com-aspose-slides-examples-Text-AddCustomPromptText-AddCustomPromptText.java" >}}

Moreover, there are many other new features, enhancement, and bug fixes included in this [release][3].

You may also check out API [examples at Github][4]. You may talk about this release and other API related issues in our [forum][5].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Slides-for-net_100.png "Aspose.Slides or .NET logo"
[2]: https://products.aspose.com/slides
[3]: https://docs.aspose.com/display/slidesnet/Aspose.Slides+for+.NET+19.10+Release+Notes
[4]: https://github.com/aspose-slides/
[5]: https://forum.aspose.com/c/slides




