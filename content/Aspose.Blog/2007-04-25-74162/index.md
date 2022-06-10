---
title: 'Aspose.Words for .NET 4.2.2 Released'
date: Wed, 25 Apr 2007 02:33:00 +0000
draft: false
url: /2007/04/25/74162/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

This is a maintenance release. Here is what's been fixed:

**RTF**

*   Duplicate error when using ImportNode. 
*   Images appear smaller when RTF (from Crystal Reports) is converted to PDF 

**DOC**

*   Null reference error when saving a document.
*   Loading DOC with CoordSize zero throws exception 
*   'Not expected other image formats here.' exception during Wml2Doc conversion.

**WordML**

*   Saving WordML document that has hyperlinks but has no Document.BaseUri throws
*   Local path is escaped incorrectly when exporting to WML 
*   Support well-known color names in w:color elements 

**HTML**

*   Import of hex character entities does not work 
*   Export vertical text to HTML 
*   Line breaks exported to HTML sometimes missing 

**PDF**

*   Before and After spacing between paragraphs needs better handling
*   A border shows around an image that does not have it originally. 
*   Nested FloatingBox output to PDF XML 
*   A paragraph that ends with a line break should take two lines, but takes only one in PDF 

**Mail Merge**

*   MailMerge takes formatting from field value run, whereas it should take it from field code run.

For those who are waiting on other fixes, don't worry, there will be another hotfix coming out soon.

To download http://www.aspose.com/Downloads/Aspose.Words/Default.aspx








