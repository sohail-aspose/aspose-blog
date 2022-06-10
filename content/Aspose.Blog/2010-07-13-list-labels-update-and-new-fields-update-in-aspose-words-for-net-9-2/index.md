---
title: 'List Labels Update and New Fields Update in Aspose.Words for .NET 9.2'
date: Tue, 13 Jul 2010 15:45:00 +0000
draft: false
url: /2010/07/13/list-labels-update-and-new-fields-update-in-aspose-words-for-net-9-2/
author: DmitryV
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Aspose.Words for .NET provides a comprehensive support for Microsoft Word lists. You can access a number of list properties, such as list levels, numbering format, and many others. Literally, you can access every list feature Microsoft Word's UI offers.  

However, until recently, you could not get the exact value of list label for each list item (paragraph) in the document. That is, if a certain paragraph had a list label like _2.1.4._, you could not access it via the Aspose.Words API. I am glad to announce this is possible now.  

Aspose.Words for .NET 9.2 has introduced a new method named **Document.UpdateListLabels()**. This method recalculates list label values for each list item throughout the document. After you call it, you can access up-to-date list label values using the **Paragraph.ListLabel.ListString** and **Paragraph.ListLabel.ListValue** properties. The former one returns a text string that represents the appearance of the list value for the label, and the latter one returns a numeric value for this label:

```
Document doc = new Document(“MyDoc.docx”);

// Update list labels throughout the document.
doc.UpdateListLabels();

Paragraph paragraph = (Paragraph)doc.GetChild(NodeType.Paragraph, 10, true);

// Gets a text like ‘2.1.4.’.
string labelString = paragraph.ListLabel.LabelString;
// Gets a numeric value like 4 (the actual number of the list item on the level).
int labelValue = paragraph.ListLabel.LabelValue;
```

Note that **UpdateListLabels()** is sometimes implicitly called when updating document fields. This is required by some fields like TOC or REF that need list labels to be up-to-date.  

By the way, the REF and INCLUDETEXT fields are now updated via Aspose.Words for .NET 9.2 API.  

To download Aspose.Words for .NET 9.2, please visit [https://downloads.aspose.com/words][1].




[1]: https://downloads.aspose.com/words




