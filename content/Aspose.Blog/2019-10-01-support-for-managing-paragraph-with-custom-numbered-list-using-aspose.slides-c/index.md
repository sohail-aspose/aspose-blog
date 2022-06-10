---
title: 'Manage Paragraph with Custom Numbered List in Word Documents using C++'
date: Tue, 01 Oct 2019 19:10:37 +0000
draft: false
url: /2019/10/01/support-for-managing-paragraph-with-custom-numbered-list-using-aspose.slides-c/
author: Adnan Ahmad
summary: ''
tags: []
categories: ['Aspose.Slides Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2017/12/aspose_slides-for-cpp-128x128.png) Here we have a new release of Aspose.Slides for C++ 19.9, which has been enriched with new features. It can now support managing paragraph with custom numbered list. For this purpose, NumberedBulletStartWith property has been added to **IBulletFormat. **

In order to add a custom number list inside a paragraph, you first need to access the slide and add an auto shape. Then, you have to access the respective TextFrame of the shape and remove the default paragraph in that. Then create the first paragraph instance using Paragraph class and set **NumberedBulletStartWith **to 2 and second paragraph instance and set **NumberedBulletStartWith** 3.

The following code sample shows how to set a Paragraph with a custom numbered list.

{{< gist aspose-com-gists 81aeb05e6d3a070aa76fdea22ed53bc7 "Examples-SlidesCPP-SetFileTypeForAnEmbeddingObject-SetFileTypeForAnEmbeddingObject.cpp" >}}

Wait, there's many other features, enhancement, and bug fixes included in this release. [Here you can get the detail!][2]

When time allows you can check out API [examples at Github][3], talk about this release and other API related issues in our [forum][4].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2017/12/aspose_slides-for-cpp-128x128.png "Aspose.Slides for C++ logo"
[2]: https://docs.aspose.com/display/slidesnet/Aspose.Slides+for+.NET+19.9+Release+Notes
[3]: https://github.com/aspose-slides/
[4]: https://forum.aspose.com/c/slides




