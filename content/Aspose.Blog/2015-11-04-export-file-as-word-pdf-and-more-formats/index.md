---
title: 'ERANET Supported Word to HTML, PDF, PDF to HTML and more formats from public procurement software using APIs'
date: Wed, 04 Nov 2015 13:36:00 +0000
draft: false
url: /2015/11/04/export-file-as-word-pdf-and-more-formats/
author: Mojmir Pridavok
summary: ''
tags: ['Aspose.Total', 'DOC DOCX conversion to PDF using Aspose.PDF for Java', 'HTML files to MS Word conversion using Aspose.Words for Java', 'HTML to PDF conversion using Aspose.PDF for Java', 'MS Word files conversion to HTML using Aspose.Words for Java', 'Success Stories', 'Work with Outlook items using Aspose.Email for Java']
categories: ['Aspose.Total Product Family']
---

## About INNOVIS, s.r.o.



{{< figure align=center src="images/Screenshot-2020-05-11-at-3.26.18-AM.png" alt="Innovis company logo">}}


[INNOVIS, s.r.o.][1], founded in 2014, is a start-up company formed by researchers co-working at the Faculty of Economics, at the Technical University of Kosice. The company's creation was inspired by the expertise and experience gained within European Framework Programs and other research projects conducted by the company's team. Based on our expertise, our vision is to transfer elements of scientific excellence gained at an international level into various business services to support the organizations' processes management and decision making. Our main domains are public and private procurement, supply chains, electronic marketplaces, standardization, exchange of electronic business documents, analytical and decision support tools, etc.

## Problem

ERANET is an online software for the management of public procurement processes in Slovakia and the Czech Republic developed by INNOVIS. Due to the nature of national legislations in both countries, such software solution becomes even more urgent. The typical comments related to the national legislations are: the law is very complicated, ambiguous, misleading etc. Public procurers become gradually frustrated with the amount of paperwork they have to generate every day and for hundreds of deadlines they need to keep track of. Then it is just a matter of time when they make mistakes filling up compulsory forms and other related documents or missing on deadlines.



{{< figure align=center src="images/About-INNOVIS-aspose-total-case-study-1024x400.png" alt="Main ERANET dashboard with internal schedule function activated" caption="Figure 1: Main ERANET dashboard with internal schedule function activated">}}


ERANET tackles all these obstacles by guiding the procurers through the whole process of public procurement starting from the order definition through the offer placement, automatic evaluation, and contracting. There are more than 50 different documents generated during the process of any order and ERANET supports all of them by automatically generating semi-final documents based on the predefined templates. Every document can be edited online in the CKEditor tool; however, the import/export has always been a painful experience, let alone exporting the documents to the .pdf file.

Since we adopted [Aspose.Total for Java][2], users can easily work around the documents both online and offline – never losing the table, multilevel bullets, or advanced formatting.

## Solution

We used [Aspose][3] as a component on our server. The main task has been conversion of documents, mainly MS Word, HTML, and PDF. There were also some minor cases when we used it to generate PDF files. There were some specific cases in the ERANET software in which users needed to import some of the Word files to the system or vice versa - export file as Word or PDF from the system. Request for action goes to the server where we call [Aspose][4] to do the work and result is returned back to the user browser and downloaded.



{{< figure align=center src="images/About-INNOVIS-aspose-total-case-study-1-1024x388.png" alt="Online text editor inside view" caption="Figure 2: Online text editor inside view">}}


Generally speaking, ERANET uses [Aspose][5] mainly for the following activities:

*   Import of Word files (_public procurement mandatory documents_) into the online text editor (_HTML format_)
*   Export of text generated in the online editor (_HTML format_) to Word files (_public procurement mandatory documents_)
*   Export of text generated in the online editor (_HTML format_) to .pdf files
*   [Transformation of Word files to .pdf][6] files and vice versa
*   [Generation of Outlook events][7] from the internal schedule

## Experience

### **Finding a solution**

Yes, we looked at the other options, but never really tried any. [Aspose trial][8] was convincing enough.

### **Implementation**

There were no big challenges. [Documentation][9] on Apose.com is quite huge but sometimes it's hard to find information (_even with search option)._ Also, we had a problem with some classes in examples, as we cannot find them in API Reference. We also had a problem with our national symbols (_diacritic_), but we sent the questions to [support][10] and after a couple of days, we get an answer (_as Forum topic_).

Currently, it is not fully implemented, but it took only two days (_counting only programmer work, not research for finding the right component_).

### **Outcome**

Implementation of [Aspose][11] had not affected our team since the whole process took just two days. On the other hand, just after the [Aspose][12] was implemented, we have realized great savings while processing customers’ requests for document templates changes.

## Next Steps

We have adopted the [Aspose.Total for Java][13] and so we do not have any short term objectives to adopt more of [Aspose][14] software. However, we are very much interested in testing the following functionalities in the future:

*   [Generation of QR codes][15] carrying the information about the concrete public procurement call – this will be used within the mobile application for the interested applicants/suppliers
*   [Spreadsheet editing and conversion][16] (_price calculation)_ into the ERANET database
*   [PDF file conversions to HTML][17] or plain text format, in order to be able to edit this file and [HTML to PDF conversion][18].

## Summary

Generally speaking, [Aspose][19] is pretty expensive software but the rich functionality is really worth it. Since we are a start-up company, it was pretty difficult to splash thousands of euros for a license, but now we consider it as one of the best decisions we made in the technical area. Well done!




[1]: http://www.innovis.sk/en/
[2]: https://products.aspose.com/total/java
[3]: https://www.aspose.com/
[4]: https://www.aspose.com/
[5]: https://www.aspose.com/
[6]: https://docs.aspose.com/display/wordsjava/Specify+Rendering+Options+When+Converting+to+PDF
[7]: https://docs.aspose.com/display/emailjava/Working+with+Outlook+Items
[8]: https://downloads.aspose.com/total/java
[9]: https://docs.aspose.com/dashboard.action
[10]: https://forum.aspose.com/
[11]: https://www.aspose.com/
[12]: https://www.aspose.com/
[13]: https://products.aspose.com/total/java
[14]: https://www.aspose.com/
[15]: https://docs.aspose.com/display/barcodejava/Generate+Barcodes
[16]: https://docs.aspose.com/display/cellsjava/Developer+Guide
[17]: https://docs.aspose.com/display/pdfjava/Convert+PDF+to+HTML+format
[18]: https://docs.aspose.com/display/pdfjava/Convert+HTML+to+PDF
[19]: https://www.aspose.com/




