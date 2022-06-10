---
title: 'Automated PDF Printing and Adding Signature to PDF Documents Significantly Improved Productivity'
date: Mon, 18 Jan 2016 03:25:04 +0000
draft: false
url: /2016/01/18/automate-pdf-printing-and-adding-signature/
author: Max Hodges
summary: ''
tags: ['.NET API to print PDF files', 'Aspose.PDF', 'Inert Digital signatures in PDF files', 'Insert Digital signatures in PDF files without Adobe Acrobat', 'PDF file printing and digital signature capabilities', 'Print PDF files programatically', 'Print PDF files without using Adobe Acrobat', 'Success Stories']
categories: ['Aspose.PDF Product Family']
---

## About WHITE RABBIT EXPRESS



{{< figure align=center src="images/Screenshot-2020-04-15-at-4.06.12-AM.png" alt="White Rabbit Express logo">}}


We run [White Rabbit Express][1], a Tokyo-based proxy buying service. We’ve helped tens of thousands of people in over 100 countries buy-and-ship Japanese products which are difficult to get outside of Japan.

Our order fulfillment operations were very inefficient and manual labor-intensive. This was especially painful during Black Friday and Cyber Monday events which increased orders by several times our normal volume resulting in delays and an overworked staff.

Taking cues from Toyota’s process management principles, we were able to eliminate huge amounts of waste by allocating roles differently, creating custom software to manage the workflows, integrating barcode label printers & scanners, and reducing wasteful motions by replacing keyboards and mice with touch-screen monitors throughout the department.

## Problem

[Aspose.PDF for .NET][2] came to our aid in two key areas: [programmatic printing of PDF documents][3] and automatically [adding signatures to PDF documents][4].

Part of our shipping process involved submitting data to a Japan Post API. The API returned several shipping documents--dispatch note, customs declaration, and commercial invoices--in PDF format. Printing these documents from our web application has been time-consuming for users, who need to open the PDF in a new window, open the print dialog, click print, then close the tab. Since this activity was highly mechanical, it was clearly something we wanted to reduce.

Furthermore, once these documents were printed, our shippers need to sign as many as seven pages per shipment using a ballpoint pen. We decided to see what could be done to get signatures digitally inserted into the shipping documents.

## Solution

We built a .NET application using C# to handle the [printing of PDFs][5] using [Aspose.PDF for .NET][6]. Our application executed as a web server on the local machine, listening over localhost port. The PDF documents were posted from our Meteor web application to the localhost port where the .NET application received them and handled the printing operations. There were no print dialogs, no extra buttons to click, and no browser tabs for the user to close.

Next, we took the photo of a signature and saved it as a PNG image file with a transparent background. While using [Aspose.PDF for .NET][7] search tools, we programmatically iterated through each page of the PDF documents, while looking for keywords that indicated a signature as a required field. The signature image file was then inserted into the PDF before we saved and printed it.



{{< figure align=center src="images/white-rabbit-japan-aspose-pdf-case-study.png" alt="Preview of order fulfilment application" caption="Image 1:- Our in-house order fulfillment web application. Shipping document files in PDF format were passed to a .NET app running [Aspose.PDF for .NET](https://products.aspose.com/pdf/net).">}}




{{< figure align=center src="images/white-rabbit-japan-aspose-pdf-case-study-1.png" alt="Preview of signature being placed in PDF file" caption="Image 2:- Signatures like these are inserted on shipping documents automatically before being sent to the printer.">}}


## Experience

### **Finding a solution**

We evaluated several solutions before selecting [Aspose.PDF for .NET][8]. Acrobat Reader lacked an API and was hard to the remote control. GhostScript was very low-level, so it required a lot of work to do simple things. PDFSharp was basically a wrapper for Adobe Acrobat.

### **Implementation**

By using the [trial version][9] of [Aspose.PDF for .NET][10], I was able to start printing PDFs programmatically in minutes and had a working solution deployed within half-a-day. The [signature image merge][11] feature was implemented in about 3 hours of work. The code examples in the online [Developers guide at Aspose.PDF for .NET][12] were very valuable in helping us quickly build our solutions.

### **Outcome**

We believe making many small improvements to a process can result in large improvements. Speeding up a process by just one minute when shipping 10-20K packages resulted in several hundred hours of time-saving. [Aspose.PDF for .NET][13] allowed us to very rapidly deliver an automated solution, freeing our team from the manual grind of repetitive tasks.

**Max Hodges**, CEO  
White Rabbit Japan




[1]: https://www.whiterabbitexpress.com/
[2]: https://products.aspose.com/pdf/net
[3]: https://docs.aspose.com/display/pdfnet/Working+with+PDF+printing+-+Facades
[4]: https://docs.aspose.com/display/pdfnet/Digitally+sign+PDF+file
[5]: https://docs.aspose.com/display/pdfnet/Working+with+PDF+printing+-+Facades
[6]: https://products.aspose.com/pdf/net
[7]: https://products.aspose.com/pdf/net
[8]: https://products.aspose.com/pdf/net
[9]: https://downloads.aspose.com/pdf/net
[10]: https://products.aspose.com/pdf/net
[11]: https://docs.aspose.com/display/pdfnet/Digitally+sign+PDF+file
[12]: https://docs.aspose.com/display/pdfnet/Developer+Guide
[13]: https://products.aspose.com/pdf/net




