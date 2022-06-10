---
title: 'josh Protocol relies on Aspose.Total for .NET for MS Word, Excel, PowerPoint, Image, and TXT to PDF Conversion'
date: Thu, 11 Mar 2010 12:35:25 +0000
draft: false
url: /2010/03/11/convert-documents-to-pdf-format-using-aspose-apis/
author: Nicolino Ambrosini
summary: ''
tags: ['Aspose.Total', 'Convert Excel worksheets to PDF format using Aspose.Cells for .NET', 'Image to PDF and PDF to Image conversion using Aspose.PDF for .NET', 'MS Word DOC/DOCX/RTF conversion to PDF format', 'PDF files generation and Manipulation with Aspose.PDF for .NET', 'PowerPoint conversion to Image and PDF using Aspose.Slides for .NET', 'Success Stories']
categories: ['Aspose.Total Product Family']
---

## About it Consult



{{< figure align=center src="images/1525606_610375058999015_1704635990_n.png" alt="it Consult logo">}}


**[it Consult][1]** is the leading software house in Italy in the Microsoft environment for services and development of software platforms for Organization Intelligence, i.e Business Process, Workflow, Document and Knowledge Management, and in areas like DigitPA standard Computer Procedures, Document Filing, and Substitutive Document Conservation.

We developed a solution named josh Protocol. The main goal of the "josh Protocol!" is to record both letters received and letters dispatched by Italian Public Authorities, to stay within the bounds of the law in force.

All such Authorities receive and send documents in different formats (_i.e.: PDF, TIFF, DOC(x), XLS(x), TXT, RTF…_). One of the components of "josh Protocol!" is a viewer able to manage PDF files. So all the documents are converted to PDF in order to be opened by the Viewer.

“josh Protocol!” is the first system, natively created on the Microsoft infrastructure,which takes full advantage of the Microsoft SharePoint functions; the Viewer allows the negation of specific rights on the single documents, i.e. printing or downloading.

So we have to introduce in our code a module able to convert files to PDF format.

## Requirements Scenario

There are two main requirements to be met:

*   Not to use OLE Automation
*   Conversion server-side from Microsoft Office (legacy) formats to Adobe PDF format

## Solution Implementation

"josh Protocol!" provides a number of tools to record letters. When a user receives (sends) a letter, the tool asks the “josh Protocol!” Service to record it. So “josh Protocol!” Service collects the requests and converts documents to PDF format using the following Aspose products:

*   [Aspose.Words for .NET][2]
*   [Aspose.Cells for .NET][3]
*   [Aspose.Slides for.NET][4]
*   [Aspose.PDF for .NET][5]

## Benefits

The main benefit we gained by using [Aspose][6] is that now we don’t have to use Ole-Automation, a technology not supported by Microsoft. If we ever want to use Ole Automation, we are forced to configure Office in the server machine and this is a bad way to deploy products.

So, by using Aspose, it is now possible to convert documents server-side, instead of client-side. So we have both the opportunity of easier product maintenance and higher reliability.

## Future Implementations

In the future, we may consider using Aspose.Forms for .NET to improve the josh form generation tools, which may be directly used by application domain experts, without the aid of programmers.

## Conclusion

[Aspose libraries][7] are easy to use and meet almost all our needs.



{{< figure align=center src="images/josh-Protocol-aspose-total-case-study-1024x633.png" alt="Josh Protocol preview" caption="Image 1:- josh Protocol preview">}}




{{< figure align=center src="images/josh-Protocol-aspose-total-case-study-1-1024x628.png" alt="" caption="Image 2:- Document processing within josh protocol">}}




{{< figure align=center src="images/josh-Protocol-aspose-total-case-study-2-1024x591.png" alt="Resultant files generated with josh Protocol" caption="Image 3:- Resultant files generated with josh Protocol">}}





[1]: https://www.itconsult.it/en/
[2]: https://products.aspose.com/words/net
[3]: https://products.aspose.com/cells/net
[4]: https://products.aspose.com/slides/net
[5]: https://products.aspose.com/pdf/net
[6]: https://www.aspose.com/
[7]: https://products.aspose.com/




