---
title: 'Sertifi Transformed MS Word, HTML, and various formats to PDF for digital signing over the web'
date: Wed, 26 May 2010 12:58:28 +0000
draft: false
url: /2010/05/26/transforming-various-formats-to-pdf-through-code-using-apis/
author: Joshua Sebor
summary: ''
tags: ['Aspose.Total', 'Convert HTML files to PDF using Aspose.Words for .NET', 'Convert MS Word files PDF format using Aspose.Words for .NET', 'Digitally sign PDF files using Aspose.PDF for .NET', 'Flexible licensing to meet your needs', 'OEM license model', 'Success Stories']
categories: ['Aspose.Total Product Family']
---

## About Sertifi



{{< figure align=center src="images/70743665_830636034036135_6297863189262499840_o.png" alt="Sertifi company logo">}}


[Sertifi][1] is a Software as a Service provider of [electronic signature solutions][2]. Part of our business is dealing with different potential formats of electronic documents submitted by our clients. Thousands of businesses around the world use Sertifi to streamline their contracts and payment processes, recognize revenue faster, and increase job efficiency. We performed a competitive analysis of the best options for this part of our business.

## Requirements Scenario

Sertifi uses PDF as the format for documents within our system. This means that any documents uploaded by clients, not in this format must be transformed. Sertifi required a fast and scalable solution that integrates with our existing codebase with a minimum of development.

## Solution Implementation

Currently, documents must be passed to Adlib (_a separate file-based server_) for transformation. This complicates the document transformation process as documents must be passed to and picked up from the service, resulting in a loss of control over the complete execution flow during the process. The proposed plan was to replace this process with a transformation directly in code using the [Aspose libraries][3].

## Benefits gained by switching to Aspose

The benefits of switching to Aspose included increased reliability, increased performance, increased scalability, and reduced cost.

The requirement of passing documents to Adlib created two potential points of failure, during document pass and document retrieval. Using [Aspose][4] for document transformation enabled Sertifi’s code to keep control of the entire process of transformation. This removed the Adlib points of failure and increases Sertifi’s overall reliability.

Adlib is also a stand-alone server and currently processes all documents sequentially as they are passed in. Some of Sertifi’s clients integrate using web service and upload documents in batch. Between this occurrence and the possibility of heavy usage of Sertifi’s site by clients, the speed of document transformation is a definite concern. Since [Aspose][5] is used as a library, and Sertifi’s solution is inherently multi-threaded, integration of the [Aspose libraries][6] enabled Sertifi to process multiple documents at once. This greatly improved document transformation performance and scalability vs. Adlib.

Lastly, [Aspose’s licensing][7] model is superior to Adlib’s. Adlib is licensed per server while Aspose is licensed per developer. Sertifi maintains a large web server farm, and Adlib’s pricing model does not work well in this case. A second problem was that Sertifi maintains a hot backup system, and under Adlib licensing terms would be required to pay for more Adlib licenses that would almost never be used. Under [Aspose][8]’s licensing terms, hot backup server installations do not require additional licenses.

## Conclusion

Sertifi’s conclusion after careful study of the competing products was that integrating [Aspose libraries][9] for document format transformation would result in reduced costs and increased reliability, scalability, and performance.

Sertifi provides the ability for its customers to quickly and easily send documents to their customers for electronic signature. Using Sertifi customers simply log into the Sertifi web portal, upload the contract they want to send and submit. Sertifi converts formats like word, HTML, and etc to PDF and displays within the Sertifi E-Sign page for signature.



{{< figure align=center src="images/Sertifi-is-a-Software-as-a-Service-aspose-total-case-study.png" alt="Preview of Administrative page" caption="Image 1:- Preview of Administrative page">}}


Sertifi converts formats like word, HTML, and etc to PDF and displays within the Sertifi E-Sign page for signature.



{{< figure align=center src="images/Sertifi-is-a-Software-as-a-Service-aspose-total-case-study-1.png" alt="Digitally sign documents" caption="Image 2:- Digitally sign documents">}}




{{< figure align=center src="images/image.png" alt="">}}


User can indicate where the customer needs to sign by dragging and dropping signature locations.



{{< figure align=center src="images/Sertifi-is-a-Software-as-a-Service-aspose-total-case-study-2-1-1024x575.png" alt="Preview of Signature drag and drop" caption="Image 3:- Preview of Signature drag and drop">}}


Customers are emailed a link to a signing page to sign and complete documents.



{{< figure align=center src="images/Sertifi-is-a-Software-as-a-Service-aspose-total-case-study-5.png" alt="">}}




{{< figure align=center src="images/Sertifi-is-a-Software-as-a-Service-aspose-total-case-study-3.png" alt="Email link to sign document" caption="Image 4:- Email link to sign the document">}}


Sertifi provides a complete audit trail on all transactions and provides detailed analytics on contracts sent, signed, the average time to close, and others.



{{< figure align=center src="images/Sertifi-is-a-Software-as-a-Service-aspose-total-case-study-4.png" alt="Preview of documents Audit trail" caption="Image 5:- Preview of documents Audit trail">}}





[1]: https://corp.sertifi.com/
[2]: https://products.groupdocs.com/signature
[3]: https://products.aspose.com/
[4]: https://www.aspose.com/
[5]: https://www.aspose.com/
[6]: https://products.aspose.com/
[7]: https://purchase.aspose.com/pricing
[8]: https://www.aspose.com/
[9]: https://products.aspose.com/




