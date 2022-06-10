---
title: 'BoardPro created a solution for PDF Concatenation, Header and Footer stamping, Annotation and Bookmarking using Aspose.PDF for .NET'
date: Mon, 11 Dec 2017 04:34:05 +0000
draft: false
url: /2017/12/11/board-pack-to-convert-different-documents-to-pdf-using-apis/
author: Zeeshan Bhatti
summary: ''
tags: ['Add Navigational Annotations in PDF using Aspose.PDF for .NET', 'Aspose.PDF', 'Concatenate PDF documents using Aspose.PDF For .NET', 'Convert .DOC to PDF using GroupDocs.Conversion', 'Convert .PPT to PDF using GroupDocs.Conversion', 'Convert .TXT to PDF using Aspose.PDF for .NET', 'Convert Image to PDF using GroupDocs.Conversion', 'Insert Bookmarks in PDF using Aspose.PDF for .NET', 'Insert Header and Footer in PDF using Aspose.PDF for .NET', 'Success Stories']
categories: ['Aspose.PDF Product Family']
---

## About BoardPro



{{< figure align=center src="images/87546861_2448313298607886_1262047157490286592_n.png" alt="">}}


[BoardPro][1] is an innovative cloud-based startup developing board management software specifically designed to meet the requirements and governance workflows of the board of directors of small to medium businesses and non-profits.

It is an easy-to-use software for board meetings, responsibilities, and documents, and it is designed specifically to meet the challenges of limited resources and limited experience.

Professional corporate boards can afford extensive governance and administration resources, freeing directors to focus on making a powerful contribution. However, many SME’s and non-profit organizations lack these dedicated resources, meaning they often run less effectively, despite the quality of their directors.

BoardPro has taken best practices from corporate boards and simplified and automated them for SME and non-profit boards. Today, still in its early days, BoardPro is used by over 200 boards and in the first 10 months, has hosted over 1000 meetings and converted more than 31,000 documents.

## Problem

One of the core features of BoardPro is the production of the meeting “Board Pack” – all the reports and papers for each meeting compiled from a variety of user-uploaded files into a single PDF.

The executives of the organization were able to go into BoardPro, find the scheduled meeting, and attach their monthly reports, special papers to the specific agenda items they relate to. The reports had an option to be uploaded in a wide variety of formats - .pdf, .doc, .docx, .ppt, .pptx, .rtf, .txt, .jpg, etc. Each file was then converted to PDF and then merged into a single PDF in the correct order, with an internally linked Index and Agenda file.

The Board Pack was then distributed to the board members, who were preparing for the board meeting from this single file. No longer were board members receiving multiple documents attached to an email, where they were left wondering which document was related to which agenda item, etc.

## Solution - Document Conversion

Before we started using [Aspose.PDF for.NET][2], we had an experience of using [GroupDocs.Conversion][3] to convert documents of various types into PDF format. We found [GroupDocs.Conversion][4] to be much superior to the alternative we had been using. We concluded that there have been great benefits of scalability and reliability achieved when switched over to [GroupDocs.Conversion][5] from a competitor product.

## Our Initial Implementation

In order to create the Board Pack solution, BoardPro needed a .NET solution for [merging the converted PDF files][6] into a single PDF file and to provide additional navigation aids. These navigation aids shall enable the readers to easily navigate between agenda items and review the supporting attached documents i.e., the following.

*   A cover page to indicate the meeting title, date, time and location.
*   An index page (table of contents) that utilized PDF page navigation to jump to the right page.
*   Navigation annotation overlay on the agenda PDF that linked the corresponding agenda item with its attached support documents.
*   Header and footer stamps for organization branding and meeting title.
*   Bookmarks for quick navigation to agenda documents



{{< figure align=center src="images/BoardPro-aspose-pdf-case-study.png" alt="A Preview of Index and Agenda" caption="An example Board Pack cover page, index, and agenda (thumbnail view)<br>">}}


### **Reliability Issues with the Competitor Product**

The earlier implementation of merging documents and generating Board Pack navigation aids utilized SyncFusion, a set of libraries for editing and merging PDF files. During the feature implementation phase, we had to constantly work around issues image and text transparency and inconsistency of behavior. Even more, issues were discovered when the implementation was released to our users. Some of the issues we struggled with are described as follows.

