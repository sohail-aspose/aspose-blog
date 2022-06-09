---
title: 'Render TrueType Fonts Programmatically using C++'
seoTitle: ""
description: ""
date: Thu, 08 Oct 2020 21:36:41 +0000
draft: false
url: /2020/10/08/render-truetype-fonts-cpp/
author: Farhan Raza
summary: 'Characters are symbols that explain the meanings of different words. You can render different text characters with TrueType fonts using C++ with Aspose.Font for C++ API. It supports different text rendering features including TrueType, Type1, and other fonts. Let us explore how to use the text rendering features with a few simple API calls.'
tags: ['render truetype fonts', 'truetype fonts cpp']
categories: ['Aspose.Font Product Family']
---



{{< figure align=center src="images/Render-truetype-font-cpp.png" alt="Render truetype font c++">}}


Characters are symbols that explain the meanings of different words. You can render different text characters with [TrueType fonts][1] using C++ with [Aspose.Font for C++][2] API. It supports different text rendering features including [TrueType][3], [Type1][4], [OTF][5], [EOT][6], and other fonts. Let us explore how to use the text rendering features with a few simple API calls. We will be covering the topic under the following headings:

*   [C++ TrueType Font Rendering API – Installation][7]
*   [Implement Interface for Drawing Glyph to Render TrueType Fonts using C++][8]
*   [Render Text with TrueType Font using C++][9]

## C++ TrueType Font Rendering API – Installation {#section1}

Considering the popularity and demand of C++ platform, we have introduced very useful features in [Aspose.Font for C++][10] API. In order to render TrueType fonts in your applications, you need to configure the API by downloading it from [New Releases][11], or you can install it via [NuGet][12] using the following command:

```
_Install-Package Aspose.Font.Cpp_
```

## Implement Interface for Drawing Glyph to Render TrueType Fonts using C++ {#section2}

First of all, you need to implement [IGlyphOutlinePainter][13] under Aspose.Font.Rendering namespace. Follow the steps below for the implementation of methods and classes:

1.  Create a class named [GlyphOutlinePainter][14]
2.  Use [System.Drawing.Drawing2D.GraphicsPath][15] to draw graphics

Below is the C++ code snippet for the implementation of interface in order to draw glyphs:

{{< gist aspose-com-gists bf610decea4168f9c64482594164892b "Examples-example-source-WorkingWithTrueTypeAndOpenTypeFonts-RenderingText-2.cpp" >}}

Secondly, please create a method with name DrawText with the following steps:

1.  Loop through symbols in the text string
2.  Get GID as glyph identified for each symbol
3.  Create GlyphOutlinePainter and pass over to [GlyphOutlineRenderer][16] object
4.  Specify Glyph coordinates with [Matrix][17] object

Moreover, after following all these steps, create utility method for calculation of font dimensions to image as elaborated in the following C++ code snippet:

{{< gist aspose-com-gists bf610decea4168f9c64482594164892b "Examples-example-source-WorkingWithTrueTypeAndOpenTypeFonts-RenderingText-4.cpp" >}}

## Render Text with TrueType Font using C++ {#section3}

We have implemented the required functionality for the rendering of text with TrueType fonts. Now let us call the methods using Aspose.Font for C++ API as the code snippet below:

{{< gist aspose-com-gists bf610decea4168f9c64482594164892b "Examples-example-source-WorkingWithTrueTypeAndOpenTypeFonts-RenderingText-1.cpp" >}}

## Conclusion

In this article, you have learned how to render text using TrueType fonts with C++. Interested to learn more about features offered by Aspose.Font for C++ API? You can learn further details by exploring [API references][18] or [Product Documentation][19]. However, if you face any ambiguity or need assistance, please feel free to reach us via [Free Support Forums][20]. We look forward to engaging with you!

## See Also

[Detect Latin Symbols in TrueType and Type1 Fonts using C++][21]




[1]: https://en.wikipedia.org/wiki/TrueType
[2]: https://products.aspose.com/font/cpp
[3]: https://docs.fileformat.com/font/ttf/
[4]: https://docs.fileformat.com/font/type1/
[5]: https://docs.fileformat.com/font/otf/
[6]: https://docs.fileformat.com/font/eot/
[7]: #section1
[8]: #section2
[9]: #section3
[10]: https://products.aspose.com/font/cpp
[11]: https://releases.aspose.com/
[12]: https://www.nuget.org/packages/Aspose.Font.Cpp/
[13]: https://apireference.aspose.com/font/cpp/class/aspose.font.rendering.i_glyph_outline_painter-members
[14]: https://apireference.aspose.com/font/cpp/class/aspose.font.rendering.i_glyph_painter
[15]: https://apireference.aspose.com/drawing/net/system.drawing.drawing2d/graphicspath
[16]: https://apireference.aspose.com/font/cpp/class/aspose.font.renderers.glyph_outline_renderer
[17]: https://apireference.aspose.com/drawing/net/system.drawing.drawing2d/matrix
[18]: https://apireference.aspose.com/font/cpp
[19]: https://docs.aspose.com/font/cpp
[20]: https://forum.aspose.com/c/font
[21]: https://blog.aspose.com/2020/10/01/detect-latin-symbols-in-truetype-type1-fonts-cpp/





