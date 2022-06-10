---
title: 'Field evaluation and list numbering improved in Aspose.Words for .NET 9.4'
date: Sat, 11 Sep 2010 10:38:00 +0000
draft: false
url: /2010/09/11/field-evaluation-and-list-numbering-improved-in-aspose-words-for-net-9-4/
author: DmitryV
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

I am glad to share that we have improved the evaluation of Microsoft Word fields when the document is rendered. There is a number of fields recalculated during rendering, such as PAGE, NUMPAGES, SECTIONPAGES and so on. Now imagine that you need to display, for example, different text on the last page of document. The following condition can be used:

{ IF {PAGE} = {NUMPAGES} “This is the last page” “See next page” }

Until the 9.4 release the result of the outermost IF field did not update during rendering, so an incorrect value was displayed in the output PDF or image file. Now it is fixed and working properly:

Another improvement has to do with list labels recalculation. You can call **Document.UpdateListLabels()** to update list labels for all list items in the document and then access the up-to-date values via the **Paragraph.ListLabel.LabelString** and **Paragraph.ListLabel.LabelValue** properties. Actually Microsoft Word follows some tricky list numbering rules (such as independent numbering in different stories etc) and these rules are now obeyed in Aspose.Words for .NET 9.4, too. Just have a look at a test document we use:

Hopefully you will enjoy working with the new version of our product. Please visit the download page at [http://www.aspose.com/community/files/51/.net-components/aspose.words-for-.net/entry258045.aspx][1].




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.words-for-.net/entry258045.aspx




