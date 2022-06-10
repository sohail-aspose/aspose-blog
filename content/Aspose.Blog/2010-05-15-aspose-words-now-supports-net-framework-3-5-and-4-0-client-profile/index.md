---
title: 'Aspose.Words now supports .NET Framework 3.5 and 4.0 Client Profile!'
date: Sat, 15 May 2010 02:44:00 +0000
draft: false
url: /2010/05/15/aspose-words-now-supports-net-framework-3-5-and-4-0-client-profile/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

[.NET Framework Client Profile][1] is a subset of the .NET Framework optimized for client applications. Basically, it excludes some of the assemblies, for example, System.Web is excluded.

The Client Profile is available for .NET Framework 3.5 and 4.0. You can compile your project for the Client Profile in Visual Studio 2008 SP1 or Visual Studio 2010. You need to select to target the client profile in the project settings in Visual Studio.

One of the Aspose.Words' **Document.Save** overloads allows saving to a **System.Web.HttpResponse** object. This useful method sends a document to the client browser. But System.Web is not available in the .NET Framework Client Profile so it was not possible to use Aspose.Words to target the Client Profile before today's Aspose.Words for .NET 9.1 release.

Both the MSI and ZIP downloads now provide additional Aspose.Words assemblies that allow targeting the .NET Client Profile. In these new assemblies the Document.Save method with the HttpResponse parameter is not available.

Here is the contents of the readme.txt file that we now include in the download. This file describes what folder contains the assemblies you need to use with a particular version of the .NET Framework.

**Folder - Description**

**net1.1 -** Contains assemblies to use with .NET Framework 1.0 and 1.1

**net1.1\_AuthenticodeSigned -** Same as above, but the assemblies are digitally signed with Authenticode. Signed assemblies may load slower than without Authenticode.

**net2.0 -** Contains assemblies to use with .NET Framework 2.0, 3.0, 3.5, 4.0 and Mono. These are the assemblies that you should normally use.

**net2.0\_AuthenticodeSigned -** Same as above, but the assemblies are digitally signed with Authenticode. Signed assemblies may load slower than without Authenticode.

**net3.5\_ClientProfile -** Contains assemblies to use with .NET Framework 3.5 or 4.0 Client Profile.

**net3.5\_ClientProfile\_AuthenticodeSigned -** Same as above, but the assemblies are digitally signed with Authenticode. Signed assemblies may load slower than without Authenticode.




[1]: http://msdn.microsoft.com/en-us/library/cc656912.aspx