*   Some PDF files that were uploaded by customers, failed to open by SyncFusion and therefore had to be skipped from the Board Pack. This caused dissatisfaction to our customers.
*   In one instance, a PDF document that was digitally signed, could not be processed in the phase where we applied custom headers and footers. We obviously didn’t expect the digital signature to be retained, but skipping the document from the merge process altogether was unacceptable.
*   Over the months, our SyncFusion based implementation failed at either of the following steps
    *   Document conversion phase,
    *   PDF merging phase,
    *   Application of headers and footers, or
    *   Creation of the index page.

In all of the above errors, there wasn’t a clear explanation of what went wrong and our support team had to resort to workarounds that were less than ideal e.g., converting PDF documents to PNG images and then converting back to PDF. With so many points of failures and no clear understanding of how to ensure the reliability of our Board Pack feature, we decided to find an alternative.

## Experience

### **Benefits gained by switching to Aspose.PDF** for .NET

Previously BoardPro had been using SyncFusion for generating Board Pack PDFs, which involved converting the user uploaded documents into PDFs and combining them together. This process, as discussed above, was riddled with bugs and reliability issues. After spending countless hours in customer support, we decided to start looking for alternatives.

Our search led us to discover [Aspose.PDF for .NET][7]. We evaluated Aspose.PDF for both scalability and reliability before making the final decision to switch from SyncFusion. In both our evaluation and later implementation to replace SyncFusion, we have found Aspose.PDF to be a winner.

Having switched to [Aspose.PDF for .NET][8], we haven't encountered a single instance where the document conversion failed. In the past, we had kept anonymized versions of the customer PDF documents that failed to open or merge using SyncFusion, and were pleased to find that all of those documents were processed flawlessly with [Aspose.PDF for .NET][9].



{{< figure align=center src="images/BoardPro-aspose-pdf-case-study-1.png" alt="A PDF merge preview" caption="An example of merging PDF files of varying rotation and page layout along-with custom headers and footers (thumbnail view)">}}


## Next Steps

BoardPro is continually offering new services to boards of SME’s and Non-profit organizations. We have plans to digital signatures, custom document templates and to offer a wider range of supporting documents to be attached. We are convinced that all of this will be possible using the range of products offered by [GroupDocs][10] and [Aspose][11].

## Summary

BoardPro no longer uses its original solution for [merging and editing PDF][12] files for building the Board Pack - this has been completely replaced using [Aspose.PDF for .NET][13].

[PDF merging feature][14] was very easy to implement using [Aspose.PDF for .NET][15], the coordinate system for custom [placement of text][16] and [annotations][17] took a little longer but we are getting used to it. Overall, [Aspose.PDF for .NET][18] was an elegant solution for our requirements at BoardPro. It has allowed us to offer higher reliability to our customers. We found [Aspose.PDF for .NET][19] to be more stable than our previous solution.

The [documentation][20] and [support forums][21] were very helpful in supporting our implementation. Overall, BoardPro has been very impressed with the product and support offered.

**Zeeshan Bhatti**, BoardPro CTO  
[BoardPro Limited][22]




[1]: https://www.boardprohub.com/
[2]: https://products.aspose.com/pdf/net
[3]: https://products.groupdocs.com/conversion/net
[4]: https://products.groupdocs.com/conversion/net
[5]: https://products.groupdocs.com/conversion
[6]: https://docs.aspose.com/
[7]: https://products.aspose.com/pdf/net
[8]: https://products.aspose.com/pdf/net
[9]: https://products.aspose.com/pdf/net
[10]: https://www.groupdocs.com/
[11]: https://www.aspose.com/
[12]: https://docs.aspose.com/
[13]: https://products.aspose.com/pdf/net
[14]: https://docs.aspose.com/
[15]: https://products.aspose.com/pdf/net
[16]: https://docs.aspose.com/display/pdfnet/Replace+Text+in+a+PDF+Document
[17]: https://docs.aspose.com/display/pdfnet/Working+with+Annotations
[18]: https://products.aspose.com/pdf/net
[19]: https://products.aspose.com/pdf/net
[20]: https://docs.aspose.com/display/pdfnet/Home
[21]: https://forum.aspose.com/c/pdf
[22]: https://www.boardprohub.com/




