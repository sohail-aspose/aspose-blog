---
title: 'Insert Document within a Word Document using LINQ Reporting Engine in C# and Java'
date: Fri, 15 Jul 2016 11:16:06 +0000
draft: false
url: /2016/07/15/insert-outer-document-within-a-word-document-using-csharp-and-java/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Aspose.Words 16.6.0 has been released. This month’s release contains over 113 useful new features, enhancements and bug fixes to the Aspose.Words products.

You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 16.6.0][1]
*   [Aspose.Words for Java 16.6.0][2]

Here is a look at just a few of the biggest features and API changes in this month’s release.

*   Added Support for Outer Document Insertion to LINQ Reporting Engine
*   Fast Extraction from DOC Format via PlainTextDocument Class is Faster by a Factor of Ten (at a cost)
*   RevisionOptions has ShowRevisionBalloons Option now
*   Saving DOCX as ISO 29500 Strict OOXML Format is Available now
*   Added Feature to Insert Empty Values in Chart Series.
*   Added MailMergeRegionInfo.Level Property
*   Added MailMerge.GetRegionsByName() Method
*   XpsSaveOptions.OptimizeOutput Option Added
*   Field.GetFieldCode() Improved, Added Field.GetFieldCode() Overload

## Outer Document Insertion with LINQ Reporting Engine

We have introduced a new feature in Aspose.Words 16.6.0 to insert document dynamically after populating it with data using LINQ Reporting Engine. Detail of this feature is available in the following documentation link.

*   [Inserting Documents Dynamically using LINQ Reporting Engine][3]

## Fast Extraction from DOC Format

We've improved the speed of the fast text indexing method for DOC format available via public API as [PlainTextDocument][4]. However to do this a special DOC reader had to be written which only guarantees the order of plain text within a story upon reading. This means that document sections may be swapped around, and their order is not guaranteed. However, the order of paragraphs words and so forth within is section will be as usual.

## Rendering Format Changes in the Balloons

We have introduced new feature in Aspose.Words 16.6.0 to render format changes in balloons. ShowRevisionBalloons property has been added to the RevisionOptions class. This option lets a user show formatting changes in the balloons. NOTE: Now it works only for delete revisions.

```
/// <summary>
/// Allows to specify whether the formatting changes are rendered in the balloons.
/// Default value for this property is <c>false</c>.
/// <remarks>
/// <para>
/// Only works for <see cref="RevisionType.Deletion"/>.
/// For <see cref="RevisionType.FormatChange"/> and <see cref="RevisionType.Insertion"/> is not supported yet.
/// </para>
/// </remarks>
/// </summary>
public bool ShowRevisionBalloons
{
    get { return mShowRevisionBalloons; }
    set
    {
        mHasChanged = true;
        mShowRevisionBalloons = value;
    }
}
```
```
Document doc = new Document(@"Document.docx"); 
doc.LayoutOptions.RevisionOptions.ShowRevisionBalloons = true; 
string outFileName = (@"Out.pdf"); 
doc.Save(outFileName);
```

## Saving DOCX as ISO 29500 Strict OOXML Format

We have introduced new feature in Aspose.Words 16.6.0 to save Document to ISO 29500 Strict OOXML Format. A new member Iso29500\_2008\_Strict is added into the OoxmlCompliance enum type. UseCase to save as Strict OOXML.

Limitations:

```
Document doc = new Document();
OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
saveOptions.Compliance = OoxmlCompliance.Iso29500_2008_Strict;
doc.Save(@"C:\MyDir\strict_OOXML.docx", saveOptions);
```

*   ISO 29500 Strict forbids VML, so we had to do a quick conversion hack by rendering VML shapes into pictures and storing them as DML Pictures. Proper VML->DML conversion is a big task without an ETA.
*   Testing has been done on documents mostly from our TestBase, so Support people please be prepared to receive a number of non-conformant, non-compliant and generally bad smelling documents that will violate our model assumptions in one way or another.

## Insert Empty Values in Chart Series

Starting from Aspose.Wrods v16.6.0, Aspose.Words supports empty values in chart data series and categories upon creating. The following code example explains this feature.

*   **double.NaN** value is used as empty data value.
*   **null** is used as empty category name.

```
// Add chart with default data.
Shape shape = builder.InsertChart(ChartType.Line, 432, 252);
Chart chart = shape.Chart;

ChartSeriesCollection seriesColl = chart.Series;
seriesColl.Clear();

// Create category names array, second category will be null.
string[] categories = new string[] { "Cat1", null, "Cat3", "Cat4", "Cat5" };

// Adding new series with empty (double.NaN) values.
seriesColl.Add("AW Series 1", categories, new double[] { 1, 2, double.NaN, 4, 5 });
seriesColl.Add("AW Series 2", categories, new double[] { 2, 3, double.NaN, 5, 6 });
seriesColl.Add("AW Series 3", categories, new double[] { double.NaN, 4, 5, double.NaN, double.NaN }); 
```

## Added MailMergeRegionInfo.Level Property

We have added the MailMergeRegionInfo.Level property in Aspose.Wrods v16.6.0 to get the nesting level for the region.

```
/// <summary>
/// Returns a collection of mail merge regions with given name.
/// </summary>
public bool OptimizeOutput
```

## XpsSaveOptions.OptimizeOutput Option Added

We have added the XpsSaveOptions.OptimizeOutput property in Aspose.Wrods v16.6.0. When this property is set to true, redundant nested canvases and empty canvases are removed, also neighbor glyphs with the same formatting are concatenated.

```
/// <summary>
/// Flag indicates whether it is required to optimize output of XPS.
/// If this flag is set redundant nested canvases and empty canvases are removed,
/// also neighbor glyphs with the same formatting are concatenated.
///
/// Default is false.
/// </summary>
public bool OptimizeOutput
```




[1]: http://www.aspose.com/downloads/words-family/net
[2]: http://www.aspose.com/downloads/words-family/java
[3]: https://docs.aspose.com/display/wordsnet/Template+Syntax#TemplateSyntax-InsertingDocumentsDynamically
[4]: https://apireference.aspose.com/words/net/aspose.words/plaintextdocument




