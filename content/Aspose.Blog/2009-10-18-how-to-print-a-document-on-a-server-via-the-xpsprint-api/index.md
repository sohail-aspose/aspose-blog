---
title: 'How-to: Print a Document on a Server via the XpsPrint API'
date: Sun, 18 Oct 2009 03:29:00 +0000
draft: false
url: /2009/10/18/how-to-print-a-document-on-a-server-via-the-xpsprint-api/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Below is an summary from a new article in our documentation, click here to view the full article and download source code.  

This article can be useful to anyone who wants to submit an XPS document to the unmanaged XpsPrint API from a **.**NET application. But the main goal of this article is to show how to print a word processing document from an ASP.NET or Windows Service application using Aspose.Words and the XpsPrint API.  

## **Problem**  

When you develop a .NET application and you need to produce some printed output, you can use the classes in the **System.Drawing.Printing** namespace or the WPF classes. But, as it turns out, if you develop an ASP.NET or Windows Service application, then your options for printing are severely limited because Microsoft recommends against using these approaches. See the links below for more information.

*   [http://support.microsoft.com/kb/324565][1] - _The use of the .NET Framework Printing classes is not supported by a service. This includes ASP pages, which generally run in the context of the server service._
*   _http://msdn.microsoft.com/en-us/library/system.drawing.printing.aspx - Classes within the System.Drawing.Printing namespace is not supported for use within a Windows service or ASP.NET application or service. Attempting to use these classes from within one of these application types may produce unexpected problems, such as diminished service performance and run-time exceptions._
*   [http://msdn.microsoft.com/en-us/library/bb613549.aspx][2] - _The use of WPF to build Windows services is unsupported. Because WPF is a presentation technology, the Windows service requires the appropriate permissions to perform visual operations that involve user interaction. If the Windows service does not have the appropriate permissions, there may be unexpected results._

The **Aspose.Words.Document** object provides a family of the **Print** methods to print documents and these methods print via the .NET printing classes defined in the **System.Drawing.Printing** namespace. There are many customers of Aspose.Words who use this printing method in their server-side applications without any problems, but there is a way to comply with Microsoft’s recommendations and it is described in this article.  

## **Solution**

The proper way to print documents according to Microsoft is to use the unmanaged [XpsPrint API][3].aspx). This API is available on Windows 7, Windows Server 2008 R2, and also on Windows Vista, provided the [Platform Update for Windows Vista][4] is installed.  

Since Aspose.Words can easily convert any document to XPS, we only need to write code that passes an XPS document to the XpsPrint API. The only problem is that the XpsPrint API is unmanaged and it requires some knowledge of the Platform Invoke.




[1]: https://docs.aspose.com/display/3dnet/Home
[2]: http://msdn.microsoft.com/en-us/library/bb613549.aspx
[3]: http://msdn.microsoft.com/en-us/library/dd374565(VS.85
[4]: https://www.microsoft.com/en-us/download/




