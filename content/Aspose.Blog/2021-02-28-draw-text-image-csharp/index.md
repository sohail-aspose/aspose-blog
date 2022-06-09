---
title: 'Add, Insert, or Draw Text on PNG, JPEG, TIFF, Icon, GIF Image using C#'
seoTitle: "C# Add Insert Draw Watermark Text in PNG JPG TIF Icon Image or Picture"
description: "You can add, insert, or draw watermark text with C# into PNG, JPG, TIFFm BMP, Icon, GIF and other image file formats. Draw text programmatically."
date: Sun, 28 Feb 2021 19:57:00 +0000
draft: false
url: /2021/02/28/draw-text-image-csharp/
author: Farhan Raza
summary: 'We see or create a lot of images for visual information. Sometimes you need to add or draw text on an image in such a manner that nobody else can modify that text. Image watermark is one of the most common examples. Likewise, labeling or reviewing images may also require drawing text.'
tags: ['add text on image', 'draw text on image', 'draw watermark on image in c#', 'insert text on image']
categories: ['Aspose.Drawing Product Family']
---



{{< figure align=center src="images/draw-text-image-csharp.png" alt="draw-text-image-csharp">}}


We see or create a lot of images for visual information. Sometimes you need to add or draw text on an image in such a manner that nobody else can modify that text. Image watermark is one of the most common examples. Likewise, labeling or reviewing images may also require drawing text. Let us explore the further uses of drawing text on images:

*   [Add, Insert, or Draw Formatted Text on Image – C# API Installation][1]
*   [Draw Text as Watermark on Existing Image Programmatically using C#][2]
*   [Draw Text on New Image from Scratch Programmatically in C#][3]

**Info**: Aspose recently developed a FREE [Text to GIF Converter][4].

## Add, Insert, or Draw Formatted Text on Image – C# API Installation {#section1}

[Aspose.Drawing for .NET][5] API is a 2D graphics library that is compatible with System.Drawing package. It supports rendering rectangles, curves, lines, text, and other graphics onto the images. It is not dependent on any 3rd party library thus can be used in any environment. For example, it can also be used to render graphics in Linux or Azure Functions V2 where System.Drawing library is not supported. You can install Aspose.Drawing for .NET API by downloading it from the [Downloads][6] section, or via the following installation command:

```
PM> Install-Package Aspose.Drawing
```

## Draw Text as Watermark on Existing Image Programmatically using C# {#section2}

Text watermark on Image is often used to show ownership, affiliation, or purpose of the picture. You can add or draw text as watermark on an existing image with the following steps:

1.  Load existing input image
2.  Initialize [Graphics][7] class object
3.  Set text formatting and text
4.  Draw text
5.  Save output image

The following code shows how to draw text as watermark on existing image programmatically using C#:

{{< gist aspose-com-gists b07fbc1311415962779e252ddb7437d8 "Draw-Text-Existing-Image.cs" >}}

## Draw Text on New Image from Scratch Programmatically in C# {#section3}

You may need to draw some text in image format for different purposes. Like you may want to keep others from modifying or copying text contents. You need to follow the following steps for drawing text on new image:

1.  Initialize new image from scratch
2.  Initialize [Brush][8] class object
3.  Set font style, size, etc.
4.  Draw text on the image
5.  Save output image

The code snippet below demonstrates how to draw text on new image from scratch programmatically using C# language:

{{< gist aspose-com-gists b07fbc1311415962779e252ddb7437d8 "Draw-text-new.cs" >}}

## Conclusion

In this article, we have learned how to add or draw text on images. You can draw text watermark in existing as well as new images from scratch without needing to install any 3rd party application. Moreover, you can process a lot of image formats including JPG, PNG, BMP, Icon, Tiff, etc. The API offers several features for processing drawings and graphics as per your requirements. You may visit the [Example Project][9] that we have designed as a showcase for different scenarios. Please feel free to contact us anytime via the [Free Support Forums][10] in case of any concerns. Cheers!

## See Also

[Using System.Drawing in Linux without libgdiplus][11]




[1]: #section1
[2]: #section2
[3]: #section3
[4]: https://products.aspose.app/slides/text-to-gif
[5]: https://products.aspose.com/drawing/net
[6]: https://releases.aspose.com/
[7]: https://apireference.aspose.com/drawing/net/system.drawing/graphics
[8]: https://apireference.aspose.com/drawing/net/system.drawing/brush
[9]: https://github.com/aspose-drawing/Aspose.Drawing-for-.NET
[10]: https://forum.aspose.com/c/drawing
[11]: https://blog.aspose.com/2020/12/13/using-system-drawing-in-linux/





