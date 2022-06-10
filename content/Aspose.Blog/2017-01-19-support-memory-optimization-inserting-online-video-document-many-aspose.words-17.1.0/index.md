---
title: 'Insert Online Video into Word Document using C# and Java APIs'
date: Thu, 19 Jan 2017 06:59:59 +0000
draft: false
url: /2017/01/19/support-memory-optimization-inserting-online-video-document-many-aspose.words-17.1.0/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Aspose.Words 17.1.0 has been released. This month’s release contains over 80 useful new features, enhancements and bug fixes.

You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 17.1.0][1]
*   [Aspose.Words for Java 17.1.0][2]

Here is a look at just a few of the biggest features and API changes in this month’s release.

*   Added public API to insert online video via DocumentBuilder.InsertOnlineVideo
*   Added TxtSaveOptions.ForcePageBreaks public property
*   Added SaveOptions.MemoryOptimization public property
*   New public API class FrameFormat available in Paragraph.FrameFormat
*   Support for DOCX roundtrip of multiple MS Word 2013 native document options added
*   Supported DOCX roundtrip of Effect Container element
*   DOCX Roundtrip of Extension lists suppororted for Charts and other graphics
*   Shape texture brush with EMF image rendering implemented
*   Shape positioning inside tables precision improved
*   Implemented support for 'FitText' attribute
*   Improved space shrink logic for Asian text
*   Improved Unicode normalization performance during layout
*   Improved handling of invalid hyphenation dictionaries
*   Improved handling of collapsed table rows
*   Improved extracting document outline when TOC headings contain hidden entries
*   Fixed positioning issue with Arabic list labels
*   Fixed height issue with LTR list labels in RTL paragraphs

## Insert Online Videos in Word Documents

Starting from 17.1.0 version, Aspose.Words supports inserting an online video into the document. Four overloads of [InsertOnlineVideo][3] method have introduced in DocumentBuilder class.

The first one works with the most popular video resources and takes the URL to the video as parameter.   
_Note : This feature is only available in Aspose.Words for .NET._

```
DocumentBuilder builder = new DocumentBuilder(doc);
 
// Pass direct url from youtu.be.
string url = "https://youtu.be/t\_1LYZ102RA";
 
double width = 360;
double height = 270;
 
Shape shape = builder.InsertOnlineVideo(url, width, height);

```

Simple insertion of online video from the following resources is supported:

\- https://www.youtube.com/  
\- https://vimeo.com/

The second overload works with all other video resources and takes embed Html code as parameter:

```
DocumentBuilder builder = new DocumentBuilder(doc);
 
// Shape width/height.
double width = 360;
double height = 270;
 
// Poster frame image.
byte[] imageBytes = File.ReadAllBytes("TestImage.jpg");
 
// Visible url
string vimeoVideoUrl = @"https://vimeo.com/52477838";
 
// Embed Html code.
string vimeoEmbedCode = "";
 
builder.InsertOnlineVideo(vimeoVideoUrl, vimeoEmbedCode, imageBytes, width, height);
```

The Html code for embedding video can vary between providers, consult your corresponding provider of choice for details.

Note that the document will be automatically optimized for MS Word 2013 to show video.

## Metered Licensing

Starting from 17.1.0 version, Aspose.Words provides the functionality to use the metered licensing mechanism. Aspose.Words allows developers to apply metered key. It is a new licensing mechanism. The new licensing mechanism will be used along with existing licensing method. Those customers who want to be billed based on the usage of the API features can use the metered licensing. The following code example shows how to set metered public and private keys.

```
// Create an instance of Metered class
Metered matered = new Metered();
// Sets metered public and private key 
matered.SetMeteredKey("PublicKey", "PrivateKey");
```

## Added Public Property SaveOptions.MemoryOptimization

When dealing with very large and complex documents Aspose.Words sometimes had problems during saving resulting in out of memory exceptions, disk swapping and generally failures.

We have introduced an option ([SaveOptions.MemoryOptimization][4] to optimize memory consumption during these scenarios. When its value is set to **true** it will improve document memory footprint but will add extra time to processing. This optimization is only applied during save operation.

```
/// <summary>
/// Gets or sets value determining if memory optimization should be performed before saving the document.
/// Default value for this property is <b>false</b>.
/// </summary>
public bool MemoryOptimization {get;set;}
```
```
Document doc = new Document(@"myDoc.docx");
SaveOptions so = SaveOptions.CreateSaveOptions(SaveFormat.Pdf);
so.MemoryOptimization = true;
doc.Save("myFile.pdf", so);
```

## Added FrameFormat Class for Getting Frame Related Properties of a Paragraph

We have introduced new property [Paragraph.FrameFormat][5] in Aspose.Words v17.1.0. This property provides access to the paragraph formatting properties via [FrameFormat][6] class. This class exposes all frame properties of paragraph in "readonly" mode

```
/// <summary>
/// Represents frame related formatting for a paragraph.
/// </summary>
/// This object is always created. If a paragraph is a frame, then all properties will contain respective values, otherwise
/// all properties are set to their defaults.
/// Use <see cref="IsFrame" /> to check whether paragraph is a frame.
public class FrameFormat
```

## Added Public Property TxtSaveOptions.ForcePageBreaks

We have introduced new public property ForcePageBreaks in TxtSaveOptions class. This property affects only page breaks that are inserted explicitly into a document. It is not related to page breaks that MS Word automatically inserts at the end of each page.

```
/// <summary>
/// <para>Allows to specify whether the page breaks should be preserved during export.</para>
/// <para>The default value is <b>false</b>.</para>
/// </summary>
public bool ForcePageBreaks { get; set; }
```
```
Document document = new Document();
TxtSaveOptions saveOptions = new TxtSaveOptions();
saveOptions.ForcePageBreaks = true;
document.Save("output.txt", saveOptions);
```




[1]: https://downloads.aspose.com/words/net
[2]: https://downloads.aspose.com/words/java
[3]: http://www.aspose.com/api/net/words/aspose.words/documentbuilder/methods/insertonlinevideo/index
[4]: http://www.aspose.com/api/net/words/aspose.words.saving/saveoptions/properties/memoryoptimization)
[5]: http://www.aspose.com/api/net/words/aspose.words/paragraph/properties/frameformat
[6]: http://www.aspose.com/api/net/words/aspose.words/frameformat




