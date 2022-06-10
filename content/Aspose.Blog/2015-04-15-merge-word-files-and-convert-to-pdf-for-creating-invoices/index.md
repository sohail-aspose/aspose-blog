---
title: 'Concentra supports Mail Merge in Word Documents, their concatenation and Conversion to PDF for multi-branded batch invoices using APIs'
date: Wed, 15 Apr 2015 08:23:47 +0000
draft: false
url: /2015/04/15/merge-word-files-and-convert-to-pdf-for-creating-invoices/
author: Graham Kennedy
summary: ''
tags: ['.NET API for MS Word files processing', 'Aspose.Total', 'Convert DOC DOCX files to PDF format', 'Dynamically generate MS Word documents', 'Mail Merge fields with content from database', 'Mail Merge in MS Word files', 'Merge MS Word files using Aspose.Words for .NET', 'Render MS Word files to PDF format', 'Success Stories']
categories: ['Aspose.Total Product Family']
---

## About Concentra



{{< figure align=center src="images/3jsKLaXj_400x400.png" alt="Concentra logo">}}


[Concentra Consulting][1] is a business consulting and technology services company headquartered in London, UK. The company combines its core skills in consulting, analytics, and technology to provide custom solutions including analytical models, business intelligence, and operational systems through web-based products and bespoke software development. Within the Custom Development Services team, we design, develop, and host bespoke client solutions for the B2B and B2C markets.

## Problem

We needed to find another way to produce the batch and [online word merged invoices][2] for our client. The previous tools used were no longer supported, and the restrictive licensing meant their offering would not scale. The client's business had grown considerably and it was essential that we find an integrated solution that could scale in line with projected volumes. It was essential our developers work with an established provider, to ensure on-going technology updates and technical support.

We had to leverage the ability for our Clients Administrators to continue to maintain branded Word templates. We used [Aspose.Total for .NET][3] to generate invoices in PDF that can be routed through Printers, Print Factories, as email attachments, or electronic interfaces to Insurers.

## Solution

When developing the solution with the [trial version of Aspose.Total for .NET][4], we quickly found it intuitive to work with and were able to implement the merging, word and PDF output quickly. It was important to keep costs down for our clients.

To process the Microsoft Word template with merge fields extracted from the database, we have written a wrapper class as part of our solution library module. This library module uses ‘Aspose DLL’, and invokes methods to handle a document (_Open, Merge fields, Print, Save as PDF and Close_). In addition, we created two console applications for batch processing, referring to the "solution library module", our business logic invoked these console applications and printed or saved the mail merged documents. The end-user receives a printed invoice or PDF attached to an email.



{{< figure align=center src="images/About-Concentra-aspose-total-case-study-1024x194.png" alt="Preparation of the Batch Printing, and emailing run" caption="Figure 1: Preparation of the Batch Printing, and emailing run">}}




{{< figure align=center src="images/About-Concentra-aspose-total-case-study-1.png" alt="Sample unbranded PDF output Invoice" caption="Figure 2: Sample unbranded PDF output Invoice">}}


## Experience

The Custom Development team investigated a number of other products, including a custom-developed option using Office Open XML but quickly discounted this as it was more cost-effective to buy rather than build our own solution. We also used trial versions of the candidate offerings to implement a key feature of the solution, and concluded from the ease of use, and shorted delivery turnaround that [Aspose.Total for .NET][5] was the preferred candidate. The structure of the [Aspose.Total OEM license][6] means we can provide solutions for our other clients without additional license fees. The [documentation][7] and easy examples were a great help during implementation and were a key factor in reducing the implementation to three weeks.

We achieved our objectives of cost-effective solution deployment and achieved the clients’ requirement of both online and batch invoice processing, which is robust and can scale as their business grows.

## Next Steps

We plan to offer similar options to our other clients, using the capabilities offered by [Aspose.Total for .NET][8], including pre-packaged template PowerPoint outputs that merge Excel data to provide presentation decks to their own data analysts.

## Summary

We chose [Aspose.Total for .NET][9], because the product offered us all the tools to achieve our immediate objectives: speed of turnaround; hence lower cost to implement the solution, with the ability of the implementation to scale as our client’s business grows. We believe our future client implementations will allow us to use [Aspose.Total for .NET][10] capabilities for PowerPoint and Excel.




[1]: https://www.concentra.co.uk/
[2]: https://docs.aspose.com/display/wordsnet/Clone+and+Combine+Documents
[3]: https://products.aspose.com/total/net
[4]: https://downloads.aspose.com/total/net
[5]: https://products.aspose.com/total/net
[6]: https://purchase.aspose.com/pricing/total/net
[7]: https://docs.aspose.com/dashboard.action
[8]: https://products.aspose.com/total/net
[9]: https://products.aspose.com/total/net
[10]: https://products.aspose.com/total/net




