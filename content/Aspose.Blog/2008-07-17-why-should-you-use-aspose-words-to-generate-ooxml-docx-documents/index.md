---
title: 'Why should you use Aspose.Words to generate OOXML (DOCX) documents?'
date: Thu, 17 Jul 2008 01:47:00 +0000
draft: false
url: /2008/07/17/why-should-you-use-aspose-words-to-generate-ooxml-docx-documents/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Let me start a bit off-topic with: **Why should you use Aspose.Words to generate DOC documents?**

Since 2004, Aspose.Words has been an excellent library for reading, converting and generating binary DOC Microsoft Word documents. There is a question on Joel Spolsky's discussion group How do Aspose and Others Generate Office Docs that unfortunately I did not have an opportunity to answer. One comment there says:

_...you need to duplicate many, many man years of work in order to do this?  
  
Has Apose really done this much work, or do they have a licensing agreement with MS to use the MS source code/libraries in order to generate the Office documents without Office automation?_

My reply to this would be: _Yes, we have put a lot of effort into reverse engineering DOC and trying to support every feature we could find. We did not have a licensing agreement with Microsoft because at that time it was very restrictive about what you could develop after you sign it. It cost us around 8 man years to support DOC and still counting because now the DOC specification is open and we are working on  features that were too obscure before._

Therefore: You use Aspose.Words to generate DOC documents simply because it is the best available tool for this job.

Now: **Why should you use Aspose.Words to generate OOXML (DOCX) documents?**

Office Open XML is great news for all. It opens up so many possibilities. Some say that because it is open and XML you can generate it yourself! But unless you are generating a very simple document, you will quickly get bogged down in details. The OOXML specification is over 6000 pages and it is complex. Simply because other document formats are open (such as PDF) not many developers think of generating PDF documents themselves. They look for a 3rd party product. The same is true for OOXML.

When you are searching for an OOXML library you could choose from one of the free or commercial libraries and their number will inevitably grow. Why choose Aspose.Words?

Remember these reasons:

1.  We put a lot of effort into supporting OOXML. Even though OOXML is an ISO standard (which has been thoroughly reviewed and tested), there is a lot of tiny little odd and undocumented things. For example, there are documents where if you omit an **optional empty string**  o:title="" attribute, MS Word will display an image properly when loaded from a disk file, but will refuse to display the image when the document is retrieved in Internet Explorer from a URL. That behaviour is not documented! We at Aspose constantly work, find and resolve such issues.  
    
2.  Aspose.Words offers not only full OOXML support, but a cohesive set of several important features: high-fidelity conversion to/from DOC, RTF, WordML 2003 as well as OpenDocument, HTML, MHTML and PDF formats, rich document object model and report generation capabilities.

There is simply no alternative to Aspose.Words.








