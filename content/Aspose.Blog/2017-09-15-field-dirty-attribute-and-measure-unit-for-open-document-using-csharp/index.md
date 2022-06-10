---
title: 'Field Dirty Attribute and Measure Unit for Open Document using C#'
date: Fri, 15 Sep 2017 11:34:18 +0000
draft: false
url: /2017/09/15/field-dirty-attribute-and-measure-unit-for-open-document-using-csharp/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

We are pleased to announce our next version [Aspose.Words for .NET 17.9][1]. This month’s release contains over 76 useful new features, enhancements and bug fixes. Please see the [release notes][2] for more detail. If you are planning to upgrade from older version of Aspose.Words to the current version, we would strongly suggest you to check the [Public API and Backward Incompatible Changes][3] section to know what APIs are changed so far.

Here is a look at just a few of the biggest features and API changes in this month’s release.

*   Caching of shading patterns for PDF output implemented. The output size of PDF documents with the repeating images (e.g. in header/footer) is now significantly reduced.
*   Precaching of printer settings implemented. Calling of AsposeWordsPrintDocument.CachePrinterSettings() reduces the time for the first call of Print() method making the sequential calls of Print() method uniform. Metafiles with EMR\_ALPHABLEND record with 32bpp ARGB raw bitmap data rendering implemented.
*   Improved character spacing control handling for Asian text.
*   Improved table grid calculation when a paragraph in a cell has large indents.
*   Improved text wrapping in narrow line band when there is a leading tab stop.
*   Added feature to set Placeholder Text of Structured Document Tag.
*   Added feature to support w:dirty attribute on a field.
*   Updating value of SaveDate field just by doing open/save.

## Added Feature to Support Dirty Attribute of Field

We have added three public properties in this version of Aspose.Words related to the dirty (stale) state of the fields and controlling whether such fields should be updated.  
Please read following article for more detail:  
[Update Fields having Dirty Attribute][4]

LoadOptions:

```
/// <summary>
/// Specifies whether to update the fields with the <c>dirty</c> attribute.
/// </summary>
public bool UpdateDirtyFields 
```

Field:

```
/// <summary>
/// Gets or sets whether the current result of the field is no longer correct (stale) // due to other modifications made to the document.
/// </summary>
public bool IsDirty
```

FieldChar:

```
/// <summary>
/// Gets or sets whether the current result of the field is no longer correct (stale) // due to other modifications
/// made to the document.
/// </summary>
public bool IsDirty
```

## Added Feature to Set Measure Unit for Open Document

A new feature has been added in this release to specify unit of measure apply to open document content. The OdtSaveOptions.MeasureUnit property is added for this purpose. You can set measure unit as Centimeters or Inches. Please read more detail from here:  
[Specify Unit of Measure to OpenDocument][5]

```
 /// <summary>
/// Allows to specify units of measure to apply to document content.
/// The default value is <see cref="OdtSaveMeasureUnit.Centimeters"/>
/// </summary>
/// <remarks>
/// Open Office uses centimeters when specifying lengths, widths and other measurable /// formatting and content properties in documents whereas MS Office uses inches.
///</remarks>
public OdtSaveMeasureUnit MeasureUnit
```

## Added Feature to Reduce Time of First Call of Print() Method

We have added public method AsposeWordsPrintDocument.CachePrinterSettings in this version of Aspose.Words to reduce time of first call of Print() method. Please refer to the following article for more detail.  
[How to Reduce Time of First Call of Print][6]

```
/// <summary>
/// Reads and caches some fields of <see cref="PrinterSettings"/>
/// to reduce printing time.
/// </summary>
/// <remarks>
/// This method is called before the printing starts if it wasn't executed previously.
/// </remarks>
public void CachePrinterSettings()
```

## Added feature to Clear Contents of Content Control

We have added new feature in this release to clear the contents of structured document tag and displays a placeholder if it is defined. The StructuredDocumentTag.Clear method has added for this purpose.

```
/// <summary>
/// Clears contents of this structured document tag and displays a placeholder /// if it is defined.
/// </summary>
public void Clear()
```

## Added Public Property List.IsRestartAtEachSection

We have added public property IsRestartAtEachSection in List class to support backward compatibility upon Mail Merge. In previous versions of Aspose.Words, if the mail merge template document contains numbered list, the numbers are not restarted for each section. You can use this property to restart list at each section. Please read following article and check the code snippet given below.  
[How to Restart List for each Section][7]

```
Dictionary<List, bool> lists = new Dictionary<List, bool>();
 
foreach (List list in document.Lists)
    lists[list] = list.IsRestartAtEachSection;
 
document.MailMerge.Execute(...);
 
foreach (KeyValuePair<List, bool> pair in lists)
    pair.Key.IsRestartAtEachSection = pair.Value 
```

## Added SaveOptions.UpdateLastSavedTimeProperty Property

We have added the SaveOptions.UpdateLastSavedTimeProperty in Aspose.Words for .NET 17.9 that controls whether to update the corresponding built-in document property on document save. Please read more detail from here:  
[Update LastSavedTime Property Before Saving][8]

```
/// <summary>
/// Gets or sets a value determining whether the <see cref="BuiltInDocumentProperties.LastSavedTime" /> /// property is updated before saving.
/// </summary>
public bool UpdateLastSavedTimeProperty
```

## Aspose.Words for .NET Resources

The following resources will help you work with Aspose.Words for .NET:

*   [Home page of .NET API][9].
*   [Download Section][10].
*   [Install using NuGet Package][11]
*   [Documentation][12] – up-to-date documentation containing Programmer’s Guide, Knowledge Base and much more.
*   [API Reference Guide][13] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   Aspose.Words Product Family Forum – post your technical questions and queries, or any other problem you are facing while working with Aspose.Words APIs.
    *   [Free Support Forum][14]
    *   [Paid Support Forum][15]
*   [Enable Blog Subscription][16] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
*   [Examples][17] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/words/net/new-releases/aspose.words-for-.net-17.9/
[2]: https://docs.aspose.com/words/net/aspose-words-for-net-17-9-release-notes/
[3]: https://docs.aspose.com/words/net/aspose-words-for-net/
[4]: https://docs.aspose.com/words/net/updating-and-removing-a-field/#UpdatingandRemovingaField-UpdateFieldshavingDirtyAttribute
[5]: https://docs.aspose.com/words/net/saving-a-document/#SavingaDocument-SpecifyUnitofMeasuretoOpenDocument
[6]: https://docs.aspose.com/words/net/print-a-document-programmatically-or-using-dialogs/#PrintaDocument-HowtoReduceTimeofFirstCallofPrint
[7]: https://docs.aspose.com/words/net/working-with-lists/#WorkingWithLists-HowtoRestartListforeachSection
[8]: https://docs.aspose.com/words/net/updating-and-removing-a-field/#UpdatingandRemovingaField-UpdateLastSavedTimePropertyBeforeSaving
[9]: https://www.aspose.com/products/words/net
[10]: https://downloads.aspose.com/words/net
[11]: https://www.nuget.org/packages/Aspose.Words/
[12]: https://docs.aspose.com/display/wordsnet
[13]: https://apireference.aspose.com/net/words
[14]: https://forum.aspose.com/c/words
[15]: https://helpdesk.aspose.com/
[16]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[17]: https://github.com/aspose-words/Aspose.Words-for-.NET




