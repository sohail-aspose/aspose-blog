---
title: 'memoQ directly imports DOC, XLS, PPTX files to create preview and renders them to other formats  without using Office Interop'
date: Fri, 13 Jan 2012 11:07:00 +0000
draft: false
url: /2012/01/13/directly-import-doc-and-xls-files-and-create-the-preview/
author: Istvan Lengyel
summary: ''
tags: ['Aspose.Total', 'Excel files conversion to PDF using Aspose.Cells for .NET', 'MS Project files creation and manipulation with Aspose.Tasks for .NET', 'MS Word files to PDF conversion using Aspose.Words for .NET', 'MS Word to PDF and PDF to DOC/DOCX conversion using Aspose.Total for .NET', 'PDF to Image conversion using Aspose.PDF for .NET', 'PowerPoint conversion to Image and PDF using Aspose.Slides for .NET', 'Success Stories']
categories: ['Aspose.Total Product Family']
---

## About memoQ



{{< figure align=center src="images/0.png" alt="memoQ logo">}}


[memoQ][1] formerly known as Kilgray Translation Technologies is the fastest growing provider of computer-assisted human translation tools. The company was founded in 2005 in Hungary, and today it has offices in 6 countries. memoQ has revolutionized the way teams work together on translation, allowing several people to work simultaneously on the same set of documents, ensuring maximum translation quality in the shortest turnaround time. memoQ is the most popular server technology among translation companies and increasingly popular among enterprise customers, especially among game developers.

## Problem

Translation tools need to allow translators to translate multiple document types in a single editor. Microsoft Office formats are still very popular, but Kilgray’s flagship product, memoQ also needs to support a myriad of other formats, from Adobe InDesign through DITA to SQL scripts. Kilgray created filters for RTF, DOCX, PPTX, XLSX, and has filters for XLS and PPT using Office Interop, but never created binary filters for DOC, XLS, PPT. The import of these files normally happens through the client software, which automates the locally installed instance of Microsoft Office.

However, users can also use the extensive web services API to integrate their business management tools with memoQ server. In this scenario, Microsoft Office’s licensing prevented Kilgray from being able to use Office Interop to handle the XLS, PPT and DOC formats, and prevented the creation of the real-time preview for translation which is done by Office through saving to HTML. As over 40 companies have integrated memoQ with their internal systems, there was a pressure on the company to come up with a solution to import these file formats without requiring a human to convert them to the Office 2007/2010 OpenXML formats.

## Solution

memoQ is a .NET application, so [Aspose.Total for .NET][2] appeared to be a good solution. Our software processes Microsoft Word, Excel, and PowerPoint files, and buying all components together appeared like a good idea. We have made it optional to replace Microsoft Office in the process, and now memoQ can directly import DOC and XLS files and create the preview, without using Office Interop. This speeds up the import process, especially in the case of Microsoft Excel, and allows computers without Microsoft Office installed to process these binary formats. The user does not see any difference, except for the fact that memoQ works on all computers, also on computers without Microsoft Office installed. This development decreases the number of support requests due to problems with Microsoft Office installations, and allows users not to license Microsoft Office – this is, for example, an extra financial burden for Mac users who use memoQ under virtualization and who need to buy a license for Microsoft Office for Windows even if they have a license for Microsoft Office for Mac.



{{< figure align=center src="images/Kilgray-Translation-Technologies-aspose-total-case-study.png" alt="Translation editor preview" caption="Figure 1: The translation editor and the real-time preview in memoQ.">}}


## Experience

### **Finding a solution**

[Aspose components][3] were recommended to us by two independent experts in translation technology who have already integrated Aspose components with memoQ. We first heard about [Aspose][4] at our user conference. We initially had some concerns about testing Aspose with all the applicable file formats, but the implementation was easier than we thought. This way our product lifecycle manager, who is not a permanent member of the development team, could simply integrate the components – and when he presented it to the management, this came as a surprise.

We used a [free trial for 30 days][5] and requested some extra time before the purchase to test the product with Excel as well. We also turned to [Aspose support][6] with some initial questions and issues, and support was very helpful. At the moment, the [Aspose.Cells for .NET][7] and [Aspose.Words for .NET][8] components are reliable enough to replace Microsoft Office, but we did not find [Aspose.Slides for .NET][9] to be on par with the other two. Support has promised an improvement, and as soon as this component also becomes reliable, we’re going to integrate it.

### **Implementation**

The implementation was surprisingly easy – it required less than a week to integrate the [Aspose components][10] into memoQ. The prototype created was almost the final deliverable, and it did not take up much effort from the development team.

### **Outcome**

With the [Aspose components][11] in place, users of the memoQ web service API and people without Microsoft Office, can also get a preview and import DOC and XLS. This will allow these users to rely completely on memoQ technology and build portals that allow automated quotation and project processing. It will also allow us to cut some dependencies on Microsoft Office and increase user satisfaction.

## Next Steps

The first step was to cut dependency on Microsoft Office. There is however another benefit that we can have through [Aspose’s products][12], and that is the import and export of PDF files for translation. PDF files are a nightmare for translation due to the fact that you need to get them into a format that you can process, such as DOCX. Unfortunately, many translation customers are not ready to send anything but PDF, and in this case, there has been a necessary preparation phase.

Some of our competitors have integrated OCR technology that works with mixed results. We originally integrated a text-only PDF filter, which worked quite reliably but lost the formatting and the output was Text. With two components from Aspose, we planned to [convert a PDF to DOCX][13], and then [convert the translated DOCX back to PDF][14]. We do not expect perfection here, but we expect this to level us up, against the competition. We also believe that translating Microsoft Project files may be interesting in the future, and [Aspose.Tasks for .NET][15] will help there. It is also possible that we can make use of [Aspose components][16] to [handle Microsoft Visio diagrams][17] in translation workflows.

## Summary

[Aspose.Total for .NET][18] allowed us to address the problem of managing three critical filetypes through the API at once. Currently, we have trusted [Aspose.Words for .NET][19] and [Aspose.Cells for .NET][20], we believe that [Aspose.Slides for .NET][21] will soon become powerful enough to address our needs. It was pleasant to work with the [support][22] and sales team at Aspose, and we look forward to integrating more of the Aspose file type components.




[1]: https://www.memoq.com/
[2]: https://products.aspose.com/total/net
[3]: https://products.aspose.com/
[4]: https://www.aspose.com/
[5]: https://downloads.aspose.com/total/net
[6]: https://forum.aspose.com/
[7]: https://products.aspose.com/cells/net
[8]: https://products.aspose.com/words/net
[9]: https://products.aspose.com/slides/net
[10]: https://products.aspose.com/
[11]: https://products.aspose.com/
[12]: https://products.aspose.com/
[13]: https://docs.aspose.com/
[14]: https://docs.aspose.com/display/wordsnet/Convert+a+Document+to+PDF
[15]: https://products.aspose.com/tasks/net
[16]: https://products.aspose.com/
[17]: https://docs.aspose.com/display/diagramnet/Working+with+Diagrams
[18]: https://products.aspose.com/total/net
[19]: https://products.aspose.com/words/net
[20]: https://products.aspose.com/cells/net
[21]: https://products.aspose.com/slides/net
[22]: https://forum.aspose.com/




