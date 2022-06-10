---
title: 'Join And Share implemented MS Office, Image, RFT, OpenOffice files rendering to PDF format as well as PDF printing using Aspose APIs'
date: Wed, 18 Jan 2012 06:41:00 +0000
draft: false
url: /2012/01/18/transform-various-file-formats-into-pdf-using-apis/
author: Thomas Grob
summary: ''
tags: ['.NET API to rotate Image file', 'Aspose.Total', 'Concatenate PDF files using Aspose.PDF for .NET', 'Convert DOC file to PDF format', 'Convert DOCX file to PDF format', 'Convert Excel files to PDF format', 'Convert Image to PDF format', 'Convert Image to PDF using Aspose.PDF for .NET', 'Convert TXT file to PDF format', 'Convert Uncompressed images to JPEG format', 'Excel files manipulation API', 'Insert Image into PDF document', 'OpenOffice document conversion to PDF suing Aspose.Words for .NET', 'Optimise Positioning of Image using Aspose.Imaging for .NET', 'Print PDF documents using Aspose.PDF for .NET', 'Programatically rotate image file', 'RFT to PDF conversion', 'Success Stories']
categories: ['Aspose.Total Product Family']
---

## About Join and Share GmbH



{{< figure align=center src="images/Screenshot-2020-05-05-at-3.31.12-AM.png" alt="Join and Share company logo">}}


[Join and Share GmbH][1] is located in Berlin, Germany. We develop customer-specific solutions based first and foremost on Microsoft products. Our certification for the Microsoft Silver Data Platform sets us apart as experts for database-oriented solutions in the field of business intelligence and enterprise applications.

Our team consists of Microsoft .NET experts, database developers for Microsoft SQL Server, Access and Office, Web developers, and UX Designers. Our customers are generally companies from the following sectors: transportation, insurance, housing, health care, education, and public administration.

## Problem

The Insurance Ombudsman is one of our long-term customers. It helps individual policyholders to have their complaints settled out of the courts' system in a cost-effective, efficient, and impartial way. In the past, documents for the arbitration process had to be sent by mail or fax. The new goal was that requests for the arbitration can be made on a web portal.

For the request, the complainant must be able to upload documents in a wide range of text and image file formats. The documents are first stored in a database and then combined in PDFs. In the file, [all pages are marked (_stamped_)][2] with the name and the file reference of the complaint. Finally, the requests are saved and printed as single PDF files.

A combination of open source and/or commercially available products is not the first choice for our development team because we don’t want to run into problems regarding the fine control and settings of the PDF produced. The requirement was to use a time-effective and easy solution.

## Solution

Unhesitatingly, we decided to evaluate [Aspose.Total for .NET][3] for the data processing of the various uploaded files.

The decision to use [Aspose.Total for .NET][4] was quickly made because we had very good results with the performance and flexibility of [Aspose.Words for .NET][5] in other projects. In our experience, the [Aspose product family][6] covers almost any feature one can have related to documents with a lot of additional functionality that would have otherwise taken a lot of time/cost to develop.

Some interesting aspects of the implementation:



{{< figure align=center src="images/About-join-and-share.png" alt="Code Snippet preview to convert Uncompressed image files to JPEG" caption="Image 1:- Uncompressed image files are converted to JPEG with the component Aspose.Image.">}}


The requirement was that the uploaded image files are printed on A4 sized paper with a defined resolution, picture quality, and margins. Easily and simply done with Aspose.PDF:



{{< figure align=center src="images/About-join-and-share-1-1024x110.png" alt="Aspose.PDF for .NET code snippet to convert Image to PDF" caption="Image 2:- Code snippet to convert Image to PDF format">}}


Pictures are easily rotated for an optimized positioning:



{{< figure align=center src="images/About-join-and-share-2-1024x109.png" alt="Code Snippet preview to optimise Image" caption="Image 3:- Code snippet to rotate and optimize the positioning of an image">}}


The text files (_Word, OpenOffice, RTF, TXT,…_) are quickly and safely [converted to PDFs with Aspose.Words for .NET][7]:



{{< figure align=center src="images/About-join-and-share-4.png" alt="Preview of Code snippet for Aspose.Imaging to process Image files" caption="Image 4:- Aspose.Imaging for .NET Code snippet to process Image files">}}


[Aspose.Cells][8] did the same job with Excel files with only four lines of code:



{{< figure align=center src="images/About-join-and-share-3-1.png" alt="Preview of Code snippet to convert Excel files to PDF format" caption="Image 5:- Code snippet to [convert Excel files to PDF format](https://docs.aspose.com/display/cellsnet/Convert+Excel+Workbook+to+PDF)">}}


The stamps for the documents are generated with [Aspose.PDF][9]:



{{< figure align=center src="images/About-join-and-share-5.png" alt="Preview of Code snippet to add Text Stamp to PDF documents." caption="Image 6:- Code snippet to [Add Text Stamp in PDF files](https://docs.aspose.com/display/pdfnet/Working+with+Stamps+and+Watermarks)">}}


Finally, the PDFs of a single query are transformed into a single PDF file, saved on a file server, and printed out. Quickly achieved with the **PdfFileEditor** and **PdfViewer** object of [Aspose.PDF for .NET][10]:



{{< figure align=center src="images/About-join-and-share-6.png" alt="Code snippet preview to Concatenate PDF files" caption="Image 7:- Code snippet to concatenate PDF files">}}




{{< figure align=center src="images/About-join-and-share-7.png" alt="" caption="Image 8:- Code snippet to [Print PDF documents](https://docs.aspose.com/display/pdfnet/Working+with+PDF+printing+-+Facades)">}}


## Experience

We have developed the application with the [evaluation version of Aspose.Total for .NET][11]. As expected, we are highly content with the results and absolutely convinced to use the product in future projects as well.

## Next Steps

We are planning to optimize the further processes of the customer with [Aspose.Total for .NET][12]. One task will be the [processing of incoming e-mails][13] with attachments.

## Summary

[Aspose.Total for .NET][14] is a powerful suite to process nearly all kinds of documents at high speed and great quality. It effectively reduces the programming effort. The [Aspose.Total for .NET][15] provides a clean and [well-documented][16] object-model. We also found many helpful code examples on the [Aspose website][17].

We would highly recommend the components to others.




[1]: http://www.join-and-share.de/
[2]: https://docs.aspose.com/display/wordsnet/Working+with+Watermark
[3]: https://products.aspose.com/total/net
[4]: https://products.aspose.com/total/net
[5]: https://products.aspose.com/words/net
[6]: https://products.aspose.com/total/net
[7]: https://docs.aspose.com/display/wordsnet/Converting+a+Document
[8]: https://products.aspose.com/cells
[9]: https://products.aspose.com/pdf
[10]: https://products.aspose.com/pdf/net
[11]: https://downloads.aspose.com/total/net
[12]: https://products.aspose.com/total/net
[13]: https://docs.aspose.com/display/emailnet/Working+with+MIME+Messages
[14]: https://products.aspose.com/total/net
[15]: https://products.aspose.com/total/net
[16]: https://docs.aspose.com/dashboard.action
[17]: https://www.aspose.com/




