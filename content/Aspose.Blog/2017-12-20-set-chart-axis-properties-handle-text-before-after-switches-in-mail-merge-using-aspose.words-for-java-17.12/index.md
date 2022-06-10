---
title: 'Set Chart Axis Properties, Handle Text Before After Switches in Mail Merge using Aspose.Words for Java 17.12'
date: Wed, 20 Dec 2017 09:57:49 +0000
draft: false
url: /2017/12/20/set-chart-axis-properties-handle-text-before-after-switches-in-mail-merge-using-aspose.words-for-java-17.12/
author: Awais Hafeez
summary: ''
tags: ['Handle text before or after switches in Mail Merge', 'Java API for Mail Merge', 'Set chart axis properties in Word in Java']
categories: ['Aspose.Words Product Family']
---

We are pleased to announce the new monthly release of **Aspose.Words for Java 17.12**. The release of this month contains a number of new features, enhancements and bug fixes of the issues reported by our users in previous versions. Please check the detailed [release notes of Aspose.Words for Java 17.12][1] to get an idea about all the new features/enhancements and fixes made in this release. Furthermore, if you are planning to upgrade the API from any previous version, we strongly recommend you to check the Public API Changes section of current release and other intermediate releases from release notes folder, to know what has been changed since your current revision of the API.

The following sections describe some details regarding these newly added features/enhancements.

## Implemented API to Set Chart Axis Properties

If you want to work with chart axis, scaling, and display units for the value axis, please use ChartAxis, AxisDisplayUnit, and AxisScaling classes. The following article shows how to define X and Y axis properties.  
[How to Set Chart Axis Properties][2]

## Added Feature to Get the docPartGallery Value of StructuredDocumentTag of Type SdtType.DocPartObj

We have improved the behavior of the following properties. Now, you can get the value of these properties for "Markup.SdtType.DocPartObj" SdtType.

```
 public class StructuredDocumentTag
{
    .....
 
    public string BuildingBlockGallery{ get; set;}
 
    public string BuildingBlockCategory{get; set;}
 
    .....
} 
```

## Changed Return Type for FieldMergingArgsBase.Field

We have provided typed access to a merge field’s properties in this release of Aspose.Words. We have changed the return type of the FieldMergingArgsBase.Field property (and hence of the corresponding descendants’ properties) from Field to FieldMergeField. Please refer to the following article for more detail.  
[How to Handle Text Before and After Switches During Mail Merge Operation][3]

## Other Improvements

There are 91 improvements and fixes in this regular monthly release. The most notable are:

*   PixelFormat property in ImageSaveOptions class.
*   Metered License upgraded to REST API 1.2.
*   Fixed few Veracode issues reported by user.
*   Implemented API to set chart axis properties.
*   Added feature to get the docPartGallery value of StructuredDocumentTag of type SdtType.DocPartObj.
*   Horizontal and vertical flipping attributes are now taken into account when rendering DML textboxes.
*   Improved rendering of diacritics for "Courier New" font.
*   Multiline MathML expressions rendering fixed.
*   EMR\_ROUNDRECT records processing while rendering metafiles fixed.
*   PDF Rendering of indexed images while converting to CMYK color space fixed.
*   OTF(CFF) fonts to PDF/A documents export fixed.
*   DML Charts with the empty area do not throw an exception on rendering now.
*   Fixed scaling problem with DML bubble charts on rendering.
*   LINQ Reporting Engine supports the dynamic setting of chart axes’ titles.
*   Improved handling of decimal tab alignment in cells when the paragraph has a hanging indent.
*   Improved text wrapping when the line contains single or no characters.
*   Improved handling of cell margins and table alignment.
*   Improved cell alignment when the line has trailing spaces and custom tabs.
*   Improved handling of collapsed paragraphs.
*   Fixed exception in the rare case when line breakpoint cannot be found.
*   Fixed exception when the document is saved with revision balloons inside of a cell.

## Aspose.Words for Java Resources

The following resources will help you work with Aspose.Words for Java:

*   [Home page for Aspose.Words for Java][4]
*   [Install Aspose.Words for Java from Maven][5]
*   Words product family forum – Post your technical questions and queries, or any other problem you faced while running Aspose.Words APIs.
    *   [Free Support Forum][6]
    *   [Paid Support Forum][7]
*   [Aspose.Words for Java online documentation][8]– Help documentation.
*   [Aspose.Words for Java online API reference][9]– API reference documents.
*   [Enable Blog Subscription][10]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words, APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
*   [Aspose.Words for Java Examples][11] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+17.12+Release+Notes
[2]: https://docs.aspose.com/display/wordsjava/Working+with+Charts#WorkingwithCharts-HowtoSetChartAxisProperties
[3]: https://docs.aspose.com/display/wordsjava/How+to+Execute+Mail+Merge#HowtoExecuteMailMerge-HowtoHandleTextBeforeandAfterSwitchesDuringMailMergeOperation
[4]: https://products.aspose.com/words/java
[5]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-words/
[6]: https://forum.aspose.com/c/words
[7]: https://helpdesk.aspose.com/
[8]: https://docs.aspose.com/display/wordsjava/Home
[9]: https://apireference.aspose.com/java/words
[10]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[11]: https://github.com/aspose-words/Aspose.Words-for-Java




