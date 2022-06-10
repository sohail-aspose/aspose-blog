---
title: 'Read Macros from Word Documents using C#'
date: Fri, 14 Jun 2019 16:29:14 +0000
draft: false
url: /2019/06/14/compress-metafiles-read-macros-from-document-improved-table-style-and-convert-wide-cell-to-horizontally-merged-cells/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose-Words-for-net.png" alt="Aspose.Words for .NET logo">}}


Hi guys! We have added very interesting features for you in the new release of [Aspose.Words for .NET 19.6][1]. Reading macros from the document, control the behavior of compressing metafiles while saving document, working with table styles, and convert wide cell to horizontally merged cell.

Let me explain the detail of each feature one by one.

**TIP**

You may want to check out **Aspose** [FREE macro removal web app][2].

## Read Macros from Document using C#

In this release, we have added support to read the VBA project source code. We have added [VbaProject][3], [VbaModuleCollection][4], and [VbaModule][5] classes in this release. Below code example shows how to read VBA Macros from the document.

{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Loading-and-Saving-WorkingWithVbaMacros-ReadVbaMacros.cs" >}}

## Compress Metafiles using C#

When you save Word document using MS Word, all metafiles are compressed by default regardless of their size. However, Aspose.Words compresses big size metafiles only. The small size metafiles are not compressed for performance reason. Starting from Aspose.Words 19.6, we have added new feature to allow users to choose an appropriate behavior using new public property [DocSaveOptions.AlwaysCompressMetafiles][6]. All meta files are compressed regardless of its size when this property has **true** value. When **false**, small meta files are not compressed. Following code example shows how to use this property.

{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Loading-and-Saving-WorkingWithDoc-AlwaysCompressMetafiles.cs" >}}

## Working with Table Style

You can change the format of table using Table styles in MS Word. With table style, you can change the look of table e.g. border, shading, alignment, text font etc. In this release of Aspose.Words, new public properties have been added into the [TableStyle][7] class. We have implemented new public types ConditionalStyleCollection, ConditionalStyle, and ConditionalStyleType. Please read the following article for more detail.

[Working with TableStyle][8]

## Added Public Method Table.ConvertToHorizontallyMergedCells

There are two well-known techniques used by MS Word to implement horizontally merged cells inside the table. The first one is the [merge flags][9], like Cell.CellFormat.HorizontalMerge, but according to the latest MS Word behavior looks like this way is not used anymore and MS Word just does not write merge flags. Instead, MS Word uses another technique, where cells are merged horizontally by its width.

So, when cells are horizontally merged by its width – there are no merge flags and of course, there is no way to use merge flags to detect which cells are merged. So, we have added a new public method to convert cells which are horizontally merged by its width to the cell horizontally merged by flags. Please read the following article.

[Convert To Horizontally Merged Cells][10]

## Obsolete methods Range.Replace removed

We have removed following Range.Replace methods in this release.

```
public int Replace(string pattern, string replacement)
public int Replace(string pattern, string replacement, FindReplaceOptions options)
public int Replace(Regex pattern, string replacement)
public int Replace(Regex pattern, string replacement, FindReplaceOptions options)
```

## License.IsLicensed Marked as Obsolete

Starting from Aspose.Words 19.6, the License.IsLicensed property is marked as obsolete. We will remove it in later releases.

```
/// <summary>
/// Returns true if a valid license has been applied; false if the component is running in evaluation mode.
/// </summary>
[Obsolete("This property is obsolete. SetLicense() method raises an exception if license is invalid.")]
public bool IsLicensed
```

There are many other features, enhancement, and bug fixes included in this release. Please check the release notes of [Aspose.Words for .NET 19.6][11].

When time allows you can check Aspose.Words' API [examples at Github][12], talk about this release and other API related issues in our [forum][13].




[1]: https://www.nuget.org/packages/Aspose.Words/19.6.0
[2]: https://products.aspose.app/slides/remove-macros
[3]: https://apireference.aspose.com/
[4]: https://apireference.aspose.com/
[5]: https://apireference.aspose.com/
[6]: https://apireference.aspose.com/net/words/aspose.words.saving/docsaveoptions/properties/alwayscompressmetafiles
[7]: https://apireference.aspose.com/net/words/aspose.words/tablestyle
[8]: https://docs.aspose.com/display/wordsnet/Working+with+TableStyle
[9]: https://docs.aspose.com/display/wordsnet/Working+with+Columns+and+Rows#WorkingwithColumnsandRows-MergedCellsinAspose.Words
[10]: https://docs.aspose.com/display/wordsnet/Working+with+Columns+and+Rows#WorkingwithColumnsandRows-ConvertToHorizontallyMergedCells
[11]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+19.6+Release+Notes
[12]: https://github.com/aspose-words/Aspose.Words-for-.NET
[13]: https://forum.aspose.com/c/words




