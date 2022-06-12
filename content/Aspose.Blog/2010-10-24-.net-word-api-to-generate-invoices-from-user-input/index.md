---
title: 'Gekom used .NET Word API to Generate Invoices from User Input and Word template'
seoTitle: "Gekom used .NET Word API to Generate Invoices from User Input and Word template"
description: ""
date: Sun, 24 Oct 2010 12:54:17 +0000
draft: false
url: /2010/10/24/.net-word-api-to-generate-invoices-from-user-input/
author: Gekom
summary: ''
tags: ['Aspose.Words', 'Convert MS Word files to PDF format', 'Dynamically render custom data into Word template', 'Generate dynamic Word documents based on template', 'Image Merge Fields in Word document', 'Insert custom company logo into Word document', 'Mail Merge in MS Word files', 'Success Stories', 'mail merge with regions']
categories: ['Aspose.Words Product Family']
---

## About Gekom



{{< figure align=center src="images/Gekom.jpg" alt="Gekom company logo">}}


[Gekom][1] is an online web application that offers small companies and freelancers a secure, reliable, and easy way to manage their customers’ quotes and invoices wherever they are. Gekom customers can quickly create and download an invoice in order to send it by e-mail or print it out.

## Requirements

During the development of Gekom, one of the major difficulties was to find the right way to handle document generation. While using a database engine to store user input is a very common issue that is not difficult for a developer to solve but document generation is not a straightforward task. The main requirements while building Gekom were:

*   To generate invoices from both user input and database records
*   To [include images such as company logos][2] on invoices
*   To be able to manage invoice templates easily

The third requirement was probably the most interesting to solve: the question was how to use Microsoft Word for authoring templates without using Microsoft Word for generating invoices?

## Actors

The above-specified scenario was supposed to be performed daily by all users of the application.

## Solution

After several tries and non-convincing results, the answer was found: [Aspose.Words for .NET][3].



{{< figure align=center src="images/Gekom-case-study-aspose-words-1024x605.png" alt="Generate Invoices as Words document" caption="Image 1:- Collecting user input from within an ASP.NET WebForms application.">}}




{{< figure align=center src="images/Gekom-case-study-aspose-words-1-1024x605.png" alt="Invoice download preview" caption="Image 2:- Downloading the invoice once it has been generated server-side.">}}




{{< figure align=center src="images/Gekom-case-study-aspose-words-2.png" alt="PDF preview of resultant invoice" caption="Image 3:- The result was a tailor-made invoice showing the chosen company logo.">}}


## Products Used

[Aspose.Words for .NET][4] has been used to build this use case into an ASP.NET web application written in C#. The following functionalities of [Aspose.Words for .NET][5] were used:

*   Simple [mail merge using Microsoft Word][6] template
*   [Mail merge with regions][7]
*   [Image merge fields][8]
*   [Save Word document as PDF][9]

## Why Aspose?

As a software developer, we have been facing the document generation challenges several times, in several contexts. We already have been using:

*   Word/SpreadsheetML in conjunction with XML data and XSLT transforms
*   Office automation
*   XSL-FO language and processors  
    

But we were never convinced by any of these solutions: performance, easy templates management, and data integration requirements were never met all together.

Once we implemented real-world scenarios using [Aspose.Words for .NET][10], we got to know for the first time, which components we will continue using.

## Future Implementations

[Aspose.Words for .NET][11] provided a so simple solution to our main requirement (_that was to be able to [manage templates using Microsoft Word][12]_), that we seriously consider extending the use of other components. We consider providing the end-users with a way to generate monthly Excel extracts using [Aspose.Cells for .Net][13].

## Conclusion

We are really convinced about the quality and the robustness of [Aspose components][14] and would recommend every software developer to have a look at it.




[1]: https://www.Gekom.cz/
[2]: https://docs.aspose.com/display/wordsnet/Working+with+Images
[3]: https://products.aspose.com/words/net
[4]: https://products.aspose.com/words/net
[5]: https://products.aspose.com/words/net
[6]: https://docs.aspose.com/display/wordsnet/Mail+Merge+and+Reporting
[7]: https://docs.aspose.com/display/wordsnet/How+to+Use+Nested+Mail+Merge+Regions
[8]: https://docs.aspose.com/display/wordsnet/Working+with+Images
[9]: https://docs.aspose.com/display/wordsnet/Converting+a+Word+document+to+PDF
[10]: https://products.aspose.com/words/net
[11]: https://products.aspose.com/words/net
[12]: https://docs.aspose.com/display/wordsnet/Loading%2C+Saving+and+Converting
[13]: https://products.aspose.com/cells/net
[14]: https://products.aspose.com/




