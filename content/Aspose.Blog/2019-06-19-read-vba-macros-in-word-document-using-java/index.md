---
title: 'Read VBA Macros in Word Document using Aspose.Words for Java 19.6'
date: Wed, 19 Jun 2019 09:47:34 +0000
draft: false
url: /2019/06/19/read-vba-macros-in-word-document-using-java/
author: Awais Hafeez
summary: ''
tags: ['Get access to the VBA project Word documents using Java']
categories: ['Aspose.Words Product Family']
---

In this post, I will enlist/explain new features introduced in [Aspose.Words for Java 19.6][1] release.

## Access/Read VBA Macros from Word Document using Java

Aspose.Words now provides three classes to get access to the VBA project source code. The [VBAProject class][2] provides access to VBA project information, the [VbaModuleCollection class][3] returns collection of VBA project modules and [VbaModule class][4] provides access to the VBA project module. The code example given below shows how to read VBA Macros from the Word document:

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-loading_saving-WorkingWithVbaMacros-ReadVbaMacros.java" >}}

## Convert to Horizontally Merged Table Cells

In the latest versions of MS Word, Table cells are merged horizontally by their width. Whereas, the merge flags were used in the older technique, like [Cell.CellFormat.HorizontalMerge][5]. The merge flags are not used when cells are horizontally merged by their width and it is also not possible to detect which cells are merged. Aspose.Words now provides [ConvertToHorizontallyMergedCells method][6] to convert cells which are horizontally merged by their widths to the cell horizontally merged by flags. It simply transforms the table and adds new cells when needed.

The following code example shows the working of the above-mentioned method.

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-programming_documents-tables-ColumnsAndRows-ConvertToHorizontallyMergedCells-ConvertToHorizontallyMergedCells.java" >}}

## Compress Metafiles in Word Document

In MS Word, all the metafiles are compressed by default regardless of their size. However, Aspose.Words used to compress large metafiles only and smaller ones were not compressed just because of better performance. Aspose.Words now provides a property [AlwaysCompressMetafiles][7], to facilitate the users if they want to compress all the metafiles either large or small. Its default value is true which means that all metafiles shall be compressed regardless of their sizes and false means that small metafiles shall not be compressed for performance reason.

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-loading_saving-WorkingWithDocSaveOptions-AlwaysCompressMetafiles.java" >}}

## Working with Table Styles

You can change the format of Table by using Table styles in MS Word. With Table style, you can change the look of Table e.g. border, shading, alignment, text font etc. In this release of Aspose.Words, new public properties have been added into the [TableStyle class][8]. We have implemented new public types [ConditionalStyleCollection][9], [ConditionalStyle][10], and [ConditionalStyleType][11]. Please read the following article for more details.

[Working with Table Styles][12]

## License.IsLicensed Marked as Obsolete

Starting from Aspose.Words 19.6, the License.IsLicensed property is marked as obsolete. We will remove it in later releases

```
/// <summary>
/// Returns true if a valid license has been applied; false if the component is running in evaluation mode.
/// </summary>
[Obsolete("This property is obsolete. SetLicense() method raises an exception if license is invalid.")]
public bool IsLicensed
```

## Obsolete methods Range.Replace Removed

We have removed the following Range.Replace methods from Aspose.Words API.

```
public int Replace(string pattern, string replacement)
public int Replace(string pattern, string replacement, FindReplaceOptions options)
public int Replace(Regex pattern, string replacement)
public int Replace(Regex pattern, string replacement, FindReplaceOptions options)
```

## See also Useful Links

*   [Aspose.Words for Java Online Documentation][13] - up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Words for Java Product Page][14]
*   [Install Aspose.Words for Java from Maven][15]
*   [Aspose.Words for Java API Reference Guide][16] - detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Download Examples at GitHub Repository][17] - we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

Keeping the Aspose tradition, you are welcome to shape the upcoming releases of Aspose.Words for Java API by posting your suggestions and concerns in the [Aspose.Words for Java Support Forum][18].




[1]: https://downloads.aspose.com/words/java/new-releases/aspose.words-for-java-19.6/
[2]: https://apireference.aspose.com/java/words/com.aspose.words/VbaProject
[3]: https://apireference.aspose.com/java/words/com.aspose.words/VbaModuleCollection
[4]: https://apireference.aspose.com/java/words/com.aspose.words/VbaModule
[5]: https://apireference.aspose.com/java/words/com.aspose.words/cellformat#HorizontalMerge
[6]: https://apireference.aspose.com/java/words/com.aspose.words/table#convertToHorizontallyMergedCells()
[7]: https://apireference.aspose.com/java/words/com.aspose.words/docsaveoptions#AlwaysCompressMetafiles
[8]: https://apireference.aspose.com/java/words/com.aspose.words/TableStyle
[9]: https://apireference.aspose.com/java/words/com.aspose.words/ConditionalStyleCollection
[10]: https://apireference.aspose.com/java/words/com.aspose.words/ConditionalStyle
[11]: https://apireference.aspose.com/java/words/com.aspose.words/ConditionalStyleType
[12]: https://docs.aspose.com/display/wordsjava/Working+with+Table+Styles
[13]: https://docs.aspose.com/display/wordsjava/Home
[14]: https://products.aspose.com/words/java
[15]: https://repository.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-words
[16]: https://apireference.aspose.com/java/words
[17]: https://github.com/aspose-words/Aspose.Words-for-Java
[18]: https://forum.aspose.com/c/words




