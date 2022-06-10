---
title: 'MailArchiva converts .EML to PST and MSG formats and programmatically processes iCal files using Java APIs'
date: Thu, 25 Apr 2013 13:00:00 +0000
draft: false
url: /2013/04/25/write-pst-data-in-java-using-apis/
author: Jamie Band
summary: ''
tags: ['.EML to MSG conversion using Aspose.Email for Java', '.EML to Microsoft PST format using Aspose.Email for Java', 'Aspose.Total', 'Convert Excel files to Image using Aspose.Cells for Java and render in Browser', 'Convert MS Word files to Image and display in browser', 'Save calendar information into iCal format', 'Success Stories']
categories: ['Aspose.Total Product Family']
---

## About MailArchiva



{{< figure align=center src="images/Screenshot-2020-05-15-at-1.28.02-AM.png" alt="Mailarchiva logo">}}


[MailArchiva][1] formerly named as Stimulus Software developed a high-quality email archiving software product for businesses of all shapes and sizes. Our goal has been to deliver an innovative, cost-effective, and reliable email archiving solution that satisfies the needs of our customers. Our flagship product, MailArchiva, is used by over 5000 companies worldwide and growing.

## Problem

Since the Enron disaster in 2001, businesses throughout the USA and Europe have required to archive their emails between five and seven years. If a court issues a subpoena for e-discovery records, companies are required to supply the information in a timely fashion or face severe penalties.

To comply with e-discovery records requests, it is imperative for companies to deploy email archiving and discovery software such as MailArchiva. The product makes it possible for companies to keep an accurate record of their email data, and to be able to supply the required information to the courts on request in a timely and accurate manner.

A key aspect of performing a records request is to be able to obtain the data in the correct format. Early versions of the MailArchiva product provided options for retrieving email data in .EML format (RFC 822). This presented a problem for many legal folks, as they primarily used Microsoft Outlook. They preferred receiving email data in Microsoft PST and Microsoft OST formats.

Recognizing the importance of providing email data in the correct format, we developed a utility to help customers export their precious email data to PST files. Unfortunately, at the time, there was no Java API available that could write PST files, we were forced to implement a separate standalone utility implemented in C++, and then later C# using Microsoft's API's.

This separate PST utility proved to be difficult for our customers to use as it was a separate download and could not leverage the powerful search and select functions available in the MailArchiva search console. Furthermore, the standalone utility required that Microsoft Office was installed on the client machine. We often found that people could not get the standalone utility to work due to communication problems with the archive server. What we really needed was a way to integrate the PST export function directly into the MailArchiva server search console.

## Solution

When we discovered that [Aspose][2] had a product that could actually write PST data in Java, we jumped up and down. All of the other Java PST libraries we had used in the past, such as JPST from Independentsoft and libPST only had the ability to read PST data, they did not have the ability to write PST data.

By integrating the [Aspose.Email for Java][3] into our product, not only could users [export to PST][4] directly from the MailArchiva web interface, but they could also [export to other formats such as MSG!][5] This could save our customers a significant amount of time since they no longer need to download and configure a separate export utility. Furthermore, they could use MailArchiva's powerful search interface to find the data they were looking for and immediately export data into the desired formats (_in a two-step process_).

Another huge plus for the Aspose solution is that their PST classes offer the ability to [save calendar information directly into iCal format][6]. Since we have recently added the ability for MailArchiva to be able to archive calendar information, we saved a huge amount of time, by not having to implement the conversion to iCal ourselves.



{{< figure align=center src="images/About-Stimulus-Software-aspose-total-case-study.png" alt="" caption="Image 1:- Export of data in PST Format">}}


## Experience

When we visited the [Aspose website][7], we immediately noticed the breadth and depth of their product range were enormous. Features that we didn't think were possible to implement, such as displaying Microsoft Office documents directly in our search interface, could be implemented with relative ease using the powerful capabilities of the [Aspose product][8] line.

When we posted a question about [how get images inside Word documents][9] embedded inline in an exported HTML document, we received prompt and useful information from the Aspose [technical support team][10]. In a matter of an afternoon, we had Word and Excel documents displaying correctly in the MailArchiva search console without the need for a browser plugin.

The success of the MailArchiva product depends so much on enabling our customers to work with different data formats. Our customers need flexible choices when importing and exporting data. We achieved this goal by using the [Aspose Email for Java][11] component and discovered that in fact, [Aspose.Total for Java][12] was what we were really looking for, as it enabled us to do so much more.

## Next Steps

While examining the [Aspose product][13] offerings, we found some new ideas on what we could add to our product. For instance, we realized that we could use their [OCR library][14] to index image data and make it searchable in the MailArchiva search console.

Now that we have Word and Excel documents viewable in our search interface, we are patiently waiting for Aspose to finish their auto port of the [Aspose.PDF for .NET][15] product. When the auto ported product is available, we will be implementing a PDF viewer right from within the MailArchiva search console. This feature will enable our customers to view PDF files from within their browser without the need for a PDF plugin.

## Summary

For Java-based products that work extensively with data formats, Aspose is the logical choice. While you may be able to find some libraries (_perhaps, even open-source ones_), that do what you need in a limited context, with Aspose, you get everything under one roof. Their offering is extremely broad, which ultimately means that you can give your customers flexible choices in the way that they manage their data.




[1]: https://www.stimulussoft.com/index
[2]: https://www.aspose.com/
[3]: https://products.aspose.com/email/java
[4]: https://docs.aspose.com/display/emailjava/Working+with+Messages+in+a+PST+File
[5]: https://docs.aspose.com/display/emailjava/Working+with+Outlook+Items
[6]: https://docs.aspose.com/display/emailjava/Working+with+Contacts+in+PST+File
[7]: https://www.aspose.com/
[8]: https://products.aspose.com/
[9]: https://docs.aspose.com/display/wordsnet/Working+with+Images
[10]: https://forum.aspose.com/
[11]: https://products.aspose.com/email/java
[12]: https://products.aspose.com/total/java
[13]: https://products.aspose.com/
[14]: https://products.aspose.com/ocr/java
[15]: https://products.aspose.com/pdf/net




