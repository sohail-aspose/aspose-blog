---
title: 'Detektei Müller GmbH Uses Aspose APIs for Generating Word and PDF Documents in ASP.NET Core'
date: Thu, 11 Apr 2019 02:52:50 +0000
draft: false
url: /2019/04/11/generating-word-and-pdf-through-aspo.net-core-using-apis/
author: Alper Tugal
summary: ''
tags: ['Aspose APIs to Generate Word and PDF', 'Aspose.Words', 'Detektei Müller GmbH', 'PDF API for .NET Core', 'Success Stories', 'Word API for .NET Core']
categories: ['Aspose.Words Product Family']
---

## About Detektei Müller GmbH



{{< figure align=center src="images/Detektie-Muller.png" alt="">}}


The "CitySpion" type of monitoring has proven its worth. Shoplifters – whether they are local professionals, drug addicts or crime tourists – have a hard time. We make life difficult for shoplifters and we make it sustainable.

## Problem

Problem We developed an ASP .NET Core web application which aggregates some data and generates reports as Word documents and as well as PDF documents. On the webserver, we don't have Word or Office applications installed. We started implementing our solution with the Open XML SDK. We could generate Word documents by filling the data within bookmarks. But one additional requirement was to export the document as PDF. This is not possible without any additional components.

## Solution

Now we generate our Word and PDF Document with [Aspose.Words for .NET][1]. This works perfectly for our requirements and was easy to implement and use. While other products had some issues with rendering images, barcodes, etc. Aspose generated the document every time like expected.



{{< figure align=center src="images/dokumente-case-study-aspose-words.png" alt="" caption="Our Web Portal to add the data which will be used to generate word document">}}


The first image shows that we can upload a Word document as a template. Then we read out all bookmarks within the document and you can map these with specific fields from our Database. You could also map images or a checkbox.



{{< figure align=center src="images/dokumente-case-study-aspose-words-1.png" alt="" caption="It's an example of our generated word document">}}


## Experience

We tried out many ways to convert the Word document into a PDF File. As first we tried out with Microsoft OneDrive. The goal was here to upload the file to OneDrive and then download it as PDF document directly from OneDrive but for this option, we need licenses from OneDrive per end-user.

The second solution we tried out was with Microsoft Flow. We created a Flow that was triggered by an Http Request. The request sends the document to the Flow and as a response, we received a PDF. There was also the licensing of the problem for us. We also tried to convert the document into HTML and then from HTML to PDF. For this, we used some free libraries. The problem here was the header and footer of Word documents. This concept is not clearly supported in the HTML.

In the end, we tried out different contributors which provide libraries like Aspose. Some other libraries have some limitations or didn't fit our needs.

## Next Steps

*   We want to make it possible to add dynamic lists to the template, which will be filled by a list of data. Aspose.Words makes us life easier to reach this goal.
*   With [Aspose.BarCode][2] we will also be able to generate barcodes which we need maybe in the future for our reports as well.

## Summary

We thought generating PDF will be very easy with .NET but we ended up with a raising white flag. We are not able to implement this by ourselves. In the end, we found with Aspose Words the best solution which matches our requirements. We recommend Aspose Words to a developer who struggling with manipulating or generating Word documents.

**Alper Tugal  
**Detektei Müller GmbH




[1]: https://products.aspose.com/words/net
[2]: https://products.aspose.com/barcode




