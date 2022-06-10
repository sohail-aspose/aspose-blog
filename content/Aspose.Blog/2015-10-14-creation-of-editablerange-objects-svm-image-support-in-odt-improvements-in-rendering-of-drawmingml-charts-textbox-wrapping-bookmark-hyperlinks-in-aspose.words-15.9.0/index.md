---
title: 'Creation of EditableRange Objects, SVM Image Support in ODT, Improvements in Rendering of DrawmingML Charts, Textbox Wrapping, Bookmark Hyperlinks in Aspose.Words 15.9.0'
date: Wed, 14 Oct 2015 08:45:16 +0000
draft: false
url: /2015/10/14/creation-of-editablerange-objects-svm-image-support-in-odt-improvements-in-rendering-of-drawmingml-charts-textbox-wrapping-bookmark-hyperlinks-in-aspose.words-15.9.0/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

[](http://www.aspose.com/.net/word-component.aspx)Aspose.Words 15.9.0 has been released. This month’s release contains over 94 useful new features, enhancements and bug fixes to the Aspose.Words products.

You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 15.9.0][1]
*   [Aspose.Words for Java 15.9.0][2]

Here is a look at just a few of the biggest features and API changes in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the links above.

*   Creation of EditableRange objects in DocumentBuilder
*   SVM image support in ODT
*   DrawingML textbox wrapping is now rendered correctly (while cold rendering i.e. using DmlRenderingMode.DrawingML)
*   Bookmark hyperlinks are now rendered correctly into PDF/A standard documents
*   Overlapping problem while rendering of Chinese characters into HTML Fixed format resolved
*   Improvements to DrawmingML Charts rendering

## Added Options to Control Image Stretching for LINQ Reporting Engine

WORDSNET-12077 has now been resolved and the documentation for the engine has been updated appropriately. Previously, there was a lack of documentation about using of charts with LINQ Reporting Engine, although this feature was included to 15.6 as per WORDSNET-10922. Now it is fixed. The following documentation sections were added/modified:

*   Using Charts to Represent Sequential Data
*   Inserting Images Dynamically
*   Pie Chart Template (Appendix C)
*   Scatter Chart Template (Appendix C)
*   Bubble Chart Template (Appendix C)
*   In-Table Template with Filtering, Grouping, and Ordering (Appendix C)
*   Chart Template with Filtering, Grouping, and Ordering (Appendix C)

## Added DocumentBuilder Public Methods for Creating EditableRanges

We have added following methods in DocumentBuilder class in Aspose.Words 15.9.0.

```
 /// <summary>
/// Marks the current position in the document as an editable range start.
/// </summary>
/// <remarks>
/// Editable range in a document can overlap and span any range. To create a valid editable range you need to
/// call both <see cref="StartEditableRange"/> and <see cref="EndEditableRange()"/>
/// or <see cref="EndEditableRange(EditableRangeStart)"/> methods.
/// Badly formed editable range will be ignored when the document is saved.
/// </remarks>
/// <returns>The editable range start node that was just created.</returns>
public EditableRangeStart StartEditableRange() 
```
```
 /// <summary>
/// Marks the current position in the document as an editable range end.
/// </summary>
/// <remarks>
/// Use this overload during creating nested editable ranges.
/// Editable range in a document can overlap and span any range. To create a valid editable range you need to
/// call both <see cref="StartEditableRange"/> and <see cref="EndEditableRange()"/>
/// or <see cref="EndEditableRange(EditableRangeStart)"/> methods.
/// Badly formed editable range will be ignored when the document is saved.
/// </remarks>
/// <param name="start">This editable range start.</param>
/// <returns>The editable range end node that was just created.</returns>
public EditableRangeEnd EndEditableRange(EditableRangeStart start) 
```

## Added ReportingEngine.Options Property

WORDSNET-12380 is now resolved. We have introduced following property in Aspose.Words 15.9.0.

```
 /// <summary>
/// Gets or sets a set of flags controlling behavior of this <see cref="ReportingEngine"/> instance
/// while building a report.
/// </summary>
public ReportBuildOptions Options
{
    get;
    set;
} 
```
```
 /// <summary>
/// Specifies options controlling behavior of <see cref="ReportingEngine"/> while building a report.
/// </summary>
[Flags]
public enum ReportBuildOptions
{
    /// <summary>
    /// Specifies default options.
    /// </summary>
    None = 0,
    /// <summary>
    /// Specifies that fields missing in a data source object should be treated as null literals by the engine.
    /// This option affects only fields of <ms><see cref="DataRow"/> and <see cref="IDataRecord"/> objects</ms>
    /// <java><see cref="DataTable"/> rows</java>. If this option is not set, the engine throws an exception
    /// when encounters a missing data field.
    /// </summary>
    AllowMissingDataFields = 1
} 
```




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.words-for-.net/default.aspx
[2]: http://www.aspose.com/community/files/72/java-components/aspose.words-for-java/default.aspx




