---
title: 'Connectrex implemented Digital Sign feature using proprietary System key for legal PDF documents using Aspose.PDF for .NET'
date: Wed, 17 Dec 2008 13:49:28 +0000
draft: false
url: /2008/12/17/apis-to-lock-and-sign-the-pdf-files/
author: Paul Allaire
summary: ''
tags: ['Aspose.PDF', 'Aspose.Words', 'Convert .doc files to .docx format', 'Manipulate PDF files using Aspose.PDF for .NET', 'Restrict user permissions on PDF files using Aspose.PDF for .NET', 'Set access privileges on PDF files using Aspose.PDF for .NET', 'Sign PDF documents using Aspose.PDF for .NET', 'Success Stories', 'digitally sign PDF documents']
categories: ['Aspose.Words Product Family', 'Aspose.Total Product Family', 'Aspose.PDF Product Family']
---

## About connectrex



{{< figure align=center src="images/Connectrex_Logo.png" alt="connectrex logo">}}


**[connectrex][1]** is a leading provider of community corrections software and a strategic consulting partner to progressive government agencies nationwide.  We are unique!  We are special!  No other company can claim our experience, talents or capabilities.  Blending award-winning software with leading community corrections staff **connectrex** has truly delivered on the vision of software that makes a difference. 

## Monitor

An enterprise-class criminal justice client management system, Monitor provides a single, state-of-the-art, integrated database solution that meets all of the investigation, supervision, institutions, document management, financial accounting, reporting, and management needs of the community corrections agencies for both adult and juvenile offenders. Our advanced roles-based security system allows clients to set permissions for individuals and groups of users that determine exactly what functions and records each person can view and modify.

Data can only be entered once in Monitor and after that, it becomes available to all users based on their security permissions. Our application design allows instant access to information and our system of management reporting, alerts, and ticklers/messaging facilitate accurate and well-informed decision making. This results in increased efficiency, communication, and agency effectiveness.

Monitor facilitates extensive data collection with a user-friendly interface, which is configurable to meet the needs of local jurisdictions, and generates the forms, reports, and statistics required by best practices for criminal justice agencies, including adult and juvenile probation departments.

Monitor meets the performance-based management and functional standards for management information systems developed by the American Probation and Parole Association (APPA), as well as national pretrial, institutions, and drug court standards.

## Requirements Scenario

Generation of the legally viable documents in locked PDF format using a set of tools adopted by our industry. The electronic signatures were only supported in Word documents.

## Solution Implementation

We implemented both [Aspose.Words for .NET][2] and [Aspose.PDF for .NET][3] APIs in Document Management subsystem of our product. This system executed as a windows service and prior to this implementation, we utilized a printer driver to produce an unsigned PDF for use as a legal document. However, with a new implementation, it started to accept an upload from a Word add-in into a WCF service. The service was then able to accept MemoryStream object, convert it into a PDF document and digitally sign it using a proprietary system key. It was then written to a document store.

The service also returned a document upon request. The individual users usually have different versions of MS Word installed, so depending upon user settings, whenever the user loaded a word document to be edited, we used the word functionality to convert the template into the appropriate Word format (.doc/.dot/.docx).

## Benefits

We realized several benefits by implementing [Aspose.Words for .NET][4] and [Aspose.PDF for .NET][5] APIs provided by [ASPOSE][6]. The initial benefit was a reduction in licensing fees as MS Office was no longer needed to be installed on each provided server. In addition to those immediate savings, we saw an additional benefit of being able to [programmatically lock and sign the PDF documents][7], and since the PDF was implemented programmatically within a service instead of a print driver, an overhead of having multiple accounts on servers to accept the printer writing for them was instead turned to a single domain account with permissions on various machines.

## Future Implementations

We plan to continue to use [ASPOSE APIs][8] as part of an ongoing development effort of [converting .doc files into .docx files][9] and then using the Linq to XML features in the .NET 3.5 platforms to modify key fields on the server, before pushing the item down to a client machine.

## Conclusion

We’ve had a great experience using [ASPOSE products][10]. They function smoothly and the documentation is excellent as well as easy to follow and understand. The initial development effort and proof of concept were done in days as compared to our experiences with other vendors which used to take several weeks to produce a viable prototype.



{{< figure align=center src="images/loryx-systems-aspose-pdf-case-study.png" alt="Preview of Form to input word document" caption="<br>Image 1:- This form is used to grab the word document that will later be signed.">}}




{{< figure align=center src="images/loryx-systems-aspose-pdf-case-study-1.png" alt="Document preview" caption="Image 2:- Document preview">}}




{{< figure align=center src="images/loryx-systems-aspose-pdf-case-study-2.png" alt="">}}


The signature tool was then able to import the signature which was then published as a signed PDF document



{{< figure align=center src="images/loryx-systems-aspose-pdf-case-study-3.png" alt="Preview of Signed documents">}}


The documents were then saved and made available as legally signed documents inside the Monitor.Net system.

**Paul Allaire  
**connectrex




[1]: https://www.connectrex.com/
[2]: https://products.aspose.com/words/net
[3]: https://products.aspose.com/pdf/net
[4]: https://products.aspose.com/words/net
[5]: https://products.aspose.com/pdf/net
[6]: https://www.aspose.com/
[7]: https://docs.aspose.com/display/pdfnet/Working+with+Security+and+Signatures
[8]: https://www.aspose.com/
[9]: https://docs.aspose.com/display/wordsnet/Loading%2C+Saving+and+Converting
[10]: https://products.aspose.com/




