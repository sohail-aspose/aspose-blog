---
title: 'Support of Automatic Detection of Text file''s Encoding, Import of MathML from HTML and Cross References are Preserved during HTML Import/Export in Aspose.Words 16.4.0'
date: Fri, 13 May 2016 07:26:05 +0000
draft: false
url: /2016/05/13/automatic-detection-of-text-file-encodin-import-of-mathml-from-html-and-cross-references-are-preserved-during-html-import-export-in-aspose.words-16.4.0.html/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

[](http://www.aspose.com/.net/word-component.aspx)Aspose.Words 16.4.0 has been released. This month’s release contains over 106 useful new features, enhancements and bug fixes to the Aspose.Words products.

You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 16.4.0][1]
*   [Aspose.Words for Java 16.4.0][2]

Here is a look at just a few of the biggest features and API changes in this month’s release.

*   Automatic Detection of Encoding of a Text file
*   Import MathML from HTML Document
*   Preserve Cross Reference during HTML Import/Export
*   Added Feature to Export Content Control to Div tag
*   Improved PDF A1b Compliancy
*   Improved Positioning of Pictures Inside Tables
*   Added Field.Update() Overload Method

## Added Field.Update() Overload Method

We have introduced a way to update a field ignoring the MERGEFORMAT switch. Field.Update(true) abandon the direct field result formatting regardless of the MERGEFORMAT switch.

```
public void Update(bool ignoreMergeFormat) 
```

## Preserve Cross Reference during HTML Import/Export

We have introduced new feature in Aspose.Words 16.4.0 to preserve cross reference in Word documents during Word document>Html>Word document round-trip.

## Automatic Detection of Encoding of a Text file

Starting from Aspose.Words v16.4.0, there is no need to set LoadOptions.Encoding. Aspose.Words automatically detects encoding of text file.

## Import MathML from HTML Document

We have introduced new feature in Aspose.Words 16.4.0 to import HTML formatted equation information (MathML) into OfficeMath.




[1]: http://www.aspose.com/downloads/words-family/net
[2]: http://www.aspose.com/downloads/words-family/java




