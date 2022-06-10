---
title: 'Introduction to Merged Aspose.Pdf API'
date: Sat, 14 May 2011 07:26:36 +0000
draft: false
url: /2011/05/14/introduction-to-merged-aspose.pdf-api/
author: Shahzad Latif
summary: ''
tags: ['Shahzad Latif']
---

In my previous post, I explained that why we are introducing merged Aspose.Pdf, what benefits it is going to give to the developers, and how you can share your thoughts and suggestions. You may read that post at the following link: New Aspose.Pdf for .NET – Merged Aspose.Pdf.Kit and Aspose.Pdf: A Sneak Peek!. In this post, I'm elaborating different parts of the merged Aspose.Pdf. I have included a diagram showing the architecture of the new Aspose.Pdf. A video tutorial, explaining the use of this new component and various namespaces included in the merged product, is also a part of this post. ![Overview of Merged Aspose.Pdf Architecture][1]

From the above diagram, you can see that there are three main parts of the new Aspose.Pdf: old Aspose.Pdf, Old Aspose.Pdf.Kit, and new Aspose.Pdf DOM API.

## Support for Legacy Code

**Aspose.Pdf.Generator** namespace corresponds to the old Aspose.Pdf. All the namespaces and classes previously available in the old Aspose.Pdf can be found under this namespace. **Aspose.Pdf.Facades** namespace contains all the namespaces and classes provided by old Aspose.Pdf.Kit. If you want to use this new component with your legacy code then you can use these two namespaces. Most of the code will remain same; there will be only small changes due to the fact that we wanted to take advantage of the new PDF Engine. However, those changes are minor, and I'll also explain the required changes separately.

## New DOM API

All the namespaces except the two mentioned above belong to the new **DOM API**. In order to take full advantage of the flexibility provided by merged component, you need to migrate to the Aspose.Pdf DOM API. Also, as this API is consistent with other Aspose components, this will help you standardize your applications as well.

## Challenge Your Creativity

You also need to understand another important aspect of the new component. You can see, in the above diagram, that Aspose.Pdf.Facades namespace is accessing the DOM API. This is because, although the interface is similar to the Aspose.Pdf.Kit for backward compatibility, the internal implementation is revamped to provide better results. Now, you have got two options for editing your PDF files: use Aspose.Pdf.Facades to implement the code quickly to save you the time, or use DOM API to solve complex business scenarios and challenge your creativity as well!

## Introductory Video Tutorial

I have also created a video tutorial which explains different parts of the merged API. This video walks you through the namespaces provided by the merged Aspose.Pdf. Please watch this video tutorial for better understanding of the new component.

This video tutorial can also be found on the YouTube at the following URL: [Introduction to Merged Aspose.Pdf][2].

## Stay Tuned!!

In my upcoming blog posts and tutorials, I'll show you the code snippets and samples of the merged API. In the meanwhile, if you have any questions or concerns, please do share with us.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2011/05/Overview-of-Merged-Aspose.Pdf-Architecture.gif "Overview of Merged Aspose.Pdf Architecture"
[2]: http://www.youtube.com/watch?v=xdTnxgQ8UgY



