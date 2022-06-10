---
title: 'Improved MS Word Document Comparison with Aspose.Words 16.10.0'
date: Sun, 16 Oct 2016 08:53:03 +0000
draft: false
url: /2016/10/16/improved-ms-word-document-comparison-with-aspose.words/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

[](http://www.aspose.com/.net/word-component.aspx)Aspose.Words 16.10.0 has been released. This month’s release contains over 109 useful new features, enhancements and bug fixes to the Aspose.Words product.

You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 16.10.0][1]
*   [Aspose.Words for Java 16.10.0][2]

Here is a look at just a few of the biggest features and API changes in this month’s release.

*   Added Feature to Get OOXML Compliance Version Determined from the Loaded Document.
*   Generate Results Closer to What MS Word Generates after Comparison
*   Support underline color during HTML import/export
*   Added Ability to Get Field Names from AddressBlock Field
*   Added Analogue of the Fields.Unlink Method
*   Added Feature to Preserve Page Field during Docx-Html-Docx Round-Trip

## Added Feature to Get OOXML Compliance Version Determined from the Loaded Document

We have added a new feature in Aspose.Wrods v16.10.0 to get OOXML compliance version determined from the loaded document content.

```
Document doc = new Document("in.docx");
OoxmlCompliance compliance = doc.Compliance;
```

Note that it makes sense only for OOXML documents. If you created a new blank document or load non OOXML document this property returns the OoxmlCompliance.Ecma376\_2006.

## Generate Results Closer to What MS Word Generates after Comparison

Document comparison has changed to compare at word level rather than at character level in Aspose.Wrods v16.10.0. This makes output looks more readable and closer to MS Word. Moreover, speed is greatly improved for big documents.

## Support underline color during HTML import/export

Support of underline color during HTML import/export has been added in Aspose.Wrods v16.10.0.

```
Document doc = new Document();
DocumentBuilder builder = new DocumentBuilder(doc);
builder.InsertHtml("<div><span style='color: red; text-decoration: underline;'>Aspose.Words</span></div>");
doc.Save(MyDir + @"Out.docx");
```

## Added Ability to Get Field Names from AddressBlock Field

We have introduced a new feature in Aspose.Wrods v16.10.0 to get the field name from Addressblock field.

```
FieldAddressBlock faddressbook = (FieldAddressBlock)doc.Range.Fields[0];
String[] names = faddressbook.GetFieldNames(); 
```




[1]: https://downloads.aspose.com/words/net
[2]: https://downloads.aspose.com/words/java




