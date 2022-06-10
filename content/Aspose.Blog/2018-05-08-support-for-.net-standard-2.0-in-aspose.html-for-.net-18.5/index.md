---
title: 'Manipulate HTML Files in .NET Standard 2.0'
date: Tue, 08 May 2018 18:48:49 +0000
draft: false
url: /2018/05/08/support-for-.net-standard-2.0-in-aspose.html-for-.net-18.5/
author: Farhan Raza
summary: ''
tags: ['HTML API for .NET Core']
categories: ['Aspose.HTML Product Family']
---



{{< figure align=center src="images/aspose-html-for-net.png" alt="">}}


We are glad to announce a new release [Aspose.HTML for .NET 18.5][1] which is available on NuGet Gallery for download and to be used in .NET applications. This release includes an amazing feature of support for .NET Standard 2.0 (.NET Core) Framework. Several other enhancements and bug fixes have also been included in this version of Aspose.HTML for .NET. An overview of these improvements and changes is given in the [release notes][2] of Aspose.HTML for .NET 18.5.

## Rendering HTML Canvas in C# {#title-heading}

[W3C HTML Canvas][3] is a part of Aspose.HTML for .NET API now, it supports rendering of HTML Canvas elements as a part of HTML document as well as direct access and manipulation of HTML Canvas 2D Context. You can manipulate as well as render an HTML Canvas to other file formats including, but not limited to, XPS and PDF.  You can use the Rendering device as follows:

```
using (var document = new HTMLDocument(dataDir + "canvas.html"))
{
 // Create an instance of HTML renderer and XPS output device
 using (var renderer = new Rendering.HtmlRenderer())
 using (var device = new Aspose.Html.Rendering.Pdf.PdfDevice("canvas.pdf"))
 {
 // Render the document to the specified device
 renderer.Render(device, document);
 }
}
```

We have also improved the CSS engine that has contributed to improving the performance of parsing CSS documents up to 20 percent. **ParameterIsNotValid** exception, as well as few problems with the rendering of HTML to PNG format, have also been rectified in the latest version of Aspose.HTML for .NET API.

## Miscellaneous Resources

Please visit the following links for information regarding [Aspose.HTML for .NET 18.5][4] and [Release Notes][5] section.

*   [Home page for Aspose.HTML for .NET][6]
*   [Download Aspose.HTML for .NET][7]
*   [Aspose.HTML product family forum][8]– Post your technical questions and queries, or any other problem you faced while running Aspose.HTML APIs.
*   [Aspose.HTML for .NET online documentation][9]– help documentation on using Aspose.HTML for .NET API.
*   [Aspose.HTML for .NET API Reference][10]– Online public API reference for using the API.
*   [Enable Blog Subscription][11]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.HTML APIs, new features, fixes and other API related topics by subscribing to Aspose.HTML blog.




[1]: https://www.nuget.org/packages/Aspose.Html/18.5.0
[2]: https://docs.aspose.com/
[3]: https://www.w3.org/TR/2dcontext/
[4]: https://www.nuget.org/packages/Aspose.Html/18.5.0
[5]: https://docs.aspose.com/
[6]: https://products.aspose.com/html/net
[7]: https://www.nuget.org/packages/Aspose.Html/18.5.0
[8]: https://forum.aspose.com/c/html
[9]: https://docs.aspose.com/display/htmlnet/Home
[10]: https://apireference.aspose.com/net/html
[11]: https://blog.aspose.com/category/aspose-products/aspose-html-product-family/




