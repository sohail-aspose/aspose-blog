---
title: 'Support of Multiple Data Sources in LINQ Reporting Engine in Aspose.Words 16.5.0'
date: Fri, 24 Jun 2016 10:17:38 +0000
draft: false
url: /2016/06/24/support-of-multiple-data-dources-to-linq-reporting-engine-suppressed-endnotes-in-fixed-page-file-format-special-handling-of-backslash-for-if-fields-in-aspose.words-16.5.0/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Aspose.Words 16.5.0 has been released. This month’s release contains over 72 useful new features, enhancements and bug fixes to the Aspose.Words products. You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 16.5.0][1]
*   [Aspose.Words for Java 16.5.0][2]

Here is a look at just a few of the biggest features and API changes in this month’s release.

*   Support of Bookmark Over 40 Characters in Exported PDF.
*   Added Explicit Support of Multiple Data Sources in LINQ Reporting Engine.
*   Support of Suppressed Endnotes in Fixed Page File Format.
*   Support Special Handling of Backslash for IF Field.
*   Improved reflow performance for large paragraphs.
*   Improved SVG output with IE compatibility.
*   Improved widow/orphan handling for tables.
*   Improved Asian text line breaking in fixed page file format.

## Support of Bookmark Over 40 Characters in Exported PDF

MS Word does not allow to create bookmarks over 40 characters. In previous versions of Aspose.Words, the bookmark name is truncated when its length is more than 40 characters. We have introduced a new feature in Aspose.Words 16.5.0 to create bookmark over 40 characters long when the target document is PDF.

## Explicit Support of Multiple Data Sources in LINQ Reporting Engine

Following overload has been added to the ReportingEngine class. It allows using multiple data source objects while building a report.

```
<pre><code>/// <summary>
/// Populates the specified template document with data from the specified sources making it a ready report.
/// </summary>
/// <remarks>
/// <para>
/// Using this overload you can reference multiple data source objects and their members in the template.
/// The name of the first data source can be omitted (i.e. be an empty string or null) if you are going to
/// reference the data source's members but not the data source object itself. Names of the other data sources
/// must be specified and unique.
/// </para>
/// <para>
/// If you are going to use a single data source, consider using of <see cref="BuildReport(Document, object)"/>
/// and <see cref="BuildReport(Document, object, string)"/> overloads instead.
/// </para>
/// </remarks>
/// <param name="document">A template document to be populated with data.</param>
/// <param name="dataSources">An array of data source objects.</param>
/// <param name="dataSourceNames">An array of names to reference the data source objects within the template.</param>
public void BuildReport(Document document, object[] dataSources, string[] dataSourceNames)

``` 
```

## Support of Suppressed Endnotes in Fixed Page File Format

We have introduced a new feature in Aspose.Words 16.5.0 to suppress endnotes when the document is exported to a fixed page file format. PageSetup.SuppressEndnotes property works for only flow layout document (Word document) in previous versions of Aspose.Words. Starting from v16.5.0, this property will work for fixed page file formats e.g. Pdf, Xps.




[1]: http://downloads.aspose.com/words/net
[2]: http://downloads.aspose.com/words/java




