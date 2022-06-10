---
title: 'Performance Improvements in Aspose.Words 10.6'
date: Sun, 30 Oct 2011 14:52:07 +0000
draft: false
url: /2011/10/30/performance-improvements-in-aspose.words-10.6/
author: Romank
summary: ''
tags: ['.NET', 'java', 'product release']
categories: ['Aspose.Words Product Family']
---

![Aspose.Words logo][1]

We have our regular monthly Aspose.Words release ready and you can download it from:

*   [Aspose.Words for .NET 10.6 (66 fixes and improvements)][2]
*   [Aspose.Words for Java 10.6 (77 fixes and improvements)][3]

In the rest of this post I am going to briefly talk about what's new.

## Page Layout Performance and Memory Optimizations

We have done some optimizations that reduce memory usage and increase speed when converting large documents to PDF, XPS or images. You should be able to convert bigger documents now. Our tests show 10-30% improvements. We are interested in your feedback too.

## More Load and Save Warnings for Fidelity Loss

In the earlier versions we introduced a mechanism for the user to receive warnings from Aspose.Words during loading, converting and saving documents. Aspose.Words issues warnings whenever a minor or major formatting or data loss occurs when converting a document. The warnings are sent to the **IWarningCallback** interface. In this release Aspose.Words issues a significantly more complete set of warnings for several conversion formats.

## Documentation: Working with Tables

In the previous release we have improved the public API for working with tables in Aspose.Words. This release follows up with a new section in the documentation and many new code examples.

As usual, the documentation is available online and also as part of the product download:

*   [Aspose.Words for .NET - Working with Tables][4]
*   [Aspose.Words for Java - Working with Tables][5]

## Other Fixes

There is a good number of other fixes and enhancements that resolve exceptions for particular documents, support some really weird custom footnote reference marks, display images better and so on. You can check the full listing on the release download page.




[1]: http://www.aspose.com/Images/aspose.words-logo2.jpg
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.words-for-.net/default.aspx
[3]: http://www.aspose.com/community/files/72/java-components/aspose.words-for-java/category1378.aspx
[4]: https://www.aspose.com/templates/aspose/App_Themes/V3/images/words/272x272/aspose_words-for-net.png
[5]: https://www.aspose.com/templates/aspose/App_Themes/V3/images/words/272x272/aspose_words-for-java.png




