---
title: 'Public Procurement Authority Generated Printable Reports for its Annual Assessment of Public Entities using APIs'
date: Wed, 28 Aug 2013 07:13:48 +0000
draft: false
url: /2013/08/28/generate-printable-reports-for-its-annual-assessment-of-public-entities/
author: John K Wilson
summary: ''
tags: ['A better alternative to BIRT', 'A competing alternative to docx4java', 'Aspose.Words', 'Java API to convert Word document to PDF format', 'Java API to programatically process MS Word document', 'Java API to replace iText', 'MailMerge in MS Word Document', 'Render MS Word file to PDF format', 'Success Stories']
categories: ['Aspose.Words Product Family']
---

## About Infinite Blue Technologies



{{< figure align=center src="images/logo.jpg" alt="">}}


Infinite Blue Technologies is a group of consultants providing bespoke software solutions for both the public and private sectors. Infinite Blue Technologies has worked on the [Public Procurement Model of Excellence][1] (PPME) tool which is used to collect data and assess the level of compliance and performance of public entities. The annual exercise culminates with the production of online reports for the individual entities to peruse and implement whatever recommendations included.

## Problem

Although reports are available online, entities are also issued official paper copies that are signed and stamped, for archiving purposes. The assessment agency already had a Microsoft Word document format, which was used when reports were manually produced and therefore, wanted the tool to produce similarly-formatted reports.



{{< figure align=center src="images/infinite-blue-case-study-aspose-words.png" alt="Preview of Assessment questionnaire" caption="Image 1:- Assessment questionnaire">}}




{{< figure align=center src="images/infinite-blue-case-study-aspose-words-1.png" alt="Preview of Assessment report" caption="Image 2:- Assessment report">}}


## Solution

After evaluating existing reporting tools such as BIRT, Jasper Reports, iText, and docx4java, we came to the conclusion that we need a solution that enables a finer control over document formatting, as well as requires shorter development time. This led us to evaluate and then we chose the solutions/products offered by [Aspose][2].

We initially decided to create a pdf template of the existing Word document. The rationale being that PDF readers are ubiquitous and documents are read-only. We had a perspective that this would allow reports to be reviewed by other stakeholders before printout. At the same time, we also realized that it would be much easier to use the existing MS Word template and create merge fields to produce a final document using [Aspose.Words for Java][3] with mail merge.

Being able to create the template in Word format was a gratifying experience for the development team because it allowed us to produce a document with which we were satisfied before sending it to [Aspose.Words for Java][4] to “fill-in the spaces”.



{{< figure align=center src="images/infinite-blue-case-study-aspose-words-2.png" alt="Preview of Word template with merge fields" caption="Image 3:- Word template with merge fields">}}




{{< figure align=center src="images/infinite-blue-case-study-aspose-words-3.png" alt="Preview of document with chart information" caption="Image 4:- Sample output">}}


Our application workflow ended up being as follows:

*   Retrieve XML data from a repository
*   Compute and render charts
*   Format rest of data for Aspose Words
*   Render the final document with Aspose Words

The fully functional [trial version][5] of the product was a godsend because it enabled us to write our test code and evaluate the output before committing to a purchase.

## Experience

We had a fairly smooth application development period due to the good [documentation][6] and [uncomplicated API][7].

We discovered that most of our code involved formatting the data from the repository before passing it to [Aspose.Words for Java][8] for "[MailMerge][9]". The actual rendering code was just a minute fraction of the overall application code.  
An initial challenge was including images of graphs in the word document but after reading the [online documentation][10], we managed to overcome that with a simple "event handler" and "<>" fields.

We also had a few tables to generate but that was also done effortlessly and the results were very satisfactory.



{{< figure align=center src="images/infinite-blue-case-study-aspose-words-4.png" alt="Sample Image handling code preview" caption="Image 5:- Sample image handling code">}}


## Next Steps

We look forward to using other [products Aspose][11] offers in our future projects and don’t have any reservations recommending their solutions to other developers.

## Summary

[Aspose.Words for Java][12] has been an excellent discovery for us and has enabled us to create a complete and well-integrated product. The simplicity of the tool coupled with its [good documentation][13] considerably reduced the effort and time to test and deliver a solution that met our client's requirements.

**John K Wilson**, CTO  
Infinite Blue Technologies




[1]: https://ppa.gov.gh/
[2]: https://www.aspose.com/
[3]: https://products.aspose.com/words/java
[4]: https://products.aspose.com/words/java
[5]: https://downloads.aspose.com/words/java
[6]: https://docs.aspose.com/display/wordsjava/Developer+Guide
[7]: https://apireference.aspose.com/words/java
[8]: https://products.aspose.com/words/java
[9]: https://docs.aspose.com/display/wordsjava/Mail+Merge+and+Reporting
[10]: https://docs.aspose.com/display/wordsjava/Developer+Guide
[11]: https://products.aspose.com/
[12]: https://products.aspose.com/words/java
[13]: https://docs.aspose.com/display/wordsjava/Developer+Guide




