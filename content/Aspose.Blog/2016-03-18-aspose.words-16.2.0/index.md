---
title: 'Fast Extraction of Plain Text in Documents using C# and Java'
date: Fri, 18 Mar 2016 15:06:23 +0000
draft: false
url: /2016/03/18/aspose.words-16.2.0/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Aspose.Words 16.2.0 has been released. This month’s release contains over 103 useful new features, enhancements and bug fixes to the Aspose.Words products.

You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 16.2.0][1]
*   [Aspose.Words for Java 16.2.0][2]

Here is a look at just a few of the biggest features and API changes in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the links above.

*   Support of Fast Extraction of Plain Text from flow-format Documents
*   Support of Axis Logarithmic Scale
*   Introduced PageSavingCallback for all fixed-page Save Formats
*   Introduced Paragraph.IsFormatRevision and Inline.IsFormatRevision Properties
*   Introduced Shape.Title Property to Get-Set Alt Text Title Property of Shape
*   Improved Font substitution

## Fast Extraction of Plain Text from flow-format Documents

We have introduced static Document.ExtractText methods to extracts text information from flow-format document.

```
public class Document
{
 ....
 public static PlaintextDocument ExtractText(string fileName)
 public static PlaintextDocument ExtractText(string fileName, LoadOptions loadOptions)
 public static PlaintextDocument ExtractText(Stream stream)
 public static PlaintextDocument ExtractText(Stream stream, LoadOptions loadOptions)
 ....
}
```
```
/// <summary>
/// Contains plain-text representation of the document's content as extracted by  and alike.
/// </summary>
public class PlaintextDocument
{
 public string Text {get;}
 public BuiltInDocumentProperties BuiltInDocumentProperties {get;}
 public CustomDocumentProperties CustomDocumentProperties {get;}
}
```

## Support of Axis Logarithmic Scale

Starting from 16.2.0 version, Aspose.Words supports axis logarithmic scale upon rendering DML chart.



{{< figure align=center src="images/LogScale.png" alt="">}}


## PageSavingCallback for all fixed-page Save Formats

We have introduced PageSavingCallback property for all fixed-Page based save formats. PageSavingCallback allows to control how separate pages are saved when a document is exported to fixed-page based save formats. You are able to control PageFileName for each separate page. You can also specify the stream where the document page will be saved using PageStream property.

```
/// <summary>
/// Custom PageFileName is specified.
/// </summary>
private class CustomPageFileNamePageSavingCallback : IPageSavingCallback
{
    public void PageSaving(PageSavingArgs args)
    {
        // Specify name of the output file for the current page.
        args.PageFileName = string.Format(@"C:\Temp\Page_{0}.html", args.PageIndex);
    }
}
```

PageSavingCallback is available for the following classes:

*   HtmlFixedSaveOptions
*   ImageSaveOptions
*   PdfSaveOptions
*   PsSaveOptions
*   SvgSaveOptions
*   SwfSaveOptions
*   XamlFixedSaveOptions
*   XpsSaveOptions

## Paragraph.IsFormatRevision and Inline.IsFormatRevision Properties

We have introduced Paragraph.IsFormatRevision and Inline.IsFormatRevision properties to check either the formatting of the object was changed in Microsoft Word while change tracking was enabled or not.

```
/// <summary>
/// Returns true if this object was formatted in Microsoft Word while change tracking was enabled.
/// </summary>
public bool IsFormatRevision { get; }
```

## Shape.Title Property to Get-Set Alt Text Title Property of Shape

Starting from 16.2.0 version, Aspose.Words starts supporting Alt Text Title. In case of older format conversion MS Word formats following string "Title: titleText - Description: descText", if there is no description "Title: titleText", if there is no title then just "descText". Aspose.Words does the same now. You can also get/set shape title like this:

```
Node[] shapes = doc.GetChildNodes(NodeType.Shape, true).ToArray();

Shape shape0 = (Shape)shapes[0];

// Get shape title.
Console.WriteLine(shape0.Title);

// Set new shape title.
shape0.Title = "New Shape Title"; 
```

## Improved Font Substitution

Font substitution improved to mimic MS Word in case when font info in the document doesn't contains the PANOSE. Previously, in this case, Aspose.Words used to substitute fonts with FontSettings.DefaultFontName. In case when PANOSE is specified in font info, Aspose.Words still uses FontSettings.DefaultFontName.

Warning is issued with text: "Font '' has not been found. Using '' font instead. Reason: closest match according to font info from the document."




[1]: https://downloads.aspose.com/words/net
[2]: https://downloads.aspose.com/words/java




