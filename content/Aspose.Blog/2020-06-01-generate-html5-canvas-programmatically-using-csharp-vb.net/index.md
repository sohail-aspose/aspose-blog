---
title: 'Generate HTML5 Canvas Programmatically using C#'
seoTitle: "Generate HTML5 Canvas using C# | Export SVG to HTML5 Canvas in C#"
description: "Dynamically generate HTML5 Canvas element using C#. Export SVG, CMX, EMF, WMF, and CDR to HTML5 Canvas. Embed canvas in a web page dynamically using C#."
date: Mon, 01 Jun 2020 18:16:12 +0000
draft: false
url: /2020/06/01/generate-html5-canvas-programmatically-using-csharp-vb.net/
author: Usman Aziz
summary: ''
tags: ['SVG to HTML5 Canvas', 'export svg to html5 canvas', 'generate html5 canvas using csharp']
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/aspose-Imaging-for-net_100.png" alt="Create HTML5 Canvas using C#">}}


In this article, I will show you how to generate the HTML5 Canvas element with graphics using C#. You can embed this feature within your .NET web applications for the dynamic generation and integration of HTML5 Canvas on web pages.

[HTML5 Canvas][1] element is used to draw graphics on the fly within the web pages. It provides you with an area that acts as a container of graphics or drawing objects. You can draw paths, boxes, texts, images, and other objects and then render them into image formats. [Aspose.Imaging for .NET][2] allows you to generate an HTML5 Canvas element using C# or VB.NET. This feature lets you create the HTML5 Canvas dynamically and set its source graphics file within your web applications such as ASP.NET application. So let's proceed further to check how to create the HTML5 Canvas element using C# with Aspose.Imaging for .NET API.

*   [C# API to Generate HTML5 Canvas - Installation][3]
*   [Create a Web Page with HTML5 Canvas using C#][4]
*   [Generate HTML5 Canvas Element Only using C#][5]

## C# API to Generate HTML5 Canvas - Installation {#CSharp-API-to-Generate-HTML5-Canvas-Installation}

First of all, let's have a look at how to install Aspose.Imaging for .NET within your .NET application. It's as simple as pie. You may either add a reference to API's [DLL][6] or install it using [NuGet Package Manager][7].

```
PM> Install-Package Aspose.Imaging
```

## Create a Web Page with HTML5 Canvas using C# {#Generate-Web-Page-with-HTML5-Canvas-using-CSharp}

HTML5 Canvas allows you to set a source image that would appear within the canvas area. Using Aspose.Imaging for .NET, you can export CDR, CMX, EMF, WMF, and SVG graphics to an HTML5 Canvas without worrying about the HTML, JavaScript, and CSS code. The following are the steps to create an HTML page having an HTML5 Canvas element on it.

*   Load a graphics file that you want to set as a source of the canvas using [Image.Load()][8] method.
*   Create HTML5 Canvas by exporting the image using [Image.Save()][9] method.

The following code sample shows how to create HTML5 Canvas with graphics using C#.

{{< gist aspose-com-gists 2d1bcb9853315458808ffbcd9e7e3e02 "Examples-Export-HTML5-Canvas.cs" >}}

## Generate HTML5 Canvas Element Only using C# {#Generate-HTML5-Canvas-Element-Only-using-CSharp}

In the previous example, we have generated a complete HTML page that contains the HTML5 Canvas element. However, in certain cases, you may need to generate the canvas element only to embed it within your web page. For such cases, you can configure Aspose.Imaging API to avoid generating the complete HTML page. The following are the steps to generate the HTML5 Canvas element.

*   Load a graphics file to set as a source of the canvas using [Image.Load()][10] method.
*   Set [Html5CanvasOptions.FullHtmlPage][11] proptery to false.
*   Export the image to HTML using [Image.Save()][12] method.

The following code sample shows how to create the HTML5 Canvas element only using C#.

{{< gist aspose-com-gists 2d1bcb9853315458808ffbcd9e7e3e02 "Examples-Export-HTML5-Canvas-Add-To-Existing-HTML.cs" >}}

## Conclusion

This article covered how to generate HTML5 Canvas dynamically using C# within .NET applications. We have seen how to create the complete HTML page containing an HTML5 Canvas or HTML5 Canvas only using Aspose.Imaging for .NET. You can explore more about the API using the [documentation][13].

## See Also

*   [Convert DICOM to JPEG, GIF, PNG, and BMP Images using C#][14]




[1]: https://en.wikipedia.org/wiki/Canvas_element
[2]: https://products.aspose.com/imaging/net
[3]: #CSharp-API-to-Generate-HTML5-Canvas-Installation
[4]: #Generate-Web-Page-with-HTML5-Canvas-using-CSharp
[5]: #Generate-HTML5-Canvas-Element-Only-using-CSharp
[6]: https://downloads.aspose.com/imaging/net
[7]: http://nuget.org/packages/Aspose.Imaging
[8]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/load/methods/2
[9]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/save/methods/3
[10]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/load/methods/2
[11]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/html5canvasoptions/properties/fullhtmlpage
[12]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/save/methods/3
[13]: https://docs.aspose.com/display/imagingnet/
[14]: https://blog.aspose.com/2020/04/01/convert-dicom-to-jpeg-gif-png-bmp-images-in-csharp-net/





