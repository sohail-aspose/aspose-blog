---
title: 'Automatically Track Revisions in Word Documents using C# and Java'
date: Tue, 08 Jul 2014 13:09:38 +0000
draft: false
url: /2014/07/08/track-revisions-in-word-documents-using-csharp-and-java-word-api/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Aspose.Words 14.6.0 has been released with this month’s release containing over 115 useful new features, enhancements, and bug fixes to the Aspose.Words products. You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 14.6.0][1]
*   [Aspose.Words for Java 14.6.0][2]

Here is a look at just a few of the biggest features and API changes in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the links above.

*   Support for automatic change tracking in a document.
*   Added vertical text support for HTML, EPUB, and MHT.
*   Footnote and endnote references now can be rendered as hyperlinks into output PDFs.
*   CJK (Chinese, Japanese, Korean) text is now properly rendered in multiline DrawingML textboxes.
*   Default text antialiasing on Java is optimized for Chinese, Japanese, and Korean fonts.
*   Font substitution feature is added to the public API.

## Track Revision Changes on Word Document

The following public methods were added to start and stop automatic revision tracking.

```
Document.StartTrackRevisions(string author, DateTime dateTime);
Document.StartTrackRevisions(string author);
Document.StopTrackRevisions();
```

Note that these methods have no correlation with the Document.TrackRevisions property so setting this property has no effect to Aspose.Words. Users should explicitly call the StartTrackRevision method to start automatically revision tracking in Aspose.Words.

Currently, formatting changes are not tracked. There are a few limitations in the current implementation. Revision tracking is suspended (node changes are not tracked) during the following methods:

*   Field updating - the Document.UpdateFields() method
*   Field insertion - the DocumentBuilder.InsertField() method
*   Text replace - the Range.Replace() method
*   Mail merge - the MailMerge.Execute() method.

Example code is as follows:

```
Document doc = new Document();
DocumentBuilder builder = new DocumentBuilder(doc);

builder.Writeln("hello");                    // This is not tracked

doc.StartTrackRevisions("amorozov");
builder.Writeln("message from amorozov");    // This is marked as inserted by amorozov

doc.StartTrackRevisions("ddarkin");
builder.Writeln("comment from Denis");       // This is marked as inserted by ddarkin

doc.StartTrackRevisions("rk", DateTime.Now);
doc.RemoveAllChildren();                     // Both paragraphs inserted above are marked as deleted

doc.StopTrackRevisions();

builder.Writeln("let's start it all over");  // This is not marked because tracking has been stopped.
```

## Insertion of HTML Fragments with Formatting

The InsertHtml method of the DocumentBuilder class now allows developers to choose what formatting will be used for inserted HTML fragments. A new overloaded version of InsertHtml has been added, whose argument useBuilderFormatting controls this behavior.

When useBuilderFormatting is false, which is the default, any formatting specified in DocumentBuilder is ignored, and the formatting of the inserted text is based on default HTML formatting. In this case,  the inserted text looks as in browsers.

When useBuilderFormatting is true, the formatting of the inserted text is based on the formatting specified in DocumentBuilder. Note that useBuilderFormatting chooses only the base formatting of the inserted text, and does not affect any formatting directly specified in the HTML fragment.

The following example illustrates the difference between the two modes:

```
DocumentBuilder builder = new DocumentBuilder();

builder.ParagraphFormat.LeftIndent = 72;
builder.Font.Name = "Arial";
builder.Font.Size = 24;

bool useBuilderFormatting = ...
builder.InsertHtml("<p style='color:red'><b>Text</b>", useBuilderFormatting);
```

In this example, if useBuilderFormatting is false, the inserted paragraph will have no left indent and will use the Times New Roman 12pt font, which is the default HTML font and indent. If useBuilderFormatting is true, the inserted paragraph will be indented by 1 inch (72 points) and will use the Arial 24pt font, as specified in DocumentBuilder. However, in both cases, the inserted text will be bold and red, as specified in the HTML fragment.

## Run.Font.Name Returns NameFarEast in Case of Chinese Text

