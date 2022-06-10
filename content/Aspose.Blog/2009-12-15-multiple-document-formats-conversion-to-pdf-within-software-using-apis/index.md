---
title: 'QJumpers Supports multiple Document Formats conversion to PDF within Software using APIs'
date: Tue, 15 Dec 2009 06:58:00 +0000
draft: false
url: /2009/12/15/multiple-document-formats-conversion-to-pdf-within-software-using-apis/
author: Justin Moore
summary: ''
tags: ['.NET API to manipulate MS Word files', '30 days free trial of MS Word document processing', 'Aspose.Words', 'Convert MS Word files to PDF format', 'Create', 'DOC/DOCX/RTF to PDF rendering', 'MS Word documents processing', 'MS Word to HTML conversion', 'MS Word to PDF conversion', 'Quick Technical Support', 'Success Stories', 'Update and Render MS Word files to various supported formats']
categories: ['Aspose.Words Product Family']
---

## About QJumpers



{{< figure align=center src="images/logo-4.png" alt="QJumpers company logo">}}


[QJumpers][1] is an innovative online provider of recruitment services. The business was formed to help employers recruit a lot easier without having to pay the fees of a typical recruitment company. Our services provide a helping hand in the recruitment process without taking control of the employer.

Our base service, Applicant Sourcing, includes advertising on the top jobsites as well as the use of our Applicant Tracking System (ATS) to help manage the communication and the recruitment process. Incoming job applications are managed using QJumpers ATS where employers can view resumes, cover letters, psychometric profiles, contact candidates and shortlist or dismiss applicants. As part of the Applicant Sourcing service, we also provide over-the-phone recruitment advice and field any initial inquiries from applicants.

Depending on the client’s workload, number of applicants and specific need, QJumpers can manage more of the recruitment process if required. Our pricing for different service levels is clear, and no commission fees are paid by the employer.

QJumpers maintains a Talent Pool of candidates which employers can search. This enables employers to find potential candidates without the extra cost of advertising on job boards, and on the flip side allows candidates to be contacted for job opportunities that fit their skills and qualifications without actively applying for roles.

Today, QJumpers has been used by over 2000 employers and more than 30,000 candidates have joined the talent pool.

## Requirements Scenario

As part of the QJumpers recruitment service, jobs are advertised on several leading job boards. Candidates can apply directly from the advertisement and the application is received by QJumpers via email. Candidates can also apply for a job directly on the [QJumpers site][2]. Candidates may attach their resume and a cover letter to their job application. QJumpers has no control over the format of these files and must handle a variety of formats including Rich Text Format (rtf), Text (txt), Word (doc), Microsoft OpenOffice XML Format (docx), Microsoft Works (wps), HyperText Markup Language (html), Portable Document Format (pdf) and OpenDocument Text (odt).

Employers may not have the required client applications installed to open the various document formats submitted by candidates. Employers may also be reluctant to open some file formats and in some cases, unable to download files for security reasons.

QJumpers’ applicant tracking system must accept the various file formats submitted by candidates and convert them to a format acceptable and widely viewable by employers.

Candidate documents must be searchable to enable employers to search QJumpers’ Talent Pool for candidates matching the employer’s requirements.

## Solution Implementation

QJumpers applicant tracking system accepts candidate documents in any format and presents the documents to employers in PDF format. Documents are stored in their original format in a SQL Server database with SQL Server Full-Text Search indexing to enable searching of documents.

Documents are then [converted to PDF format][3] for presentation using [Aspose.Words for .NET][4]. Documents are also available in their original format for the convenience of the document owner.

Unfortunately, not all files received by QJumpers are automatically converted. Pre-Word 97 documents and Microsoft Works (WPS) format files are currently not supported by [Aspose.Words for .NET][5] and currently, QJumpers manually converts these documents.

Documents are presented in close fidelity to the original document, exceptions being that borders are removed and if a font is used in the document, that is not installed on the server then it is replaced.

## Benefits gained by switching to Aspose

Previously QJumpers had been using a component for populating PDF templates with candidate data for generic resumes. As we were already using that product, we implemented a solution using the same product to generate output in various formats, such as PDF.

This involved installing OpenOffice on the webserver and using Component Services COM+ Automation to open and convert documents.

This was difficult to implement and involved messing around with security permissions to launch OpenOffice from ASP.NET using a DCOM+ Component Services. The system had stability problems. Some problematic documents caused OpenOffice to hang and the website to become unresponsive.

[Aspose.Words for .NET][6] was very easy to implement. Support on the [Aspose forums][7] has been helpful with issues fixed promptly.

[Aspose.Words for .NET][8] removed our dependence on Component Services and Automation of OpenOffice. We no longer have the problems that occurred when we automated a client application from ASP.NET. Our system is stable, faster and more secure using [Aspose.Words for .NET][9] as compared to previous solutions when we used OpenOffice and Component Services.

## Future Implementations

QJumpers is continually offering new services to employers and candidates and will be using [Aspose.Words for .NET][10] to implement document related functionality. As per current development plans, we are focused on the ability for employers to attach job descriptions, custom application forms, and additional documents to a job listing.

QJumpers still uses its original solution for populating PDFs with candidate data. This will be redeveloped using [Aspose.Words for .NET][11] in the near future.

The need for manual intervention to convert pre-Word 97 and Microsoft Works documents is something that QJumpers would like to address. We hope [Aspose.Words for .NET][12] will add support for pre-Word 97 and Microsoft Works (wps) documents.

QJumpers is also investigating the usage of [Aspose.Words for .NET][13] as part of a reporting solution.

## Conclusion

[Aspose.Words for .NET][14] was easy to implement and an elegant solution for our requirements at QJumpers. We found [Aspose.Words for .NET][15] faster, more stable, and more effective at converting documents than our previous solution.

The usage of [Aspose.Words for .NET][16] removed a somewhat unstable dependency on Component Services Automation of OpenOffice.

The fidelity of documents is very good. The main benefit is that employers are able to view the content of a candidate's CV. For our requirements, it does not matter if aesthetic components like borders and fonts are preserved.

[Aspose support forums][17] have been quick to respond and very helpful. QJumpers have been very impressed with the product and support offered. We wish we had found [Aspose][18] sooner.




[1]: https://www.qjumpers.co.nz/employer/home/
[2]: http://www.qjumpers.co.nz
[3]: https://docs.aspose.com/display/wordsnet/Converting+a+Word+document+to+PDF
[4]: https://products.aspose.com/words/net
[5]: https://products.aspose.com/words/net
[6]: https://products.aspose.com/words/net
[7]: https://forum.aspose.com/c/words
[8]: https://products.aspose.com/words/net
[9]: https://products.aspose.com/words/net
[10]: https://products.aspose.com/words/net
[11]: https://products.aspose.com/words/net
[12]: https://products.aspose.com/words/net
[13]: https://products.aspose.com/words/net
[14]: https://products.aspose.com/words/net
[15]: https://products.aspose.com/words/net
[16]: https://products.aspose.com/words/net
[17]: https://forum.aspose.com/c/words
[18]: https://www.aspose.com/




