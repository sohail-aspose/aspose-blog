---
title: 'SCONCE Uses Aspose.Words to Generate Word and PDF Files in a Web Application'
date: Sat, 30 Sep 2017 08:06:09 +0000
draft: false
url: /2017/09/30/creat-word-and-pdf-files-in-a-web-application-using-apis/
author: Meyyappan Annamalai
summary: ''
tags: ['Aspose.Words', 'Success Stories']
categories: ['Aspose.Words Product Family']
---

## About SCONCE



{{< figure align=center src="images/sconce.png" alt="">}}


SCONCE is a leading provider of PLM and MCAD services across a wide-range of industry verticals. Since 2001, SCONCE has helped many Fortune 1000 companies maximize the value of their PLM and MCAD technology investments. SCONCE deliver full spectrum of PLM services, business transformation including best practices, process consulting, PLM roadmaps, scoping and implementation services, legacy systems migration, custom enhancements, enterprise systems integration, training, enterprise architecture sizing and infrastructure systems support. With global presence, deep domain expertise, best practices, proven delivery methodologies and commitment to customers’ success, it’s a proven trusted services partner for any PLM solution.

SCONCE has developed its proprietary in-house product SCINTRA to cater to its end-to-end management of Leads, Sales Opportunities, Purchase Orders, Projects, Resources, and Performance. In addition to Services, SCONCE has its footprint in Products(Solutions) as Service by its State-of-the-art Shape Based Search (SBS) solution and Test Automation solutions.

## Problem

There is significant word processing involved in SCINTRA for its reports such as Invoices, Receipts, Project Plans, Pay Slips, which need to be generated in a seamless and secure manner. The reports have to be in both Office .docx as well as in PDF format, thus allowing flexibility to edit the word documents whenever required before generating the pdf files.

Since SCINTRA being a web application, Microsoft Interop could not be used and hence we were using OpenXML for the same. This meant that a Scheduler was required to be implemented for processing Word documents to PDFs. This posed overhead of constant queue monitoring on the server. This approach required manual cross-checking in few cases such as print-to-pdf which posed security loop-holes.

## Solution

We did a POC using [Aspose.Words for .NET][1] for generating Word and PDF documents and found that it was highly reliable, stable and secure for our requirement.

The overhead of manual checking is no more required with Aspose and we generate Office Word and PDF documents programmatically in a seamless manner.

Currently, we are using Aspose.Words for .NET for generating our invoices, receipts, payslips and we intend to make it as ‘the platform’ for all our Word processing needs of SCINTRA.



{{< figure align=center src="images/scintra-case-study-aspose-words.png" alt="">}}




{{< figure align=center src="images/scintra-case-study-aspose-words-1.png" alt="">}}




{{< figure align=center src="images/scintra-case-study-aspose-words-2-1024x319.png" alt="">}}


## Experience

We surfed and studied various products for Word/PDF generation and found that our experience of POC by using Aspose were highly positive and hence we proceeded with Aspose. The implementation and integration of Aspose to SCINTRA was seamless and looking forward to good customer support.

## Next Steps

As a next step, we have plans of using Aspose as ‘the-platform’ for all our Word Processing that involves Office Documents and PDF generation. We also have plans to expand usage of the same to our other divisions within the company such as for the Shape Based Search (SBS) solution and for Automation Solution reports generation.

## Summary

Our overall experience with [Aspose product][2] so far has been very impressive. Aspose integration to our product suite reduced our internal server processing overhead and ensured the generation of reports in a seamless, secure and reliable manner. We at Sconce wish Aspose all the very best for its future roadmap and look forward to our association for further business needs.

**Meyyappan Annamalai  
**CEO SCONCE



[1]: https://products.aspose.com/words/net
[2]: https://products.aspose.com/




