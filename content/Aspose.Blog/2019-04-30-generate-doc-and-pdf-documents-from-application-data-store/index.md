---
title: 'Commugen Programmatically Generated MS Word files based on Dataset and Rendered output to PDF'
date: Tue, 30 Apr 2019 16:30:28 +0000
draft: false
url: /2019/04/30/generate-doc-and-pdf-documents-from-application-data-store/
author: Vladimir Tyomin
summary: ''
tags: ['.NET API to convert MS Word files to PDF', 'Aspose.Words', 'Convert Word files to PDF using Aspose.Words for .NET', 'DOC to PDF conversion', 'Dynamically generate MS Word files based on dataset.', 'Parse Excel worksheet content using Aspose.Cells for .NET', 'Read Email file content using Aspose.Email for .NET', 'Success Stories']
categories: ['Aspose.Words Product Family']
---

## About Commugen



{{< figure align=center src="images/logo-1.png" alt="">}}


[Commugen][1] is a software company that developed a platform that enables non-programmers to build web-based applications.

Solutions based on the platform serve leading Israeli companies, mainly in the financial and government sectors. They include solutions for e.g. governance, risk management, and compliance.

## Problem

Commugen developed an ASP.NET web application where we enabled modeling data structures and relationships between structures. After modeling, the application generates an input interface that enables the gathering of data throughout the organization. The data is then displayed for analysis and task generation in reports and dashboards. Most of our customers required to export the data from these reports & dashboards to a Word or a PDF document.

Commugen is an Israeli based company, so there was also a mandatory need for good multi-lingual support, including Right-To-Left texts.

We thought to go to the source, Microsoft as a good idea. Therefore, we implemented a Word generation mechanism using MS Word on the server. Then we used MS Word automation to generate the DOC and PDF files.

However, this mechanism had significant stability problems. It could not work in production for a significant amount of time without breaking and needing a human intervention for restart.

## Solution

We searched for an alternative to Word automation. We read about [Aspose][2], and looked at the website. We were happy to see that [Word manipulation][3] was just a part of the Aspose offering. Since we have been receiving new customer demands all the time, we thought that a product that is expandable to solving other problems would be the right fit for us.

We tried working with the [trial version][4] of the library and we found it was straightforward to incorporate it into our .Net code. Commugen managed to generate DOC and PDF documents from its application data store using [Aspose.Words for .NET][5]. It worked perfectly for us, as well as for our customers, as it merged the customer's templates with the application content to create a document. The solution became stable and it worked pretty fast. In all contexts, Aspose.Words for .NET generated the desired documents as we expected.

Figures 1 & 2 below show an example of [Aspose.Words][6] usage in a Commugen application.



{{< figure align=center src="images/commugen-case-study-aspose-words.png" alt="Image of supply chain Risk management Application" caption="Image 1:- A Supply Chain Risk Management application, which generates a report, as a final stage after risk assessment.">}}




{{< figure align=center src="images/commugen-case-study-aspose-words-1-1024x501.png" alt="" caption="Image 2:- A sample of the generated PDF report from the Supply Chain Risk Management solution above.">}}


## Experience

Commugen’s applications manage data. Sometimes the data needs to be moved "offline" e.g. to people who do not have access to the application. Therefore, it was required to be exported and distributed in different formats and contexts, such as MS Word and PDF.

[Aspose.Words for .NET][7] does not require online authentication or processing. Therefore, it was an appropriate choice for our customers who mainly required to use it in an on-premise configuration. For our customers, it appeared as a seamless experience, integrated into our solution. All in all, [Aspose.Words for .NET][8] proved to be easy to try, buy, install and use.

## Next Steps

We are very satisfied with [Aspose.Words for .NET][9] so we plan to expand the use of [Aspose solutions][10] to other problems we encounter.

We have also examined the [Aspose.Email solution][11] as we need to [read and parse e-mail][12] and get save them into our application data store. We found that getting attachments from e-mails was particularly difficult to accomplish, but when we tried the [Aspose.Email for .NET][13] component, it handled it flawlessly.

We also thought to use [Aspose.Cells for .NET][14] for the import of Excel file's content to the application data store, so that we can replace existing implementation. So far we have found it as fast and reliable.

## Summary

We believe that a software company like ours needs to focus on its core product. To develop faster and be competitive, you need significant libraries to delegate some of the R&D to them. We found [Aspose][15] to be a great solution to fit this theory. [Aspose][16] also provided a wide range of solutions. It is easier for us to work with one reliable provider for a range of needs that surface during software development.

**Vladimir Tyomin,  
**CTO, Commugen




[1]: https://www.commugen.com/en/
[2]: https://www.aspose.com/
[3]: https://docs.aspose.com/display/wordsnet/Features
[4]: https://downloads.aspose.com/words/net
[5]: https://products.aspose.com/words/net
[6]: https://products.aspose.com/words/family
[7]: https://products.aspose.com/words/net
[8]: https://products.aspose.com/words/net
[9]: https://products.aspose.com/words/net
[10]: https://products.aspose.com/
[11]: https://products.aspose.com/email
[12]: https://docs.aspose.com/display/emailnet/Features+Overview
[13]: https://products.aspose.com/email/net
[14]: https://products.aspose.com/cells/net
[15]: https://www.aspose.com/
[16]: https://www.aspose.com/




