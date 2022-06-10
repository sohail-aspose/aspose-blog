---
title: 'C2S Implemented Fast and accurate Email Message Processing, Attachments Extraction and Conversion of Word and Excel to TIFF format'
date: Mon, 27 Jul 2015 07:59:06 +0000
draft: false
url: /2015/07/27/fast-and-accurate-document-conversion-using-apis-case-study/
author: Martin Peirce
summary: ''
tags: ['.NET API to convert DOC DOCX files to TIFF format', '.NET API to render MS Word files to TIFF format', 'Aspose.Cells for .NET To convert Excel files to TIFF image', 'Aspose.Email to extract attachments from Email message', 'Aspose.Total', 'Control ColorMode and Resolution during TIFF creation', 'Convert Excel files to TIFF format', 'Extract attachments from Email Message', 'MS Word file to TIFF conversion API', 'Programatically process Email Messages using Aspose.Email for .NEt', 'Render DOC DOCX files to TIFF format', 'Success Stories']
categories: ['Aspose.Total Product Family']
---

## About C2S



{{< figure align=center src="images/logo-1.png" alt="C2S company logo">}}


[C2S][1] provide document processing solution for accounts payable and digital mailroom.

At the core of our solution are two systems - ABBYY OCR & FileDirector Document Management. Both systems process and handle documents that are images like PDF or Tiff perfectly. ABBYY OCR cannot recognize existing text documents like Excel or Word and FileDirector will only allow annotations of scanned documents like Tiff.

## Problem

C2S has always struggled to find a consistent solution for document handling that can carefully and accurately convert documents. We then came across the [Aspose.Total for .NET][2].

## Solution

Having previously used PDF# and other open-source libraries, we were more often than not left disappointed by the performance. Our clients required bulletproof processing and accuracy.

During the development of our Santiago tool, we had a specific customer requirement that made us search and find a perfect solution. Santiago is a scheduler that monitors email accounts and downloads attachments that meet set rules. The attachments are then forwarded into a workflow. Santiago effectively feeds a digital mailroom or accounts payable solution.

The customer in question received attachments from over 500 branches around London. The attachments were agendas and minutes of meetings and were in any format including Word or Excel. We needed to forward these into our FileDirector solution, fully indexed into the correct queue but the customer asked to be able to [annotate the documents][3] – add text, arrows, highlights, etc. This appeared to be only possible if we converted the documents into Tiff.

Therefore, we have now uses [Aspose.Total. for NET][4] library into Santiago with excellent results.

## Experience

The Santiago email downloader solution has been designed to be completely modular and therefore extremely flexible. The system is designed to download emails, extract information, and save it as required. It is capable of saving not just the attachments of an email, but also the body (_[both HTML and plain text][5]_) and the metadata (_[sender address, recipient addresses, subject, date, etc][6]_) and we save this in a range of formats.

The primary requirement that led us to [Aspose.Total for .NET][7] was the need to convert documents (_mainly MS Word and_ [_Excel formats_) into TIFF][8]. We experimented with several different libraries but [Aspose.Total for .NET][9] was by far the best solution.

Santiago operates by downloading emails as .eml files into a user-designated folder, from this folder the Data Extraction module picks up the .eml file, [extracts the required documents][10], and saves this to a further designated folder. Finally, the File2Tiff module picks up the extracted documents, performs the conversion, and again saves them to the final location where they can be collected by the FileDirector system for archiving.



{{< figure align=center src="images/About-C2S-aspose-total-case-study.png" alt="Preview of The workflow for this process" caption="Image 1:- The workflow for this process">}}


The File2Tiff module examines the extension of the file to be converted and selects the required conversion system:

File2Tiff is then able to utilize the [Aspose.Words for .NET][11] and [Aspose.Cells for .NET][12] libraries to perform the conversion, making use of the Document and Workbook classes respectively, using only a few lines of code:



{{< figure align=center src="images/c2s-case-study-aspose-total-3.png" alt="CodSnippet to determine the file extension" caption="Image 2:- Code snippet to determine the file extension">}}


[Aspose.Words for .NET][13]



{{< figure align=center src="images/c2s-case-study-aspose-total.png" alt="Conversion of MS Word files to other formats" caption="Image 3:- Code snippet for the conversion of MS Word files to other formats">}}


[Aspose.Cells for .NET][14]



{{< figure align=center src="images/c2s-case-study-aspose-total-1.png" alt="Excel to Image conversion code snippet" caption="Image 4:- Conversion of Excel files to Image format">}}


A particularly useful feature of both libraries is the ability to specify image saving options. This allows us to provide the end-user with the flexibility to [specify the resolution][15] at which they wish to save the document, selecting between saving in color or greyscale and choosing particular pages of a document to convert:



{{< figure align=center src="images/c2s-case-study-aspose-total-2.png" alt="Code snippet to convert DOCX to TIFF with customer Resolution " caption="Image 5:- Setting resolution options while converting DOC to TIFF format">}}


### Summary

The [Aspose.Total for .NET][16] package offers significantly more functionality than we have implemented so far. We will continue to enhance the Santiago system further to harness the power of this product, as well as re-visiting the existing modules to ascertain whether they could benefit from the addition of Aspose.




[1]: https://www.c2s.co.uk/
[2]: https://products.aspose.com/total/net
[3]: https://docs.aspose.com/display/wordsnet/Working+with+Graphic+Elements
[4]: https://products.aspose.com/total/net
[5]: https://docs.aspose.com/display/emailnet/Extracting+Message+Contents+from+Emails
[6]: https://docs.aspose.com/display/emailnet/Extracting+Message+Contents+from+Emails#ExtractingMessageContentsfromEmails-ExtractingEmailHeaders
[7]: https://products.aspose.com/total/net
[8]: https://docs.aspose.com/display/cellsnet/Track+Conversion+Progress+of+Excel+to+TIFF
[9]: https://products.aspose.com/total/net
[10]: https://docs.aspose.com/display/emailnet/Working+with+Attachments+and+Embedded+Objects
[11]: https://products.aspose.com/words/net
[12]: https://products.aspose.com/cells/net
[13]: https://products.aspose.com/words/net
[14]: https://products.aspose.com/cells/net
[15]: https://docs.aspose.com/display/wordsnet/Saving+a+Document+as+a+Multipage+TIFF
[16]: https://products.aspose.com/total/net




