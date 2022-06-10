---
title: 'Dataforensics Implemented Word, Excel Documents Conversion to PDF along with Watermarks Using Aspose APIs'
date: Mon, 06 Jun 2011 10:52:11 +0000
draft: false
url: /2011/06/16/generate-dynamic-pdf-reports-with-watermarks-using-apis/
author: Scott L 
summary: ''
tags: ['Aspose.Cells', 'Aspose.Words', 'Concatenate PDF documents using Aspose.PDF For .NET', 'Convert DOC files to PDF format using Aspose.Words for .NET', 'Convert Excel files to PDF format', 'Convert MS Word files to PDF format', 'Render DOC/DOCX to PDF format using Aspose.Words for .NET', 'Render Excel files to PDF format using Aspose.Cells for .NET', 'Success Stories']
categories: ['Aspose.Words Product Family', 'Aspose.Cells Product Family']
---

## About Dataforensics



{{< figure align=center src="images/Dataforensics.jpg" alt="Dataforensics company logo">}}


[Dataforensics][1] is a privately owned software company that provides integrated software solutions to improve field data collection, data management, and follow-on analysis for facilities and infrastructure. Client users include engineers, geologists/hydrogeologists, contractors, and infrastructure assessment experts. These individuals work for private design and construction organizations as well as government agencies. They use Dataforensics’ software products to develop, synthesize, and manage extensive amounts of information related to inventory and condition, as well as the characteristics and performance of existing and planned facilities and infrastructure. This data is used to support planning decisions related to design, construction, quality control, vulnerability, damage assessment, and asset management. Dataforensics software products help users save time and resources while improving the quality of the information available for their critical planning and design activities.

## Problem

Dataforeniscs needed an Enterprise capable PDF generation engine. It must be able to convert Word, Excel, and [Open Office documents to PDF][2] documents, combine them, and [create bookmarks][3] for organization within the documents. This is a critical portion of our application to provide the complete workflow that simulates what users today would do manually without our software. This version of the software hasn’t been released to our users yet, but currently, we have two organizations utilizing this particular application with approximately 50 users potentially affected.

## Solution

> **_Dataforensics PQC Application utilizes Aspose to Streamline Workflow_  
> **Scott L. Deaton, Ph.D. – President, Dataforensics LLC

Dataforensics PQC application is the most advanced data management system for construction material testing data. It allows geotechnical engineering consultants and government agencies to have complete control over the field testing and inspection process while having real-time access to the data recorded by technicians in the field. It encompasses the entire business process starting with configuration of the project, defining the related specifications through data collection, reporting, analysis, review, approval, and finally transmittal of the reports to the appropriate people and organizations. It provides a single system that facilitates communication between all involved parties from field technicians to professional engineers to clients to owners and to contractors.

Specifically, the system facilitates recording and reporting construction quality control data related to field density testing, concrete testing, and field reports. Field reports can include a variety of purposes such as daily field reports describing the construction activity or other special inspection reports for structural steel inspection, rebar installation inspection, foundation inspections, concrete placement, or any other report the user wants to define.

Dataforensics system is unique because the field reports module is completely flexible. Companies get the option to use existing Word, Excel, or PDF-based forms for inputting the data while in the field and subsequently load it into the system on the website. The screenshots of this process are shown below. First, the inspector completes their document in Word, Excel, Open Office, or as a PDF form. It can then be loaded directly into the PQC system as shown below where the user indicates critical metadata related to the report being loaded and then attaches the file.



{{< figure align=center src="images/dataforensics-case-study-aspose-words-cells-1.png" alt="Preview of Report load module" caption="Image 1:- Report upload module">}}


Once the report is loaded into the system, a Professional Engineer reviews the reports and approves them. Once the report is approved, no changes can be made to it, except by the original Professional Engineer who approved it. The approval process is shown below, where the first screenshot indicates how the Professional Engineer selects the report by enabling the checkbox under the Approved column and then clicks the Mark Approved button. The second screenshot indicates the result of the approval process, where it indicates who approved the report.



