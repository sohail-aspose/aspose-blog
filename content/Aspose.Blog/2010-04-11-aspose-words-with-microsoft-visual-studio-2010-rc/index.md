---
title: 'Aspose.Words with Microsoft Visual Studio 2010 RC'
date: Sun, 11 Apr 2010 23:06:00 +0000
draft: false
url: /2010/04/11/aspose-words-with-microsoft-visual-studio-2010-rc/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Some customers have reported they cannot build an application with Aspose.Words in Microsoft Visual Studio 2010 RC.

We confirm you cannot build a project if you select one of the following **Target framework** settings in the **Project Properties**:

*   .NET Framework 3.5 **Client Profile**
*   .NET Framework 4.0 **Client Profile**

The error message is _"... it has a dependency on Sysem.Web ... which is not in the currently targeted framework"_.

Yes, Aspose.Words has a dependency on System.Web to provide a Document.Save method that allows to save a document directly into an HttpResponse object.

We currently release two Aspose.Words.dll assemblies. One is targeting .NET 1.1 and the other is targeting .NET 2.0. So far it has been no problem. Aspose.Words does not use or rely on any of the .NET 3.0, 3.5 or 4.0 features and we did not need to build Aspose.Words.dll targeting any of these frameworks because Aspose.Words.dll that targets .NET 2.0 loaded and run successfully on all these versions. A few months ago we even tested Aspose.Words with Microsoft Visual Studio 2010 Beta and there was no problem.

We are going to resolve this immediately and release a hotfix within a week or so. Most likely we will be providing separate Aspose.Words.dlls that target every .NET framework version in our downloads.








