---
title: 'ODT Charts Rendering Supported, Paragraph.InsertField Overloads Added, Fixed Table Grid Calculation and many other Improvements Added in Aspose.Words 15.8.0'
date: Sun, 06 Sep 2015 09:30:27 +0000
draft: false
url: /2015/09/06/odt-charts-rendering-supported-paragraph.insertfield-overloads-added-fixed-table-grid-calculation-and-many-other-improvements-added-in-aspose.words-15.8.0/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

[](http://www.aspose.com/.net/word-component.aspx)Aspose.Words 15.8.0 has been released. This month’s release contains over 98 useful new features, enhancements and bug fixes to the Aspose.Words products.

You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 15.8.0][1]
*   [Aspose.Words for Java 15.8.0][2]

Here is a look at just a few of the biggest features and API changes in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the links above.

*   New functionality similar to ADO.NET was added to increase the number of MailMerge and Reporting data sources.
*   Implemented fixed table grid calculation.
*   Improved footnote balancing.
*   Supported roundtrip of ruby a.k.a phonetic guide in flow formats. Limited support for rendering to PDF is also provided.
*   EMF+ rendering is improved (line caps and shadows).
*   ODT Charts rendering implemented.
*   CustomXmlMarkup fully removed from the code.
*   Allow to specify encoding when saving as HTML.

## Paragraph.InsertField Method Overloads Added

WORDSNET-12080 is now resolved. We have added following overloads of Paragraph.InsertField method. These methods allow inserting a field into an arbitrary point in the paragraph:

```
 public Field InsertField(FieldType,bool,Node,bool);
public Field InsertField(string,Node,bool);
public Field InsertField(string,string,Node,bool); 
```

## OutlineOptions.CreateMissingOutlineLevels Property Added

CreateMissingOutlineLevels property is added to OutlineOptions class. Default value for this property is false:

```
 /// <summary>
/// <para>Gets or sets a value determining whether or not to create missing heading levels when the document is
/// exported.</para>
/// <para>Default value for this property is <b>false</b></para>
/// </summary>
public bool CreateMissingOutlineLevels { get;set; } 
```

## HtmlFixedSaveOptions.Encoding Property Added

WORDSNET-12178 is now resolved. We have introduced following property in Aspose.Words 15.8.0.

```
 /// <summary>
/// Specifies the encoding to use when exporting to HTML.
/// Default value is <ms><c>new UTF8Encoding(true)</c> (UTF-8 with BOM)</ms><java>'UTF-8' Charset</java>.
/// </summary>
/// <javaName>Encoding(java.nio.charset.Charset)</javaName>
public Encoding Encoding { get; set; } 
```

## CustomXmlMarkup Support Fully Removed from Aspose.Words Code

We used to keep CustomXmlMarkup nodes marked as Obsolete, but now it is fully removed as per:

[Custom XML markup is removed when you open a document in Word 2013][3]

## ODT Charts Rendering Supported

WORDSNET-10052 is now resolved. Starting from 15.8.0 version of Aspose.Words, it supports rendering of ODT charts upon saving to fixed page formats. Also chart is rendered to image and is displayed when save to flow formats other than ODT and OTT. Still this is the first version of this feature and some features of charts are not supported upon rendering. Currently axis titles, trend lines, error bars are not supported, also stock and surface charts are not fully supported. These features will be supported in the future versions of Aspose.Words.




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.words-for-.net/default.aspx
[2]: http://www.aspose.com/community/files/72/java-components/aspose.words-for-java/default.aspx
[3]: http://support.microsoft.com/kb/2761189




