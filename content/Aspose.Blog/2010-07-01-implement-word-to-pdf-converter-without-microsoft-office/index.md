---
title: 'Gilde Software Implemented high-performance Word To PDF converter using APIs instead Microsoft Office'
date: Thu, 01 Jul 2010 17:41:00 +0000
draft: false
url: /2010/07/01/implement-word-to-pdf-converter-without-microsoft-office/
author: Andre Stijns
summary: ''
tags: ['.NET API to integrate with SharePoint', 'Aspose.Total', 'Aspose.Words', 'Convert Word documents to PDF format', 'No Office Automation for MS Office files processing', 'Perform Word to PDF conversion without using MS Word', 'Programatically process MS Word files without using MS Office', 'Success Stories', 'Word to PDF conversion without Office Interop']
categories: ['Aspose.Words Product Family', 'Aspose.Total Product Family']
---

## About Gilde Software



{{< figure align=center src="images/Home-logo-1-300x137-1.png" alt="">}}


[Gilde Software][1] consists of several collaborating companies, which focus on achieving efficiency and continuity for its clients. We have more than 25 years of experience in the automation of solutions for project and service companies. The Gilde system is a total solution for project-based and service-providing SMEs. The basic functions of the Gilde system are Relationship management & CRM, Calculation, Project administration & Project monitoring, and Invoicing. 

The functions of the Handsoft Pro Portal at present are:

*   FAQ for users of Handsoft Pro
*   Tips and Tricks for users of Handsoft Pro
*   Process related Manuals for users of Handsoft Pro

At the backend, we use MS Sharepoint to manage our process-related manuals, and at the frontend, an ASP.NET website.

We have used [Aspose.Words for .NET][2] and [Aspose.PDF for .NET][3] to convert the [Word documents from MS Sharepoint into Pdf][4] documents for the frontend ASP.NET website, and this website is integrated with our Handsoft Pro Software.

## Requirements Scenario

*   Any product that can enable us to directly [convert MS Word documents to PDF][5], without MS Office installed
*   It had to perform consistently and well
*   We preferred a .NET component above a COM
*   The component had to be competitively priced to fit in our budget

## Solution Implementation

After trying a couple of different packages, we came upon the [Aspose][6] solution. We found that it works without the need to install MS Office and does everything that we required

From ASP.NET application, first, we check if there is an already converted PDF document and if this is the case, we compare this converted document to the most recent version in SharePoint. If these documents match, then we allow the user to download the converted PDF. If the documents are different, we perform a new conversion based on the most recent SharePoint version and present this to the user instead.

## Benefits

*   A complete package that contains all the developer tools we need now and for future projects.
*   It performs well and does exactly what we ask of it.
*   It’s easy and intuitive to use

## Future Implementations

We intend to develop a resource planning module that will be integrated in our Handsoft Pro Software.

## Conclusion

After we tried a couple of other components, we found that the [Aspose][7] has more than enough tools than we required, but we will certainly be able to use a lot of the functionality in future implementations.



{{< figure align=center src="images/gilde-group-case-study-aspose-words.png" alt="Preview of MS Sharepoint with MS Word files" caption="Image 1:- Screenshot of the backend (MS Sharepoint) with the process related manuals in MS Word.">}}




{{< figure align=center src="images/gilde-group-case-study-aspose-words-1.png" alt="Preview of Frontend Application" caption="Image 2:- Screenshot of the frontend (ASP.Net website integrated into our Handsoft Pro application) with the process related manuals in Pdf.">}}





[1]: https://gildesoftware.nl/
[2]: https://products.aspose.com/words/net
[3]: https://products.aspose.com/pdf/net
[4]: https://docs.aspose.com/display/wordsnet/Converting+a+Word+document+to+PDF
[5]: https://docs.aspose.com/display/wordsnet/Converting+a+Word+document+to+PDF
[6]: https://www.aspose.com/
[7]: https://www.aspose.com/




