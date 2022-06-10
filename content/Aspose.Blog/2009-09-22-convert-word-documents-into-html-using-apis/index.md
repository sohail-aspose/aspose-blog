---
title: 'TNTP Implemented MS Word Documents conversion to HTML and PDF format using Apsose APIs'
date: Tue, 22 Sep 2009 07:05:00 +0000
draft: false
url: /2009/09/22/convert-word-documents-into-html-using-apis/
author: Neel Sata
summary: ''
tags: ['.NET API to convert MS Word files to PDF format', '.NET API to render MS Word files to HTML format', 'Aspose.Total', 'DOC and DOCX conversion to HTML format', 'MS Word to PDF conversion APIs', 'OpenOffice document conversion to PDF format', 'OpenOffice to HTML conversion', 'Success Stories']
categories: ['Aspose.Total Product Family']
---

## About The New Teacher Project (TNTP)



{{< figure align=center src="images/59655733_2294473640612916_3166119568418537472_n.png" alt="TNTP logo">}}


[The New Teacher Project (TNTP)][1] is a national non-profit that focuses on recruiting, staffing, certifying, and retaining high-quality teachers into high-needs school districts. In order to better support the school districts we serve, we are building a new platform with Microsoft .NET technologies to allow us to track applicants through our application and selection process. As part of this process, applicants submit documents such as resumes, personal statements, and essays that are used to gauge their eligibility and potential as teachers. Our platform has a wide variety of file conversion needs, and we indent to use the Aspose suite of tools to handle all requirements.

## Requirements Scenario

A number of requirements for TNTP’s new platform technology included uploading, storing, and managing documents. To fulfill this requirement, the Technology team built an Assets Server that allowed us to manage safely and efficiently uploaded by users. A number of requirements also called for the retrieval of these documents in different formats than they were originally submitted. An example is the following user story: "As an admin user, I want to generate applicants’ resumes and applications as a PDF so that they can be sent to selectors as file attachments but cannot be edited."

This story requires the system to retrieve documents originally submitted in [Word and OpenOffice format and render them as PDFs][2]. Other stories required the [conversion of word documents to HTML files][3] (_eg. for display in web browsers for principal access_). The ability to embed documents in our pages allowed us to present an elegant and easy-to-use version of the applicant submitted information.

## Solution Implementation

TNTP will be integrating the [Aspose suites][4] into our .NET based platform. We successfully prototyped this integration with the [evaluation version][5] of the Aspose suite.

Our first implementation of the functionality allowed an admin user to screen information on an applicant, including the applicant’s resume, within a screening page. The resume, which was submitted as one of a variety of word document types, is retrieved in HTML and displayed within the screener’s page.;-



{{< figure align=center src="images/The-New-Teacher-Project-aspose-total-case-study-1024x533.png" alt="Preview of Word file to HTML format" caption="Image 1:- Word file converted to HTML format">}}


As part of a similar feature, an admin user can upload Instructions and have them displayed to users. [Aspose][6] allowed us to accommodate this feature without the costly implementation of a content management system, by converting uploaded Instructions documents into HTML pages:



{{< figure align=center src="images/The-New-Teacher-Project-aspose-total-case-study-1-1024x476.png" alt="Preview of uploaded file" caption="Image 2:- File preview in solution">}}


We also plan to use [Aspose][7] to generate PDF versions of applicant documents to distribute to admin users and principals.



{{< figure align=center src="images/The-New-Teacher-Project-aspose-total-case-study-2.png" alt="Preview of option to generate PDF document" caption="Image 3:- Option to generate PDF document">}}


## Benefits

For TNTP, the benefits are twofold.

*   First, the Technology team dramatically reduces the cost and effort of building a file conversion framework.
*   Second, TNTP will have a scalable product that allows us to quickly review applicant documentation in a variety of formats during our application process.

[Aspose][8] allowed us to create user-friendly versions of frequently used information, as well as helped to maintain the security of documents that shall not be editable by users.

## Future Implementations

No future implementations planned at this time. However, we will be exploring other applications for [Aspose][9] as we build out our Roadmap.

## Conclusion

TNTP is excited to save time and money using the [Aspose product][10] and is thankful for the generosity of the [Aspose][11] organization in offering a discount on their product.




[1]: https://tntp.org/
[2]: https://docs.aspose.com/display/wordsnet/Converting+a+Word+document+to+PDF
[3]: https://docs.aspose.com/display/wordsnet/Converting+a+Document#ConvertingaDocument-ConvertaDocumenttoHTMLwithRoundtripInformation
[4]: https://products.aspose.com/total/net
[5]: https://downloads.aspose.com/total/net
[6]: https://www.aspose.com/
[7]: https://www.aspose.com/
[8]: https://www.aspose.com/
[9]: https://www.aspose.com/
[10]: https://products.aspose.com/
[11]: https://www.aspose.com/




