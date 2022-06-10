---
title: 'Render Text with TrueType and Type1 Fonts using C#'
seoTitle: "Render Text with TrueType and Type1 Fonts in C# | .NET Font Rendering"
description: "Use .NET Font Rendering API to render the text using TrueType TTF or Type1 fonts glyphs using C# or VB.NET within your .NET applications."
date: Wed, 16 Sep 2020 16:53:58 +0000
draft: false
url: /2020/09/16/render-text-with-truetype-type1-font-using-csharp/
author: Usman Aziz
summary: 'In the previous post, you have seen how to use Aspose.Font for .NET API for loading and saving CFF, TrueType, and Type1 fonts programmatically. In this article, you will learn how to render text using the TrueType, and Type1 font glyphs using C#. The code samples will show you how to how to generate a JPG image having text rendered on it.'
tags: ['render text using font glyphs using csharp', 'render text using truetype font in csharp', 'render text using type1 font using csharp']
categories: ['Aspose.Font Product Family']
---



{{< figure align=center src="images/aspose_font-for-net.png" alt="render text using fonts">}}


In the [previous post][1], you have seen how to use [Aspose.Font for .NET][2] API for loading and saving [CFF][3], [TrueType][4], and [Type1][5] fonts programmatically. In this article, you will learn how to render text with TrueType and Type1 font using C#. The code samples will show you how to generate a [JPG][6] image based on the provided text.

*   [.NET Font Rendering API - Installation][7]
*   [Implement Text Rendering Interface][8]
*   [Render Text with TrueType Font using C#][9]
*   [Render Text with Type1 Font using C#][10]

## .NET Font Rendering API - Installation {#NET-Font-Rendering-API-Installation}

[Aspose.Font for .NET][11] provides a powerful font rendering mechanism in order to render the text using TrueType and Type1 fonts. You can [download][12] the API or get it installed using [NuGet][13].

```
PM> Install-Package Aspose.Font
```

## Implement Text Rendering Interface {#Implement-Text-Rendering-Interface}

In order to achieve the text rendering, Aspose.Font for .NET provides an [IGlyphOutlinePainter][14] interface to draw the glyphs. The following steps demonstrate how to implement the methods in _IGlyphOutlinePainter_.

*   Implement the _IGlyphOutlinePainter_ interface methods using _GlyphOutlinePainter_ class which requires an object of type [System.Drawing.Drawing2D.GraphicsPath][15] for drawing graphics.

{{< gist aspose-com-gists 10f0e5f274b436379dbc8fd4fb183fc5 "Examples-CSharp-WorkingWithTrueTypeAndOpenTypeFonts-RenderingText-2.cs" >}}

*   Create a new method _DrawText()_ to draw the text into [System.Drawing.Bitmap][16] object.

{{< gist aspose-com-gists 10f0e5f274b436379dbc8fd4fb183fc5 "Examples-CSharp-WorkingWithTrueTypeAndOpenTypeFonts-RenderingText-3.cs" >}}

*   Define a utility method to calculate the font's width according to the image's width.

{{< gist aspose-com-gists 10f0e5f274b436379dbc8fd4fb183fc5 "Examples-CSharp-WorkingWithTrueTypeAndOpenTypeFonts-RenderingText-4.cs" >}}

## Render Text with TrueType Font using C# {#Render-Text-with-TrueType-Font-using-CSharp}

The following code sample shows how to use the above-mentioned implementation to render text with a TrueType font using C#.

{{< gist aspose-com-gists 10f0e5f274b436379dbc8fd4fb183fc5 "Examples-CSharp-WorkingWithTrueTypeAndOpenTypeFonts-RenderingText-1.cs" >}}

## Render Text with Type1 Font using C# {#Render-Text-with-Type1-Font-using-CSharp}

The following code sample shows how to render text with a Type1 font using C#.

{{< gist aspose-com-gists 10f0e5f274b436379dbc8fd4fb183fc5 "Examples-CSharp-WorkingWithType1Fonts-RenderingText-1.cs" >}}

## Conclusion

In this article, you have learned how to implement the rendering of text with a TrueType or Type1 font using C#. The code samples have shown how to generate JPG images based on the provided text. You can explore more about [Aspose.Font for .NET][17] using the [documentation][18].

## See Also

*   [Load, Save and Extract Information from Fonts using C#][19]




[1]: https://blog.aspose.com/2020/09/14/load-save-extract-information-from-fonts-using-csharp/
[2]: https://products.aspose.com/font/net
[3]: https://docs.fileformat.com/font/cff/
[4]: https://docs.fileformat.com/font/ttf/
[5]: https://docs.fileformat.com/font/type1/
[6]: https://docs.fileformat.com/image/jpeg/
[7]: #NET-Font-Rendering-API-Installation
[8]: #Implement-Text-Rendering-Interface
[9]: #Render-Text-with-TrueType-Font-using-CSharp
[10]: #Render-Text-with-Type1-Font-using-CSharp
[11]: https://products.aspose.com/font/net
[12]: https://downloads.aspose.com/font/net
[13]: https://www.nuget.org/packages/Aspose.Font
[14]: https://apireference.aspose.com/font/net/aspose.font.rendering/iglyphoutlinepainter
[15]: https://docs.microsoft.com/en-us/dotnet/api/system.drawing.drawing2d.graphicspath?view=dotnet-plat-ext-3.1
[16]: https://docs.microsoft.com/en-us/dotnet/api/system.drawing.bitmap?view=dotnet-plat-ext-3.1
[17]: https://products.aspose.com/font/net
[18]: https://docs.aspose.com/font/net/getting-started/
[19]: https://blog.aspose.com/2020/09/14/load-save-extract-information-from-fonts-using-csharp/





