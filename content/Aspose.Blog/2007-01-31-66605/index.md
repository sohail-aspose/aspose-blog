---
title: 'AWesome RTF'
date: Wed, 31 Jan 2007 22:09:00 +0000
draft: false
url: /2007/01/31/66605/
author: DmitryV
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Finally it is [released][1], the thing that you were waiting for so long. Yet another format is fully added to Aspose.Words arsenal, and this is Rich Text Format. Today we have released RTF importing module, thus keeping our promises to make it public in January (although it's 31st ![Smile [:)]][2].

The release does not mean, however, that working on the module is stopped. We will be polishing the code, making it more and more resilient to badly formed RTF, and fixing any formatting issues you report.

Let me explain why the development is not over. The RTF format itself is not so strict and neat from a developer's point of view as one would wish. But what is more troublesome is that most third-parties simply did not follow the rules declared in the spec or followed them quite frivolously. RTF was developed around 20 years ago; can you imagine how many different third-party RTF tools was developed in the course of these 20 years? That seems to be the main cause led to producing heaps of awkward and corrupted RTF documents. However, Microsoft Word seems to be very resilient to such documents. It rarely crashes and does open badly formed RTF okay. That means we ought to act similarly.

But Microsoft Word's history counts around 18 years (almost as long as RTF itself), and Aspose.Words is only 3+ years old ![Smile [:)]][3]. We want this kid to be as resilient to incorrect RTF as the format's "native" application, and we want the formatting to be exactly like that shown by Word. We've managed to test around 1000 documents downloaded from the Web by involving our Google Proofing project (in addition to our common unit tests). We were shocked! Some of the documents just ignored any rules and recommendations declared in the RTF specification. I'm proud to say that Aspose.Word failed only on ~60 of them, and most of the issues had been fixed by the moment of release. Pretty good for start.

Yet the 1000 documents are a drop in the ocean. We are going to keep testing arbitrary documents from the Web, but we also require your assistance. It's simple: if you ever come across an RTF document that throws an exception or contains formatting issues when imported by Aspose.Words, just report it in the [support forum][4] and attach the document(s) to your post. Then I will try to fix the issue immediately or once I'm able to, depending on the complexity of the case. We want to refine the importing module so that it would accept any valid or corrupted RTF document and build a proper document model. That's the real cooperation which would allow us to open another AWesome page in Aspose.Words history.

Besides, our next step in improving RTF import is optimization of the code, increasing performance and minimizing memory impact. I will keep you posted about the progress.




[1]: https://docs.aspose.com/display/wordsjava/Mail+Merge+and+Reporting
[2]: https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/pdf/272x272/aspose_pdf-for-net.png)
[3]: https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/pdf/272x272/aspose_pdf-for-net.png
[4]: https://docs.aspose.com/display/wordsjava/Mail+Merge+and+Reporting




