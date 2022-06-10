---
title: 'Text Wrapping Around Images and Shapes in Word Document using C# .NET'
date: Mon, 10 Jan 2011 00:32:00 +0000
draft: false
url: /2011/01/10/text-wrapping-around-images-and-shapes-is-about-to-be-released-in-aspose-words-for-net/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

I am happy to announce that a very cool and important feature is going to be included in Aspose.Words for .NET 9.6 that is about to be released in just a few days.

Text wrapping around images and shapes when rendering Microsoft Word documents to PDF, XPS, and printing is now supported. This is a major milestone for Aspose.Words in achieving the "high fidelity rendering" goal.

In Microsoft Word documents text can wrap around shapes in the following ways (I also indicate what is supported by Aspose.Words):

*   **Square - supported now**
*   Tight - not yet supported
*   Through - not yet supported
*   **Top and Bottom - supported now**
*   Behind/In Front of Text - was already supported
*   Inline with Text - was already supported

The four wrapping types now supported cover the majority of user scenarios. Tight and Through are used rarely - they refer to text flowing neatly around a complex shape contour, such as a picture of a dog for example. Although Tight and Through are used rarely, we are very likely to support them in one of the further versions.

The picture below shows how Aspose.Words has rendered a document into an image. That image is semi-transparent and overlayed and displayed on top of the original text document opened in Microsoft Word. We use this harness for testing Aspose.Words outputs. You can see how good the result is.

And the nicest thing of all - we have already auto-ported this feature to Java and it is already part of the auto-ported version of Aspose.Words for Java that we [rushing to release][1].

I would like to thank our hard-working developers who made this possible and also thank the hard waiting customers - you all helped make this great feature possible.




[1]: https://blog.aspose.com/category/words/




