---
title: 'Support for HTML to Markdown Notation in Aspose.HTML for .NET 18.6'
date: Mon, 18 Jun 2018 22:17:16 +0000
draft: false
url: /2018/06/18/support-for-html-document-to-markdown-notation-in-aspose.html-for-.net-18.6/
author: Farhan Raza
summary: ''
tags: []
categories: ['Aspose.HTML Product Family']
---



{{< figure align=center src="images/aspose-html-for-net.png" alt="">}}


We at Aspose are glad to announce new release [Aspose.HTML for .NET 18.6][1] which can be downloaded from NuGet Gallery and can be used in .NET applications. You can convert an HTML document to a Markdown format to make the content easy-to-read and easy-to-write. In this release, some issues related to HTML to PDF and PNG rendering have also been rectified. An overview of these improvements and changes is given in the [release notes][2] of Aspose.HTML for .NET 18.6.

## HTML to Markdown Conversion {#title-heading}

Markdown allows you to write using an easy-to-read and easy-to-write plain text format, then convert it to structurally valid HTML. You can convert your document to markdown format with Aspose.HTML for .NET 18.6.  HTML document can be converted to Markdown notation as follows:

**C#**

```
using (var document = new Aspose.Html.HTMLDocument("my first paragraph" +"my second paragraph", dataDir)){document.Save( dataDir + "Markdown.md", HTMLSaveFormat.Markdown);}
```

  
We have also included support to render HTML documents to MHTML File Format. You can even control the saving process by creating **MHTMLSaveOptions** object and setup relevant fields, as per your requirements. For further information about it, you may visit [HTML to MHTML Conversion][3].

## Miscellaneous Resources

Please visit the following links for information regarding [Aspose.HTML for .NET 18.6][4] and [Release Notes][5] section.

*   [Home page for Aspose.HTML for .NET][6]
*   [Download Aspose.HTML for .NET][7]
*   [Aspose.HTML product family forum][8]– Post your technical questions and queries, or any other problem you faced while running Aspose.HTML APIs.
*   [Aspose.HTML for .NET online documentation][9]– help documentation on using Aspose.HTML for .NET API.
*   [Aspose.HTML for .NET API Reference][10]– Online public API reference for using the API.
*   [Enable Blog Subscription][11]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.HTML APIs, new features, fixes and other API related topics by subscribing to Aspose.HTML blog.




[1]: https://www.nuget.org/packages/Aspose.Html/18.6.0
[2]: https://docs.aspose.com/
[3]: https://docs.aspose.com/
[4]: https://www.nuget.org/packages/Aspose.Html/18.6.0
[5]: https://docs.aspose.com/
[6]: https://products.aspose.com/html/net
[7]: https://www.nuget.org/packages/Aspose.Html/18.6.0
[8]: https://forum.aspose.com/c/html
[9]: https://docs.aspose.com/display/htmlnet/Home
[10]: https://apireference.aspose.com/net/html
[11]: https://blog.aspose.com/category/aspose-products/aspose-html-product-family/