{{< figure align=center src="images/dataforensics-case-study-aspose-words-cells-2.png" alt="Preview of reports in grid" caption="Image 2:- Selection of report from the table grid">}}




{{< figure align=center src="images/dataforensics-case-study-aspose-words-cells-3.png" alt="Details regarding the user who approved the report." caption="Image 3:- Report approved by the reviewer">}}


Once the report is Approved, when a user tries to access the report, it is converted to a PDF document using [Aspose.Words for .NET][4], if the source file is MS Word document or its converted to PDF format using [Aspose.Cells for .NET][5], if the source file is MS Excel format. Furthermore, a watermark is added in the header, indicating who approved the document, their title, and the date it was approved. An example of one of the Aspose converted PDF document is shown here.



{{< figure align=center src="images/dataforensics-case-study-aspose-words-cells-4-769x1024.png" alt="Preview of PDF file generated with Aspose API" caption="Image 4:- Report generated with Aspose component">}}


Additionally, the system includes a Transmittal module that facilitates tracking and sending the appropriate reports to the relevant people and organizations. The transmittal module allows users to set up predefined templates regarding the reporting criteria such as date ranges and other filter criteria, for which PDF documents shall be generated and sent to the appropriate people automatically. It then also serves for tracking and managing the reports that are sent out, making this process significantly more manageable, as compared to previous methods. These Transmittal documents may include density test results or concrete test results generated as a PDF via SQL Server Reporting Services or any of the documents from the field report module. Accordingly, when a Transmittal is generated, the PDF document for density tests and/or concrete tests must be combined with the Word or [Excel documents converted to PDF][6] documents using [Aspose.Words for .NET][7] and [Aspose.Cells for .NET][8] to create a single PDF document that can be emailed. For very large documents, a link to the document can be included in the email as an alternative to attaching the document itself.

## Experience

### Finding a solution

During previous employment, one of our junior developers worked with [Aspose products][9] for document conversion. Our development team then researched the products online and compared the various solutions. Specifically, our requirements were:

*   **[PDF Conversion][10]**: The ability to convert documents (_Word and Excel as well as Open Office documents_) to a PDF.

*   **Enable developers to create unlimited works**. While we were searching for solutions regarding our immediate requirements, we wanted to know that the solution could be integrated into future products. The [Developer OEM license][11] met that criteria.

*   **Microsoft Office shall not be installed on the server**. Some solutions were based on printer drivers where they were "printing" the Office document to a PDF document but required Microsoft Office to be installed on the server. [Aspose provided the standalone solution][12] which did not require MS Office Automation.

The online reviews provided comparisons of Aspose with other products and they seemed to be more positive than other programs, so we downloaded the [free trial][13] of Aspose to test and develop POC. Lastly, Aspose made it easy to work with them. Our development manager was able to obtain a price quote without talking to a salesperson. However, some other companies were not providing a price quote and licensing terms, unless we spoke to a salesperson. Aspose has publicly posted [pricing and licensing terms][14] on their website and made it easy to work with them on the purchase.

### **Implementation**

The implementation of our solution took approximately 1 year. However, the portion of the system that utilized the [Aspose components][15] approximately took 2 months.

After downloading the [Aspose.Words for .NET][16] and [Aspose.Cells for .NET][17] assemblies and after their addition in our ASP.Net application, we found the source code in the [online documentation][18] to [convert a Microsoft Word document to a PDF][19]. It simply took an addition of four simple lines of code to [convert a document from Microsoft Word][20] or [Excel to PDF][21]. In addition to returning [noneditable PDF][22] documents for approved reports, we knew [Aspose][23] would meet the requirements for future user requirements. During the implementation, we didn’t need to utilize [Aspose support][24] as the implementation was so straightforward.

### **Outcome**

