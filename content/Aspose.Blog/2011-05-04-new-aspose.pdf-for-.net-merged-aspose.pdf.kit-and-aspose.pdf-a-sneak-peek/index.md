---
title: 'New Aspose.Pdf for .NET - Merged Aspose.Pdf.Kit and Aspose.Pdf: A Sneak Peek!'
date: Wed, 04 May 2011 06:35:12 +0000
draft: false
url: /2011/05/04/new-aspose.pdf-for-.net-merged-aspose.pdf.kit-and-aspose.pdf-a-sneak-peek/
author: Shahzad Latif
summary: ''
tags: ['Shahzad Latif', 'Aspose.Pdf', 'Aspose.Pdf.Kit', 'Merged Aspose.Pdf', 'PDF DOM API', 'PDF Editing']
---

We recently announced, in our March 2011 Newsletter, that we were going to merge Aspose.Pdf and Aspose.Pdf.Kit into a single Aspose.Pdf product. I'm very much excited to share with you that we have made quite a progress. And in this post, I'm going to give you a sneak peek into the developments so far. This post will give you insights into the new Aspose.Pdf, the reasons for merging both products, and the benefits it is going to provide to the developers.

## Why New Aspose.Pdf?

The developers have been successfully using [Aspose.Pdf][1] and [Aspose.Pdf.Kit][2] in their applications. Aspose.Pdf allows to create PDF files from scratch, while Aspose.Pdf.Kit helps manipulate existing PDF files. In the merged Aspose.Pdf, we're going to provide features for creating new PDF files and manipulating existing PDF files, in a single component.

Aspose.Pdf.Kit exposes various classes with different methods and properties. There was a big advantage of providing such an API: it was quite easy, for the developers, to implement various features quickly; and we still have this interface in our new component (I'll explain the related concepts in my next post). However, this interface had certain limitations:

1.  The user was limited to the functionality provided by methods exposed by these classes
2.  The interface was not consistent with our other products.

This new version of Aspose.Pdf is going to provide a [DOM based API][3] which is consistent with other products in the [Aspose product fleet][4]; this means, it will be quite easier to learn and provide more flexibility in terms of functionality.

Also, the developers had to use two different libraries for working with PDF files -- one for creating PDF files while the other one for manipulating existing files. The developers often used to get confused whether they should buy Aspose.Pdf, Aspose.Pdf.Kit, or both. With the merged API, they will have to buy a single component, and there will be no such confusion any more!

## Improvements in the Merged Aspose.Pdf!

As discussed earlier, the new Aspose.Pdf will provide a DOM based API consistent with other Aspose products. In addition to that, the new API will be quite flexible; you'll not be limited by the functionality provided by a particular method, rather you'll have DOM based access to the objects of the PDF files and will be able to manipulate the objects as you like.

Aspose.Pdf.Kit provides different sets of features in the form of classes; each class representing a different set of features. While using Aspose.Pdf.Kit, you have to open and close the PDF file with each class separately; however with the new API, you'll open and close the PDF file only once, which is going to reduce the overhead quite a bit. Above all, the underlying PDF processing mechanism (PDF Engine) is enhanced to provide faster and more reliable performance.

## What's Next?

We understand that with this change, you'll be having different questions like:

*   What kind of structure the new Aspose.Pdf will have?
*   What about backward compatibility?
*   When will this merged version be launched?
*   How much time will be required for migration?
*   What about training like samples, tutorials, demos?
*   How the licensing will work?

As this is an introductory post, I'm unable to cover all of these topics in this single post. However, I have planned to guide you through step by step and answer the above questions -- and any other questions you might have -- in my future posts and video tutorials.

## We Want You to be Part of It!

It is quite an excitement to work so closely with our teams through all the phases -- from planning to development. Everyone at Aspose is focused on providing a better and more flexible component to the users. However, we can make it even better for you, with your cooperation. We listened you in the past and we're happy to continue the legacy. We would really appreciate if you share your comments, suggestions, concerns, and questions. You may post your thoughts in the comments section of this post or in [Aspose.Pdf.Kit forum][5]. I'll provide you more insights, samples, tutorials and other information related to the merged Aspose.Pdf in the future posts. So, please stay tuned!




[1]: http://www.aspose.com/categories/.net-components/aspose.pdf-for-.net/default.aspx
[2]: http://www.aspose.com/categories/.net-components/aspose.pdf.kit-for-.net/default.aspx
[3]: http://en.wikipedia.org/wiki/Document_Object_Model
[4]: http://www.aspose.com/categories/.net-components/aspose.total-for-.net/default.aspx
[5]: http://www.aspose.com/community/forums/aspose.pdf.kit-product-family/215/showforum.aspx



