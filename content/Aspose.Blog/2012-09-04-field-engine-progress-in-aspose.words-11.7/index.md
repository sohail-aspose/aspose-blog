---
title: 'Field Engine Progress in Aspose.Words 11.7'
date: Tue, 04 Sep 2012 08:25:15 +0000
draft: false
url: /2012/09/04/field-engine-progress-in-aspose.words-11.7/
author: DmitryV
summary: ''
tags: ['.NET', 'IncludePicture', 'MERGEFORMAT', 'TOC', 'fields', 'java', 'product release', 'reporting', 'table of content']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose.words-logo2.jpg" alt="">}}


We have just released Aspose.Words for .NET and Java 11.7. This month’s release includes almost 200 improvements to many areas of our components!

You can download the latest Aspose.Words release from the following links:

*   [Aspose.Words for .NET 11.7.0][1]
*   [Aspose.Words for Java 11.7.0][2]

Being responsible for the fields and reporting area of Aspose.Words, I would like to briefly let you know about the most notable improvements we recently made in this release.

## Table of Contents Improvements

TOC (Table of Contents) is with no doubts the most complex Microsoft Word field. In the Aspose.Words project, this field is backed with a number of relatively big classes responsible for collecting TOC entries, field building, updating, etc. Take into account that combining numerous TOC field switches can vastly change the appearance of the TOC and some nuances are even not documented gives you an idea why making it look “just like in MS Word” is no trivial task for us. The most complicated part is about TOC entry indentation and tab stop positioning.

While working on the recent Aspose.Words releases (11.6 and 11.7), we decided to concentrate on TOC’s functionality because we wanted to close most of TOC related issues accumulated in our defect tracking system. Around 70 TOC related unit tests that we have confirm that we have succeeded. Updating TOCs using Aspose.Words almost always looks identical or to Word in all test cases. Even huge and complex documents are handled properly!



{{< figure align=center src="images/TestTocFormatting1.png" alt="">}}


## MERGEFORMAT Improvements

MERGEFORMAT is another Microsoft Word feature whose logic is insufficiently documented and requires deep investigation. So far Aspose.Words has managed to produce very good results when formatting extremely complex fields (containing paragraph and section breaks and differently formatted text). We have recently we added to this excellent support by adding more tests (one of which contains around 100 formatting cases) and were able to close some previously reported issues.

Now using the MERGEFORMAT switch now gives expected result in all of our test cases.



{{< figure align=center src="images/TestMergeFormatRuns.png" alt="">}}


## INCLUDEPICTURE Support

The INCLUDEPICTURE field acts as a placeholder for a picture which may be dynamically inserted or replaced with another one in a Microsoft Word document. In context of Aspose.Words, the history of the INCLUDEPICTURE field has been dragging on from the beginning of project’s development. The difficulty has been the way it is loaded from Microsoft Word document and represented by the Aspose.Words API. By design the field is converted to an inline image (shape)  during document load and hence inner content can get lost from the model and only the resulting picture instead of the field is there. This behaviour has worked perfectly for most our customers for years though.

We have noticed that some of our customers wished to have full support for INCLUDEPICTURE preserved in the model, for example when they wanted to insert another picture by changing the source path and updating the field via Aspose.Words on the fly. That’s why we decided to provide such possibility. We implemented the update of the INCLUDEPICTURE’s field with no problems however simply removing the “INCLUDEPICTURE to shape” conversion would be unsafe – it just could not be tested thoroughly enough for all of our customers.

Therefore we solved this problem by associating this loading behavior to the new **LoadOptions.PreserveIncludePictureField** property and made it false by default so it won't accidentally affect anyone's existing code. So if you desire to preserve the INCLUDEPICTURE field when opening a document, simply create a **LoadOptions** object, set the **PreserveIncludePictureField** property to true and pass the object to the **Document** constructor like this:

```
LoadOptions lo = new LoadOptions();
lo.PreserveIncludePictureField = true;
Document doc = new Document("in.docx", lo);
```

Remember, though, that this behaviour is not typical for Aspose.Words and may potentially cause issues. Of course, you don’t need to use the new **LoadOptions** property if you simply insert the INCLUDEPICTURE field via **DocumentBuilder**. The update works perfectly whatever the origin of the field is:

```
DocumentBuilder builder = new DocumentBuilder();
builder.InsertField(@"INCLUDEPICTURE ""TestIncludePicture.jpg""");

// This line is actually redundant because the INCLUDEPICTURE field was updated
// right in the insertion method above.
builder.Document.UpdateFields();
```




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.words-for-.net/category1188.aspx
[2]: http://www.aspose.com/community/files/72/java-components/aspose.words-for-java/category1378.aspx




