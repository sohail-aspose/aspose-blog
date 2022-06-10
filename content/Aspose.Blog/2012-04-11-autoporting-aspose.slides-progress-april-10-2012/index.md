---
title: 'Autoporting Aspose.Slides progress, April 10, 2012'
date: Wed, 11 Apr 2012 08:00:31 +0000
draft: false
url: /2012/04/11/autoporting-aspose.slides-progress-april-10-2012/
author: Caroline Von Schmalensee
summary: ''
tags: ['.NET', 'Codeporting', 'Microsoft', 'PowerPoint', 'autoporting', 'java', 'programming', 'progress']
categories: ['Aspose.Slides Product Family']
---

![Aspose.Slides logo][1]

When Aspose started designing products, we focused on .NET. Some of our .NET products were very popular and we created versions of them for other platforms. We now also support Java, SharePoint, SQL Server Reporting Services and JasperReports. The .NET and Java products are similar in many ways: they are components and APIs that software developers use when creating their own applications.

In 2011, we decided to offer Aspose.Words for Java users the same features that our .NET users had access to. We had two options on how to do this: either, we could manually extend the Java APIs to include the features that the .NET APIs already had, or we could work out a way of automatically porting the .NET APIs to Java. The latter approach saves time and ensures that the two products stay synchronized. So that was the way we decided to work.

The Aspose.Words project was successful and we've worked steadily on autoporting our other projects too. We're currently working on Aspose.Slides.

# Aspose.Slides for .NET and Java

Aspose.Slides for .NET is currently at version 6.1. Aspose.Slides for Java sits at 2.9.1. As you can guess from the version differences, the two products are different in many ways:

## Aspose.Slides for .NET

## Aspose.Slides for Java

Create load and save PPT, POT, PPS, PPTX, POTX, PPSX. Save to PDF. Save to TIFF, XPS.

Create load and save PPT, POT, PPS, PPTX, POTX, PPSX. Save to PDF.

Render slides to raster and vector images.

Render slides to raster images.

Print presentations using flexible page and print settings.

N/A.

The autoporting process brings the .NET features across to Java. During the autoporting work we're also reviewing the code to improve performance, add a few features our customers have asked for and fix a number of issues. The final result will be not just one but two improved products.

# The autoporting process

So how do we go about autoporting a product? We work in C# to design the .NET product and use CodePorting, an internal utility that translates the code, line by line, to Java. We have a number of unit tests that we run to make sure that the two versions of the code produce the same output. Where there are differences, we make changes until the conversion works. It's a painstaking process but when we're finished, we can convert the .NET product to Java in seconds. Doing it this way, preparing the code for automatic conversion, is faster than writing the Java product from scratch to include the same features as the .NET product.

[To see an example from the Aspose.Word autoporting process, watch this video][2].

# Keeping you up to date

To keep you up to date on our progress, we'll post updates here every couple of weeks.




[1]: http://www.aspose.com/Images/aspose.slides-logo2.jpg
[2]: http://www.aspose.com/community/files/260350/download.aspx




