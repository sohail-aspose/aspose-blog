---
title: 'How to do DOC to PDF conversion (and other conversions) in SharePoint'
date: Fri, 20 Apr 2007 04:26:00 +0000
draft: false
url: /2007/04/20/how-to-do-doc-to-pdf-conversion-and-other-conversions-in-sharepoint/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

_The complete article is here_ _Add DOC to PDF and Other Conversions to Microsoft Office SharePoint Server 2007 with Aspose Components__._

This article describes how you can add an ability to convert DOC to PDF (DOC2PDF) to Microsoft Office SharePoint Server 2007 (MOSS) using [Aspose.Words][1] and [Aspose.Pdf][2].

Microsoft Office SharePoint Server 2007 includes a new feature that allows to convert documents from one format (content type) to another. You can use document conversions to transform your content to suit your business requirements. You can invoke the conversion from the user interface or programmatically via the SharePoint Object Model.

SharePoint includes several document converters that you can use out of the box:

*   .DOCX (Office Open XML) to HTML web page (also .DOCM to web page)
    
*   InfoPath to HTML web page
    
*   XML to HTML web page
    

The set of document converters included with MOSS is limited. You can only convert DOCX, InfoPath and XML documents into web pages.

Thankfully, the document converters framework in SharePoint is extensible. It allows for custom converters to be implemented and seamlessly integrated into SharePoint allowing for any required content type conversion to be supported.

While Aspose components cannot be directly used as document converters for SharePoint out of the box, this article shows how you can easily create a small .NET application that wraps an Aspose component and works as a document converter for SharePoint.

**Selecting to convert a DOC document to PDF in MOSS.**




[1]: http://www.aspose.com/Products/Aspose.Words/
[2]: https://products.aspose.com/pdf




