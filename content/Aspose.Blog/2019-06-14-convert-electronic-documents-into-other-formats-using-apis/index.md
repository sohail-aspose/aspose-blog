---
title: 'InFocus IT empowered Document Processing Solution to generate DOC and PDF files from XHTML'
date: Fri, 14 Jun 2019 07:34:42 +0000
draft: false
url: /2019/06/14/convert-electronic-documents-into-other-formats-using-apis/
author: Andrew Bates
summary: ''
tags: ['Customer Reviews', '.NET API with extensive documentation', '.NET to Convert XHTML to PDF format', 'Aspose.Words', 'Convert XHTML to PDF', 'Free Technical support', 'Free Trial Version', 'Parse XHTML and render output in PDF format', 'Render XHTML to DOC format', 'Simple and easy XHTML to PDF conversion', 'Success Stories']
categories: ['Aspose.Words Product Family']
---

## About InFocus IT



{{< figure align=center src="images/5d89c6d07f1c7_img.png" alt="InFocus Company Logo">}}


[InFocus IT][1] has been incorporated since 2005 and provides enterprise development services and solutions to a variety of different markets.

We deliver enterprise solutions that once deployed just work. Many of the systems that we develop or work with, generally have a large corpus of electronic content in a variety of file formats. Interchanging between these seamlessly can be a challenge.

## Problem

We constantly have a need to convert electronic documents into other document formats. We already had an experience of using [Aspose.Words for .NET][2] and found it to be a very reliable and stable product. Many solutions automated Word, but they are slow and not recommended by Microsoft on a server.

[Aspose.Words for .NET][3] enabled us to have no third-party deployed on a server to perform Document conversion quickly and easily.

We also have other solutions that we are looking to develop in the automatic capture of updates for publishing. We envisage that [Aspose.Words for .NET][4] will allow us to apply corrections and styling to the documents before they are supplied to the editorial.

## Solution

The publishing platform we developed holds the content in XHTML. This ensures that it can easily be published to various platforms easily and doesn’t carry too much overhead. Soon we realized that enabling legal customers to only download XHTML wasn’t going to deliver the value that our publishing platform required.

The publishing platform is built around a series of microservices that provide very focused functionality. One service is the export web API developed in C# and .NET Core. We aggregate the document to publish as part of the export operation. This adds headers and similar content. This is built up in XHTML.

In order to convert the XHTML to our supported export file formats (_DOCX and PDF_), we performed the following steps.

*   Added a reference to [Aspose.Words for .NET][5] via Nuget to the web API service
*   Loaded the aggregated XHTML document into [Aspose.Words for .NET][6], add the required headers and footers using the DocumentBuilder class
*   Saved the resultant document to the target file format

All of this functionality was delivered in roughly a page of code which was pretty impressive.

The end-user is unaware of this process as we obviously prepare the document on the server when the request is made to export content.



{{< figure align=center src="images/5d89c6d07f637_img.png" alt="" caption="Figure 1:- Optima Legal Online with the export to DOCX and PDF links top right. The users are presented with a link to open the prepared document.">}}




{{< figure align=center src="images/5d89c6d07fa54_img.png" alt="" caption="Figure 2:-– Zimbabwe Capital Gains Tax Act [Chapter 23:01], section exported from Optima Legal Online in PDF using [Aspose.Words for .NET](https://products.aspose.com/words/net).">}}


## Experience

We looked at various other options which all came in around the same cost but nothing else afforded the same level of robustness and functionality.

iTextPro had support for HTML to PDF conversion but they did not have support for DOCX. We could have supplemented that by writing our own DocumentFormat.OpenXml component but that would have taken a lot of effort to implement. We wanted to get away from automating Word so that wasn’t an option for us.

The implementation to [convert from XHTML to DOCX and PDF][7] literally took a day to write the code and perform unit tests around it. The object model was intuitive and very simple to achieve that we wanted to do.

The current solution meets the current export functionality for Optima Legal Online and we will be looking to utilize the other functionality in editorial systems and other systems that we will be looking to develop.

Using [Aspose.Words for .NET][8] probably saved us several months of development effort in developing our own solution and good developers aren’t cheap. [Aspose][9] delivered the product requirements over and above what we could have written as bespoke development.

## Next Steps

We will be looking to take [Aspose.Words for .NET][10] back into our editorial systems to enhance their functionality.

We are also looking to use it for styling captured legislation so that it can be published faster.

## Summary

It was so easy to implement the required functionality within our products saving us a lot of development time and money and also gave us functionality that we can enhance our products going forward.

I have worked with [Aspose][11] at previous client sites and back then, we did notice some niggles. We did raise these via the [support forum][12] and they were generally resolved with the next release which seems to be monthly and is good service.

We would highly recommend using [Aspose.Words for .NET][13] for document conversion and processing. It's intuitive and simple to add powerful capabilities around document composition and conversion.



[1]: http://infocusit.com/
[2]: https://products.aspose.com/words/net
[3]: https://products.aspose.com/words/net
[4]: https://products.aspose.com/words/net
[5]: https://products.aspose.com/words/net
[6]: https://products.aspose.com/words/net
[7]: https://docs.aspose.com/display/wordsnet/Converting+a+Document
[8]: https://products.aspose.com/words/net
[9]: https://www.aspose.com/
[10]: https://products.aspose.com/words/net
[11]: https://www.aspose.com/
[12]: https://forum.aspose.com/c/words
[13]: https://products.aspose.com/words/net




