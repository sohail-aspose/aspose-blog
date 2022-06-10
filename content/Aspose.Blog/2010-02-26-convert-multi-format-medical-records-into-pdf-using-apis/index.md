---
title: 'Complia Health implemented Server Side PDF conversion of multi-format medical records including MS Office files using Aspose APIs'
date: Fri, 26 Feb 2010 09:44:00 +0000
draft: false
url: /2010/02/26/convert-multi-format-medical-records-into-pdf-using-apis/
author: Satish Movva
summary: ''
tags: ['Aspose.Total', 'Concatenate PDF files using Aspose.PDF for .NET', 'Convert MS Office files to PDF format', 'Convert MS Office to PDF', 'Convert images to PDF using Aspose.PDF for .NET', 'Fill PDF forms', 'Image to PDF conversion', 'Insert Image or Text watermark in PDF fiels', 'MS Office files conversion to PDF format', 'MS Word conversion to PDF using Aspose.Words for .NET', 'MS Word processing without MS Office Automation', 'PDF concatenation', 'Programatically fill PDF forms using Aspose.PDF for .NET', 'Success Stories', 'Watermark PDF documents using Aspose.PDF for .NET']
categories: ['Aspose.Total Product Family']
---

## About Complia Health



{{< figure align=center src="images/logo-with-tag.png" alt="Complia Health company logo">}}


[Complia Health][1] is a leading provider of technology and expertise for the long-term and post-acute care market. Complia Health is a recent spinoff of a healthcare company in the US.

Complia health has built the premier operations platform for Home health care, hospice, private duty, and supplemental staffing industries. The product encompasses both operational and clinical components of a home care services agency including smartphone access and point of care devices. It’s a full web bases SaaS platform and is a pioneer in the industry. The product encompasses over 6 million lines of code and is 100% Microsoft ASP.NET. The product has been in continuous use since 2004 and is used by over 300 home care services providing agencies in the United States.

The product allows a home care services agency to manage all agency operations including client intake, payer setup, scheduling, billing, payroll, payment posting, and collections. In addition, the product fully supports all clinical functions for Medicare, Medicaid, and commercial insurance for the provision of home healthcare services including assessments, plans of care, medication profiles and interactions analysis, and documentation of nurse visit notes.

The product is used by agency personnel to manage the day to day operations and by physicians to view and manage their parents’ care progress and by nurses to provide the care at the patients’ home.

## Requirements Scenario

We had a requirement to perform a server-side stitch of many clinical records of a patient into a single PDF arranged in chronological order. The clinical records can be composed of PDFs, live data from databases formatted into a PDF form, scanned images Word and Excel documents, electronic faxes in TIFF format, and clinical wound pictures. All the documents had to be converted on the server-side in high performance and reliable manner with no server performance degradation. There should be no requirement to install Microsoft Office or other client-side products on the servers to enable the conversion of Microsoft Office documents, as it typically results in unstable server environments.

## Solution Implementation

Documents are either uploaded or scanned into our system and stored in a Microsoft SQL database as BLOBs. The documents can be in Word, Excel, PowerPoint, JPEG, BMP, PNG, TIFF formats among others.

We previously used a combination of libraries for [stitching PDF documents together][2], [converting images to PDFs][3], and [filling out PDF documents][4] on government-mandated forms. While some worked well for the conversion of image formats we ran into a problem with the conversion of Microsoft Office documents. The library supported the conversion if openoffice.org was installed or the Microsoft Office Libraries were installed on the servers. The use of these client-side tools on the server led to server instability due to memory leaks as well as performance degradation on the servers. Since these were front end servers that also served a large n-tier application, this caused a slowdown of the entire system when one user converted documents.

We used [Aspose.Words for .NET][5] to [convert Word documents to PDF][6]. We implemented the conversion code into our system very quickly and easily.

## Benefits

The product enabled us to use one single component for all of our **PDF conversion** and manipulation needs, including [stitching multiple documents together][7], [barcodes][8], and [watermarking][9]. It’s one product to learn and use seamlessly in Visual Studio.

The [Aspose products][10] are high performance and reliability. It does not require Microsoft Office, OpenOffice or other client type applications to be installed on the server to enable access to Microsoft Office documents and their manipulation. We now have the ability to manipulate Microsoft Office documents and to support new functionality such as [mail merge][11] that we weren’t capable of before. This allowed our users to have greater productivity and they made more efficient use of our system.

In addition, we now expect to be able to run our application on 64-bit server platforms without enabling 32-bit compatibility mode as previous tools we used were restricted to 32-bit mode.

We now have no more issues of memory leakage due to the instantiation of client type applications and libraries on the servers when manipulating Microsoft Office documents on the server-side.

## Future Implementations

We plan to use [Aspose.PDF for .NET][12] for [PDF forms manipulation][13] as well as [document stitching][14] so that we can use one product to do all tasks rather than two products from two different vendors.

We plan to use the rest of the features in the [Aspose.Total for .NET][15] product as they have opened up our horizons in new functionality we can add to our system. This included enabling ad hoc reports for end-users using network programming features for automating submission of files to government agencies, using Flask programming for a service area visualization tool using GIS data, using [Barcode generation and detection][16] for auto-indexing of documents into our built-in document management system.

These new features will substantially increase the value of our system to our users and provide us a competitive edge.

## Conclusion

We are very glad to have found [Aspose][17] as an alternative to using multiple different products from different vendors in our need for document conversion and document manipulation on the server-side in a high-performance large scale n-tier SaaS platform.



{{< figure align=center src="images/ContinuLink-Health-Technologies-aspose-total-case-study-1024x625.png" alt="Form preview for document selection" caption="Figure 1: A page where the user selects all possible documents for a patient.">}}




{{< figure align=center src="images/ContinuLink-Health-Technologies-aspose-total-case-study-1.png" alt="Filled out bill sent to patient" caption="Figure 2: A filled out bill sent to the patient.">}}





[1]: http://www.compliahealth.com/
[2]: https://docs.aspose.com/
[3]: https://docs.aspose.com/
[4]: https://docs.aspose.com/display/pdfnet/Working+with+Forms
[5]: https://products.aspose.com/words/net
[6]: https://docs.aspose.com/display/wordsnet/Converting+a+Word+document+to+PDF
[7]: https://docs.aspose.com/
[8]: https://docs.aspose.com/
[9]: https://docs.aspose.com/display/pdfnet/Working+with+Stamps+and+Watermarks
[10]: https://products.aspose.com/
[11]: https://docs.aspose.com/display/wordsnet/Mail+Merge+and+Reporting
[12]: https://products.aspose.com/pdf/net
[13]: https://docs.aspose.com/display/pdfnet/Working+with+Forms
[14]: https://docs.aspose.com/
[15]: https://products.aspose.com/total/net
[16]: https://docs.aspose.com/
[17]: https://www.aspose.com/




