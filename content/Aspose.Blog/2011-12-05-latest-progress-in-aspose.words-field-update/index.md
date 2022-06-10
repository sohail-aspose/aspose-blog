---
title: 'Latest Progress in Aspose.Words'' Field Update'
date: Mon, 05 Dec 2011 10:31:50 +0000
draft: false
url: /2011/12/05/latest-progress-in-aspose.words-field-update/
author: DmitryV
summary: ''
tags: ['Microsoft Word', 'fields']
categories: ['Aspose.Words Product Family']
---

[Aspose.Words][1]' support of Microsoft Word fields is being improved all the time. At the moment, Aspose.Words updates around 3/4 of all  Microsoft Word fields that can be updated. We're hoping to support all 'updateable' fields before long. In the meantime, I'd like to share what progress we have made recently and what fields we have added to the supported list. I will use the same categorization offered by Word and OOXML specs.

## Date and Time

While updating DATE and TIME fields were supported from the very beginning (due to the simplicity of implementation), the remaining fields in this category stayed unsupported for a significant time. The fields are:

*   CREATEDATE
*   EDITTIME
*   PRINTDATE
*   SAVEDATE

Recently we filled this gap so that Aspose.Words can now update all Date and Time fields.

## Document Automation

Aspose.Words supports all Document Automation fields that it makes sense to update. Two of them, GOTOBUTTON and MACROBUTTON, are not updateable, but were improperly displayed when rendering to PDF or image or saving to a format like HTML. The latest release of Aspose.Words fixes this issue.

## Document Information

Like for the Date and Time category, we supported the evaluation of all Document Information fields that were overlooked earlier. So the following fields are updated in the latest release:

*   AUTHOR
*   COMMENTS
*   FILENAME
*   FILESIZE
*   KEYWORDS
*   LASTSAVEDBY
*   NUMCHARS
*   NUMPAGES
*   NUMWORDS
*   SUBJECT
*   TEMPLATE
*   TITLE

## Index and Tables

We have been working hard on one of the most popular Microsoft Word fields – table of contents (TOC). At the moment, Document.UpdateFields() (or Field.Update()) produces identical or very close result to how it looks after pressing F9 in Microsoft Word. In particular, we have fine-tuned tab stop positions generated for TOC entries in the latest release. Still, there is much work to do for this field because it is probably the most complex one.



{{< figure align=center src="images/05-12-2011-14-06-49.png" alt="">}}


There are a few fields in this category whose update is not supported yet, but they are on our TODO list and will be handled in the near future.

## Mail Merge

We have added support for two complex mail merge fields – ADDRESSBLOCK and GREETINGLINE. These two behave like compound MERGEFIELDs, allowing you to compose (surprise!) an address block or greeting line, respectively:



{{< figure align=center src="images/05-12-2011-14-03-13.png" alt="">}}




{{< figure align=center src="images/05-12-2011-14-03-31.png" alt="">}}


Also, the SET field is now supported, which means you can use it to define bookmark values.

## Numbering

The SEQ field is now fully supported.




[1]: https://products.aspose.com/words




