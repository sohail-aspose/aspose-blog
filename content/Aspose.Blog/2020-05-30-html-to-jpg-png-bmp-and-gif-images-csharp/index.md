---
title: 'C# Convert HTML to JPG, PNG, BMP and GIF Image with .NET'
seoTitle: ""
description: ""
date: Sat, 30 May 2020 21:28:47 +0000
draft: false
url: /2020/05/30/html-to-jpg-png-bmp-and-gif-images-csharp/
author: Farhan Raza
summary: ''
tags: ['c# html to image', 'convert html to images in c#', 'html to bmp', 'html to gif', 'html to images', 'html to jpg', 'html to png']
categories: ['Aspose.HTML Product Family']
---

HTML files are frequently used over the internet. Subsequently, [Aspose.HTML for .NET][1] API supports a lot of features to work with HTML file format. In this article, we will be learning how to convert HTML to image using C#. Let us explore the following uses cases:

*   [Convert HTML to JPG Image using C#][2]
*   [Convert HTML to PNG Image using C#][3]
*   [Convert HTML to BMP Image using C#][4]
*   [Convert HTML to GIF Image using C#][5]

First of all, let us check the basic HTML file, containing some text and image, that we will be using as the input file in these examples.

```
<!DOCTYPE html>
<html>
<head>
<style>
body {
  text-align: center;
  color: black;
}
</style>
</head>
<body>
<h2>Welcome to HTML to Image C# Test Conversion</h2>

<img src="HTML to Image.png" alt="HTML to Image" style="width:300px">
</body>
</html>
```

## Convert HTML to JPG Image using C# {#section1}

You can convert HTML to JPG image using C# language in your .NET applications. The API supports several features for getting the output with different variations. For example, you can set the size of the output image as well as any background color that you want in your output image.

You need to follow the steps below for converting HTML to JPG image:

1.  Initialize image rendering options using [ImageSaveOptions][6] class
2.  Set page size or background-color
3.  Convert the HTML file

Furthermore, the following code shows how to convert HTML to JPG image using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "HTMLtoJPG.cs" >}}

Moreover, let us take a look at the generated output JPG image:



{{< figure align=center src="images/HTMLtoJPG-1.jpg" alt="HTML to JPG">}}


Furthermore, you can notice the background color and size of the image from the properties. The resolutions are 300dpi so the width and length of the image are 2100 because it is 7 inches in length and width.

## Convert HTML to PNG Image using C# {#section2}

PNG image files are more advanced files than JPG images. For example, they can have transparent backgrounds, unlike JPG images. Therefore, sometimes it is better to convert HTML to PNG image because it is a popular and compatible file format.

You can follow the steps below for the conversion:

1.  Load input HTML file
2.  Initialize an object of [ImageSaveOptions][7] class
3.  Convert HTML to PNG image

Following code snippet shows how to convert HTML file to PNG image using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "HTMLtoPNG.cs" >}}

## Convert HTML to BMP Image using C# {#section3}

You can convert HTML to BMP image using ImageFormat.Bmp property. Likewise, you should follow the below steps for the conversion:

1.  Load HTML file
2.  Set property with BMP [ImageFormat][8]
3.  Perform conversion with [Converter][9] class

Following code shows how to convert HTML to BMP image in C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "HTMLtoBMP.cs" >}}

## Convert HTML to GIF Image using C# {#section4}

**Info**: Aspose [Text to GIF][10] converter allows you to create fun animations just by typing.

HTML to GIF image conversion is an important feature of the API. You can convert the file with the following steps:

1.  Load input HTML document
2.  Specify [ImageSaveOptions][11] using GIF [ImageFormat][12]
3.  Call [ConvertHTML][13] method to convert HTML to GIF image

The code below shows how to convert HTML to GIF image using C# in your .NET applications:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "HTMLtoGIF.cs" >}}

## Conclusion

To sum up, we have learned how to convert HTML to JPG, PNG, BMP and GIF in .NET applications using C# or VB.NET. HTML conversion to these image formats is one of the most important features of Aspose.HTML for .NET API. Moreover, the converting or rendering results are with the highest fidelity and efficiency. That is why, the API is a best fit for converting, editing, or manipulating HTML files. Moreover, we look forward to hearing back from you. Please feel free to contact us via the [Free Support Forum][14] in case of any assistance.

## See Also

[Convert EPUB to PDF][15]




[1]: https://products.aspose.com/html/net
[2]: #section1
[3]: #section2
[4]: #section3
[5]: #section4
[6]: https://apireference.aspose.com/net/html/aspose.html.saving/imagesaveoptions
[7]: https://apireference.aspose.com/net/html/aspose.html.saving/imagesaveoptions
[8]: https://apireference.aspose.com/html/net/aspose.html.rendering.image/imageformat
[9]: https://apireference.aspose.com/net/html/aspose.html.converters/converter
[10]: https://products.aspose.app/slides/text-to-gif
[11]: https://apireference.aspose.com/net/html/aspose.html.saving/imagesaveoptions
[12]: https://apireference.aspose.com/html/net/aspose.html.rendering.image/imageformat
[13]: https://apireference.aspose.com/net/html/aspose.html.converters.converter/converthtml/methods/1
[14]: https://forum.aspose.com/c/html
[15]: https://blog.aspose.com/2020/06/17/epub-to-pdf-csharp/





