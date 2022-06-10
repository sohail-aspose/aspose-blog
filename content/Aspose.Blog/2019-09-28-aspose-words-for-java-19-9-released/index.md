---
title: 'Advanced HarfBuzz Shaper based Typography Supported by Aspose.Words for Java 19.9'
date: Sat, 28 Sep 2019 09:04:47 +0000
draft: false
url: /2019/09/28/aspose-words-for-java-19-9-released/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Today, I will highlight the major features introduced in [Aspose.Words for Java 19.9][1] release:

## OpenType Fonts and Kerning Features Supported

OpenType is a font format for scalable computer fonts and introduced to provide better support for languages and writing systems as compared to PostScript and TrueType. We have added TextShaperFactory property in LayoutOptions class. This property is used to get or set [ITextShaperFactory][2] implementation used for Advanced Typography rendering features. How does this feature work? It’s very simple. Please check the code example and detail in the following article.  
[How to Use OpenType Features][3]

## Create Repeating Section Content Control

The repeating section content control allows repeating the content contained within it. Using Aspose.Words for Java, the structured document tag nodes of the repeating section and repeating section item types can be created and for this purpose, [SdtType enumeration type][4] provides REPEATING\_SECTION\_ITEM member. The following code example demonstrates how to bind a repeating section content control to a table.  

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-programming_documents-StructuredDocumentTag-WorkingWithStructuredDocumentTag-CreatingTableRepeatingSectionMappedToCustomXmlPart.java" >}}

## LINQ Reporting using XML, JSON, and CSV Data Sources

The LINQ Reporting engine of Aspose.Words for Java now enables you to reference business objects of your application in report templates. We have added XmlDataSource, JsonDataSource, and CsvDataSource classes in this release to use XML, JSON, and CSV as data sources to generate reports using LINQ Reporting. Please read the following articles for complete detail of this feature.

*   [Accessing XML Data][5]
*   [Accessing JSON Data][6]
*   [Accessing CSV Data][7]

## Create and Modify VBA Macros

The following code example demonstrates [how to modify VBA Macros][8] from the document using the VbaModule.setSourceCode() property.

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-loading_saving-WorkingWithVbaMacros-ModifyVbaMacros.java" >}}

## Link Custom Document Property to Bookmark

Aspose.Words for Java now provides a method CustomDocumentProperties.addLinkToContent(String, String) to create a new 'linked to content' custom document property which returns the newly created property object or null if the link source is invalid. The following code example demonstrates how to configure the link to a content custom property.

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-properties-ConfiguringLinkToContent-ConfiguringLinkToContent.java" >}}

## See also Useful Links

*   [Aspose.Words for Java Online Documentation][9] - up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Words for Java Product Page][10]
*   [Install Aspose.Words for Java from Maven][11]
*   [Aspose.Words for Java API Reference Guide][12] - detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Download Examples at GitHub Repository][13] - we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

Keeping the Aspose tradition, you are welcome to shape the upcoming releases of Aspose.Words for Java API by posting your suggestions and concerns in the [Aspose.Words for Java Support Forum][14].




[1]: https://downloads.aspose.com/words/java/new-releases/aspose.words-for-java-19.9/
[2]: https://apireference.aspose.com/java/words/com.aspose.words/layoutoptions#TextShaperFactory
[3]: https://docs.aspose.com/display/wordsjava/How+to+Use+OpenType+Features
[4]: https://apireference.aspose.com/java/words/com.aspose.words/SdtType
[5]: https://docs.aspose.com/display/wordsjava/LINQ+Reporting+Engine+API#LINQReportingEngineAPI-AccessingXMLData
[6]: https://docs.aspose.com/display/wordsjava/LINQ+Reporting+Engine+API#LINQReportingEngineAPI-AccessingJSONData
[7]: https://docs.aspose.com/display/wordsjava/LINQ+Reporting+Engine+API#LINQReportingEngineAPI-AccessingCSVData
[8]: https://docs.aspose.com/display/wordsjava/Working+with+VBA+Macros
[9]: https://docs.aspose.com/display/wordsjava/Home
[10]: https://products.aspose.com/words/java
[11]: https://repository.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-words
[12]: https://apireference.aspose.com/java/words
[13]: https://github.com/aspose-words/Aspose.Words-for-Java
[14]: https://forum.aspose.com/c/words




