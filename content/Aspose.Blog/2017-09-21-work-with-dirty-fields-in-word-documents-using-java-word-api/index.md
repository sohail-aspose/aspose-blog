---
title: 'Work with Dirty Fields in Word Documents using Java'
date: Thu, 21 Sep 2017 06:18:51 +0000
draft: false
url: /2017/09/21/work-with-dirty-fields-in-word-documents-using-java-word-api/
author: Tilal Ahmad
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose-Words-for-Java.png" alt="">}}


A new version [Aspose.Words for Java 17.9][1] has been published. It includes all the features, enhancements and fixes introduced in its corresponding .NET version along with fixes of the issues reported in previous versions’ of Aspose.Words for Java. Some of the important enhancements are support of dirty fields, Open Document measure unit and restart list for each section along with other important enhancements and fixes. Please check the detailed [release notes of this version][2] to get an idea about all the new features/enhancements and fixes made in this release.

Furthermore, if you are planning to upgrade the API from any previous version, we strongly recommend you to check the [Public API Changes section of current release][3] and other intermediate releases from [release notes folder][4], to know what has been changed since your current revision of the API.

The following sections describe some details regarding these newly added features/enhancements.

## Support of Dirty Fields in Word Documents

In this version, we have introduced support related to the dirty (stale) state of the fields and controlling whether such fields should be updated. New public properties are included in Field and FieldChar class to flag Field for update at the time of document opening.  
Another new property setUpdateDirtyFields property in LoadOptions class is introduced to specify whether to update the fields with the dirty attribute. When the value of LoadOptions.setUpdateDirtyFields() is set to true, all fields having true value for Field.IsDirty or FieldChar.IsDirty property are updated on document load. Please read following article for more detail: [Update Fields with Dirty attribute][5]

## Support of Open Document Measure Unit

Open Office uses centimeters as measuring unit for specifying lengths, widths and other measurable formatting and content properties in documents. A new feature has been added in this release to specify unit of measure apply to open document contents. The OdtSaveOptions.setMeasureUnit() property is added for this purpose. You can set measure unit as Centimeters or Inches. Please check following documentation link for sample code and details:  
[Specify Measuring Unit of Open Document][6]

## Clear Contents of Structured Document Tag

We have received some requests to provide functionality to clear contents of Structured Document Tag(SDT). The StructuredDocumentTag.clear method has added for this purpose, it clears the contents of structured document tag and displays a placeholder if it is defined. Please check the code example and read more detail from following article.  
Clear Contents of Structured Document Tag

## Added SaveOptions.UpdateLastSavedTimeProperty Property

We have added the SaveOptions.UpdateLastSavedTime Property in Aspose.Words for Java 17.9 that controls whether to update the corresponding built-in document property on document save. Please read more detail about the feature from following link.  
[Update LastSavedTime Property before Saving][7] 

## Restart List for Each Section

We have added the List.IsRestartAtEachSection property in Aspose.Words for Java 17.9 to restart List for each section. Note that this option is supported only in RTF, DOC and DOCX document formats. Please follow this link for more details:   
[Restart List for each Section][8]

## Other Improvements

There are 87 improvements and fixes in this regular monthly release. The most notable are:

*   New performance fixes.
*   Caching of shading patterns for PDF output implemented. The output size of PDF documents with the repeating images (e.g. in header/footer) is now significantly reduced.
*   Improved character spacing control handling for Asian text.
*   Improved table grid calculation when a paragraph in a cell has large indents.
*   Improved text wrapping in narrow line band when there is a leading tab stop.
*   Added feature to set Placeholder Text of Structured Document Tag.
*   Added feature to support w:dirty attribute on a field.
*   Updating value of SaveDate field just by doing open/save

## Aspose.Words for Java Resources

The following resources will help you work with Aspose.Words for Java:

*   [Home page for Aspose.Words for Java][9]
*   [Download Aspose.Words for Java][10]
*   [Install Aspose.Words for Java from Maven][11]
*   Words product family forum – Post your technical questions and queries, or any other problem you faced while running Aspose.Words APIs.
    *   [Free Support Forum][12]
    *   [Paid Support Forum][13]
*   [Words for Java online documentation][14]– Help documentation.
*   [Words for Java online API reference][15]– API reference documents.
*   [Enable Blog Subscription][16]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words, APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
*   [Words for Java Examples][17]– We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/words/java/new-releases/aspose.words-for-java-17.9/
[2]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+17.9+Release+Notes
[3]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+17.9+Release+Notes
[4]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java
[5]: https://docs.aspose.com/display/wordsjava/Insert+and+Remove+Field#InsertandRemoveField-UpdateFieldshavingDirtyAttribute
[6]: https://docs.aspose.com/display/wordsjava/Saving+a+Document#SavingaDocument-SpecifyUnitofMeasuretoOpenDocument
[7]: https://docs.aspose.com/display/wordsjava/Working+with+Document#WorkingwithDocument-UpdateLastSavedTimePropertyBeforeSaving
[8]: https://docs.aspose.com/display/wordsjava/Working+with+Lists#WorkingwithLists-HowtoRestartListforeachSection
[9]: https://www.aspose.com/products/words/java
[10]: https://downloads.aspose.com/words/java
[11]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-words/
[12]: https://forum.aspose.com/c/words
[13]: https://helpdesk.aspose.com/
[14]: https://docs.aspose.com/display/wordsjava/Home
[15]: https://apireference.aspose.com/java/words
[16]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[17]: https://github.com/aspose-words/Aspose.Words-for-Java