Overall, we felt that the utilization of [Aspose.Cells for .NET][25] and [Aspose.Words for .NET][26] components provided a more complete solution that allowed users to perform their entire business process within our application. The development time period was significantly less as compared to using open source components or developing our own conversion tool. [Aspose.Cells for .NET][27] and [Aspose.Words for .NET][28] fit the requirements for our customers to have an easy to use, reliable document conversion and compilation engine.

## Next Steps

The next steps for our product are to roll out the update to our existing customers so that they have a single source, a single-step process for combining the various types of documents, whether Word, Excel, Open Office, or PDF, in the Daily Report document management system.

We are also investigating the possibility of using [Aspose.Cells for .NET][29] for automating reporting for another application that we currently sell as a standalone software application. As part of this new development, we are considering moving it to the software as a service, web-based model so the end-users can simply log in to our website, process their data and generate the necessary reports without having to install any new software on their systems.

## Summary

The integration of [Aspose.Cells for .NET][30] and [Aspose.Words for .NET][31] into our construction quality control data management, document management, and transmittal system, enabled users to configure any type of document/report (_MS Word, Excel or Open Office_) that can then automatically be converted to a PDF and [combined into a single document][32]. This provided significant efficiencies for our clients that enabled them to batch process reports on a weekly/monthly basis, and/or at the end of a project. The usability and stability of [Aspose products][33] have provided confidence to our development team about using the [Aspose components][34] for potential future development and we highly recommend [Aspose products][35] to other development teams. The only issue we have with [Aspose products][36] is that they are slightly expensive for such a small company. However, the discounts they are able to provide for testimonials, case studies, etc, certainly aids with the deployment cost.

Scott L. Deaton, Ph.D.  
President, Dataforensics, LLC




[1]: http://www.dataforensics.net/
[2]: https://docs.aspose.com/display/wordsnet/Converting+a+Word+document+to+PDF
[3]: https://docs.aspose.com/display/pdfnet/Working+with+Bookmarks
[4]: https://products.aspose.com/wordshttps://products.aspose.com/words/net
[5]: https://products.aspose.com/cells/net
[6]: https://docs.aspose.com/display/cellsnet/Convert+Excel+Workbook+to+PDF
[7]: https://products.aspose.com/words/net
[8]: https://products.aspose.com/cells/net
[9]: https://products.aspose.com/
[10]: https://docs.aspose.com/display/wordsnet/Converting+a+Word+document+to+PDF
[11]: https://purchase.aspose.com/pricing/total/net
[12]: https://docs.aspose.com/display/wordsnet/Migration+from+Microsoft+Office+Automation+to+Aspose
[13]: https://downloads.aspose.com/words/net
[14]: https://purchase.aspose.com/pricing
[15]: https://products.aspose.com/
[16]: https://products.aspose.com/words/net
[17]: https://products.aspose.com/cells/net
[18]: https://docs.aspose.com/display/wordsnet/Developer+Guide
[19]: https://docs.aspose.com/display/wordsnet/Converting+a+Word+document+to+PDF
[20]: https://docs.aspose.com/display/wordsnet/Converting+a+Word+document+to+PDF
[21]: https://docs.aspose.com/display/cellsnet/Convert+Excel+Workbook+to+PDF
[22]: https://docs.aspose.com/display/pdfnet/Working+with+Security+and+Signatures
[23]: https://www.aspose.com/
[24]: https://forum.aspose.com/c/words
[25]: https://products.aspose.com/cells/net
[26]: https://products.aspose.com/words/net
[27]: https://products.aspose.com/cells/net
[28]: https://products.aspose.com/words/net
[29]: https://products.aspose.com/cells/net
[30]: https://products.aspose.com/cells/net
[31]: https://products.aspose.com/words/net
[32]: https://docs.aspose.com/
[33]: https://products.aspose.com/
[34]: https://products.aspose.com/
[35]: https://products.aspose.com/
[36]: https://products.aspose.com/




