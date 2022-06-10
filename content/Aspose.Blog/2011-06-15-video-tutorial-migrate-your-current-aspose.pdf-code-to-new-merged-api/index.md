---
title: 'Video tutorial - Migrate your current Aspose.Pdf for .NET code to new Merged API'
date: Wed, 15 Jun 2011 16:57:50 +0000
draft: false
url: /2011/06/15/video-tutorial-migrate-your-current-aspose.pdf-code-to-new-merged-api/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'Merged Aspose.Pdf', 'PDF', 'video tutorial']
categories: ['Aspose.Total Product Family', 'Aspose.PDF Product Family']
---

![Aspose.Pdf icon][1]

As a sequel to our previous blog posts announcing the release of new Merged Aspose.Pdf API (_which is expected to be rolled out by the start of next month July_), this blog post presents a video tutorial on migrating your existing code based on Aspose.Pdf for .NET to new Merged Aspose.Pdf for .NET API. Just a recap before I proceed further, this new component will have all the features currently available in Aspose.Pdf for .NET and all the features currently available in Aspose.Pdf.Kit for .NET, plus some new features will also be introduced in this API.

For the sake of code migration from current Aspose.Pdf for .NET to new merged Aspose.Pdf, you only would be required to make few minor changes. Currently, all the classes are present under Aspose.Pdf namespace. However in the merged product, all the classes of the Aspose.Pdf component have been moved under Aspose.Pdf.Generator namespace. If you are only importing Aspose.Pdf namespace then you only need to change it to Aspose.Pdf.Generator. However, if you are using the namespace along with the class names, then you’ll have to change the namespace in the code wherever it's required.

Please take a look over following video tutorial in which we have explained the steps on migrating a simple Hello World application to use the new Merged API.

Please don't forget to check out the other blog post on Migrating from Legacy Code to Merged Aspose.Pdf for .NET"




[1]: http://www.aspose.com/Images/aspose.pdf-logo2.jpg




