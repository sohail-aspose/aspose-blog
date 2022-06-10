---
title: 'Create and Modify VBA Macros in Word Documents using C#'
date: Fri, 20 Sep 2019 09:13:39 +0000
draft: false
url: /2019/09/20/create-and-modify-vba-macros-in-word-doc-docx-using-csharp-word-library/
author: Tahir Manzoor
summary: ''
tags: ['Create and Modify VBA Macros in Word using Csharp']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose-Words-for-net.png" alt="Aspose.Words for .NET logo">}}


It is our pleasure to announce the September release of [Aspose.Words for .NET][1]. We have included quite exciting features and enhancements in this release. Now, you can generate reports using LINQ Reporting with data sources like XML, JSON, and CSV. Working with VBA macro code, programmatically create repeating section content control, link custom document property to bookmark and many other features have been included in this release. let’s check out what this release offers and how to use newly introduced features.

**TIP**

You may want to check out **Aspose** [FREE macro removal web app][2].

## Create and Modify VBA Macros in Word Documents using C#

A new property VbaModule.SourceCode has been added in this release to get or set VBA project module source code. The following code example demonstrates how to modify VBA Macros using the VbaModule.SourceCode property.

{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Loading-and-Saving-WorkingWithVbaMacros-ModifyVbaMacros.cs" >}}

## Create Repeating Section Content Control in Word Document

MS Word allows you to insert the repeating content control with XML mapping in Word document. You can insert repeating content control around entire paragraphs or table rows. We have added this feature in the latest release of Aspose.Words. A new enumeration type _RepeatingSectionItem_ has been added in this release.

{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Programming-Documents-StructuredDocumentTag-WorkingWithSDT-CreatingTableRepeatingSectionMappedToCustomXmlPart.cs" >}}

Please read the following article for more detail.

*   [Working with Repeating Section Content Control][3]

## LINQ Reporting with XML, JSON, and CSV Data Sources

As you know, LINQ Reporting Engine enables you to build reports using an extended set of reporting features. The engine enables you to reference business objects of your application in report templates. We have added XmlDataSource, JsonDataSource, and CsvDataSource classes in this release to use XML, JSON, and CSV as data sources to generate reports using LINQ Reporting. Please read the following articles for complete detail of this feature.

*   [Accessing XML Data][4]
*   [Accessing JSON Data][5]
*   [Accessing CSV Data][6]

## Link Custom Document Property to Bookmark

MS Word allows you to link custom document property to a bookmark. In MS Word, you can check this option under document properties dialog. In this release, we have added LinkSource and IsLinkToContent properties in DocumentProperty class and a method AddLinkToContent in CustomDocumentProperties class. The following code example shows how to link custom document property to a bookmark.

{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Programming-Documents-Document-DocProperties-ConfiguringLinkToContent.cs" >}}

## Remove License.IsLicensed property

The License.IsLicensed obsolete property has been removed in order to increase anti-hacking resistance. Moreover, this property was useless because of the License.SetLicense method. This method throws an exception in case of a wrong license key.

## Introduced SavePictureBullet option for MS Word 97 Document

We have added DocSaveOptions.SavePictureBullet property in this release to work with PictureBullet data. This option is provided for MS Word 97 which cannot work correctly with PictureBullet data. Please set this option to "false" to remove PictureBullet data.

We recommend you please check the release notes of [Aspose.Words for .NET 19.9][7] for complete detail of API changes.

When time allows you can check Aspose.Words' [API reference guide][8], [examples at Github][9], talk about this release and other API related issues in our [forum][10].




[1]: https://www.nuget.org/packages/Aspose.Words/19.9.0
[2]: https://products.aspose.app/slides/remove-macros
[3]: https://docs.aspose.com/display/wordsnet/Working+with+Content+Control+SDT#WorkingwithContentControlSDT-WorkingwithRepeatingSectionContentControl
[4]: https://docs.aspose.com/display/wordsnet/LINQ+Reporting+Engine+API#LINQReportingEngineAPI-AccessingXMLData
[5]: https://docs.aspose.com/display/wordsnet/LINQ+Reporting+Engine+API#LINQReportingEngineAPI-AccessingJSONData
[6]: https://docs.aspose.com/display/wordsnet/LINQ+Reporting+Engine+API#LINQReportingEngineAPI-AccessingCSVData
[7]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+19.9+Release+Notes
[8]: https://apireference.aspose.com/net/words
[9]: https://github.com/aspose-words/Aspose.Words-for-.NET
[10]: https://forum.aspose.com/c/words