Previously, we always returned the NameAscii attribute value for the public Run.Font.Name property getter. Now, the behavior is slightly changed. If the source run is of the FarEast character category then Run.Font.Name returns the NameFarEast attribute value like Microsoft Word does.

## AddFontSubstitutes, GetFontSubstitutes and SetFontSubstitutes Methods Added to FontSettings

Previously, the font substitution mechanism (the fonts to be used when a specified font is missing from the system) was hardcoded into Aspose.Words' code base and there was no way in the public API to manually customize it. Now, the following three new public static methods have been added to the FontSettings class:

```
/// <summary>
/// Adds substitute (alternative) font names for given original font name
/// </summary>
/// <param name="originalFontName">Original font name</param>
/// <param name="substituteFontNames">List of alternative font names to be used if original font is not presented in system.</param>
public static void 
```

### AddFontSubstitutes```
(string originalFontName, params string[] substituteFontNames);

/// <summary>
/// Returns array containing alternative font names to be used if original font is not presented in system.
/// </summary>
/// <param name="originalFontName">Original font name</param>
/// <returns></returns>
public static string[] 
```

### **GetFontSubstitutes**```
(string originalFontName)

/// <summary>
/// Override substitute (alternative) font names for given original font name
/// </summary>
/// <param name="originalFontName">Original font name</param>
/// <param name="substituteFontNames">List of alternative font names to be used if original font is not presented in system.</param>
public static void 
```

### SetFontSubstitutes```
(string originalFontName, params string[] substituteFontNames)
```

Now users can customize substitute fonts if needed (with default Aspose substitutes remaining).

```
FontSettings.AddFontSubstitutes("Microsoft YaHei", "MSungGB18030C-Medium");

Document doc = new Document(MyDir + "input.docx");
doc.Save(MyDir + "out.pdf");
```

## CustomPropertiesExport Property Added to PdfSaveOptions

Previously, there was an option (ExportCustomPropertiesAsMetadata) to control how document's custom properties were exported to PDF document. Now, this property is obsolete, instead, the following new property is added:

```
/// <summary>
/// Gets or sets a value determining the way <see cref="Document.CustomDocumentProperties"/> are exported to PDF file.
/// Default value is <see cref="PdfCustomPropertiesExport.None"/>
/// </summary>
public PdfCustomPropertiesExport 
```

### CustomPropertiesExport```
 { get; set; }
```

It provides new functionality - export custom properties of document to PDF as entries in /Info dictionary. The usage is as follows:

```
doc.CustomDocumentProperties.Add("prop1", true);
doc.CustomDocumentProperties.Add("prop2", 10);

PdfSaveOptions options = new PdfSaveOptions();

// Export custom properties as entries in /Info dictionary.
options.CustomPropertiesExport=PdfCustomPropertiesExport.Standard;
doc.Save("MyDocument.pdf", options);
```

Export custom properties as metadata are still available, here is how you can use this property.

```
doc.CustomDocumentProperties.Add("prop1", true);
doc.CustomDocumentProperties.Add("prop2", 10);

PdfSaveOptions options = new PdfSaveOptions();

// Export custom properties as Xmp-metadata.
options.CustomPropertiesExport=PdfCustomPropertiesExport.Metadata;
doc.Save("MyDocument.pdf", options);
```

## Render Footnote and Endnote References as Hyperlinks into PDF

Footnote and endnote references PDF rendering is now controlled by PdfSaveOptions.CreateNoteHyperlinks property. If it is set to true then footnote and endnote references in the main text story are rendered into active hyperlinks. When clicked, the hyperlink will lead to the corresponding footnote or endnote. The default value is false. The usage is described below.

```
PdfSaveOptions options = new PdfSaveOptions();

// Generate hyperlinks for footnote/endnote references
options.CreateNoteHyperlinks = true;
doc.Save(MyDir + "MyDocument.pdf", options);
```




[1]: https://downloads.aspose.com/words/net
[2]: https://downloads.aspose.com/words/java




