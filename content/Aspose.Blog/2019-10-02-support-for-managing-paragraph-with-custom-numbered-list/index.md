---
title: 'Manage Paragraph with Custom Numbered List in PowerPoint using C#'
date: Wed, 02 Oct 2019 04:01:23 +0000
draft: false
url: /2019/10/02/support-for-managing-paragraph-with-custom-numbered-list/
author: Adnan Ahmad
summary: ''
tags: []
categories: ['Aspose.Slides Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Slides-for-net_100.png) Here comes new release of [Aspose.Slides][2] for .NET and Java, which has been enriched with new features. It can now support managing paragraphs with custom numbered list. For this purpose, NumberedBulletStartWith property has been introduced in **IBulletFormat. **

In order to add a custom number list inside a paragraph, you first need to access the slide and add an auto shape. Then, you have to access the respective TextFrame of the shape and remove the default paragraph in that. You then need to create a new paragraph instance using Paragraph class and set **NumberedBulletStartWith **to 2 and second paragraph instance and set **NumberedBulletStartWith** 3.

The following code sample shows how to set Paragraph with custom numbered list.

{{< gist aspose-com-gists a56eda38c01ad33dc653116c7bae4293 "Examples-CSharp-Text-SetCustomBulletsNumber-SetCustomBulletsNumber.cs" >}}

The similar Java based example for this is:

{{< gist aspose-com-gists 1f55f0222bc39a382d831900e8de7400 "Examples-src-main-java-com-aspose-slides-examples-Text-SetCustomBulletsNumber-SetCustomBulletsNumber.java" >}}

Wait, there's many other features, enhancement, and bug fixes included in this release. [Here you can get the detail!][3]

When time allows you can check out API [examples at Github][4], talk about this release and other API related issues in our [forum][5].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Slides-for-net_100.png "Aspose.Slides or .NET logo"
[2]: https://products.aspose.com/slides
[3]: https://docs.aspose.com/display/slidesnet/Aspose.Slides+for+.NET+19.9+Release+Notes
[4]: https://github.com/aspose-slides/
[5]: https://forum.aspose.com/c/slides




