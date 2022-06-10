---
title: 'Running Aspose.Words in the Windows Azure Cloud'
date: Thu, 20 Aug 2009 16:23:00 +0000
draft: false
url: /2009/08/20/running-aspose-words-in-the-windows-azure-cloud/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

**What is Windows Azure?**

The [Windows Azure Platform][1] (Azure) is an internet-scale cloud services platform hosted in Microsoft data centers. Azure enables developers to quickly and easily create applications running in the cloud using their skills with the .NET Framework.

Applications running in Windows Azure essentially run inside 64-bit virtual machines running Microsoft Server 2008. Each virtual machine provides .NET Framework 3.5 and can provide an ASP.NET environment.

**Why Aspose.Words in Azure?**

Azure provides services to run applications and store data. A great number of Internet-connected web and corporate applications will be built to run in Azure. These applications will require capabilities to generate, transform and store various types of documents. The documents could be contracts, reports, policies, resumes, invoices and so on.

Aspose.Words for .NET is a class library that can be used on a server for generating, converting and processing documents in a variety of formats. It makes a perfect sense to use Aspose.Words for .NET to solve document programming tasks when you develop an application to run in Windows Azure.

Here are just some ideas how you can use Aspose.Words for .NET in Azure:

Convert documents uploaded by users in various formats into a standard, for example DOCX format and store in the Windows Azure Storage.

Load a document template from the Windows Azure Storage and populate it with data from SQL Azure to generate a report, contract or another document.

Generate a document (for example, invoice) and convert it to the PDF or XPS format and send to the client browser.

Convert a document to PDF/A or TIFF for long-term archiving in the Windows Azure Storage.

Accept requests from the clients in a WebRole application via ASP.NET pages or WCF calls and perform actual document processing in load balanced WorkerRole applications.

You can use all of the Aspose.Words for .NET features from Windows Azure applications. Aspose.Words for .NET does not depend on Azure.

**Can I use Aspose.Words in Windows Azure Already?**

Yes, but it is better to wait until the next version Aspose.Words for .NET 6.7 comes out in early September 09. We have now completed testing on Windows Azure, resolved some issues and added convenience features.

**New Aspose.Words Samples for Windows Azure**

The next version of Aspose.Words will include a new section in the documentation with two sample projects for Windows Azure.

One of the sample projects is called ConvertDocumentSimple. It is a very simple application that loads, converts and saves a document. Although it is very simple and does not rely on any advanced services of the Windows Azure platform, it demonstrates that Aspose.Words can be used to easily build applications that run in the cloud.  

We have already deployed this application to Windows Azure and you can try it out live here _http://asposewords.cloudapp.net/_.

The following are the screenshots of how we developed and depoyed the sample applications.




[1]: https://azure.microsoft.com/en-gb/




