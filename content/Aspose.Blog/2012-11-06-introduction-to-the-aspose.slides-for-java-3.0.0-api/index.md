---
title: 'Introduction to the Aspose.Slides for Java 3.0.0 API'
date: Tue, 06 Nov 2012 15:27:30 +0000
draft: false
url: /2012/11/06/introduction-to-the-aspose.slides-for-java-3.0.0-api/
author: Mudassir
summary: ''
tags: ['API', 'Microsoft PowerPoint', 'autoporting', 'java', 'methods', 'migration', 'product release']
categories: ['Aspose.Total Product Family', 'Aspose.Slides Product Family']
---

![Aspose.Slides icon][1]

In my [previous post][2], I announced a new release of Aspose.Slides for Java 3.0.0 and briefly touched on some of the new features in the API. This post elaborates on some of the new features and changes in Aspose.Slides for Java 3.0.0.

API versions prior to Aspose.Slides for Java 3.0.0 were developed in parallel with Aspose.Slides for .NET. So the API’s were different in terms of functionality. A few months back we decided to develop Aspose.Slides for Java 3.0.0 and all subsequent versions based on the latest version of Aspose.Slides for .NET. The process used to achieve this is what we refer to as autoporting: a method for porting the Java version directly from the .NET version. Preparing for autoporting brought about a complete restructuring of the Aspose.Slides for Java API.

Many new features have been added to the new API along with changes to the existing API methods for accessing different properties. But, for smooth transition of code from the old API to the new API has also been kept in mind and over all approach for doing things has been kept the same and only methods names have been modified in accordance with Aspose.Slides for .NET API.

## No Third-party Dependencies

APIs prior to version 3.0.0 depend on JAI API and Baltik SVG Toolkit for rendering presentations and exporting to SVG. Some of our customers had problems with these APIs.  The Aspose.Slides for Java 3.0.0 API is has its own mechanisms for rendering presentations and exporting to SVG and no longer depends on these third-party libraries.

## Migrating from Aspose.Slides for Java 2.n.n to Aspose.Slides for Java 3.0.0

The new API has been completely restructured. To help you migrate from earlier versions of Aspose.Slides for Java to Aspose.Slides for Java 3.0.0, the documentation contains a list of how method names have changed. Use it to map current methods to the new API.

The three major structural changes to the new API are:

*   renamed **get()** methods
*   renamed collection classes
*   renamed enumerations

The sections below explain these changes further to help you migrate code to the new API quickly.

### The get\_Item() Method

A major modification needed to migrate to 3.0.0 is renaming **get()** methods. All classes’ **get()** method have been renamed **get\_Item()**. For example, to access a slide in a slide collection in Aspose.Slides 2.9.n, you used the following statement:

//Getting the first slide in presentation

Slide slide=Pres.getSlides().get(0);

In Aspose.Slides 3.0.0, use the following statement.

//Getting the first slide in presentation

Slide slide=Pres.getSlides().get\_Item(0);

To get an item from a collection of entities in a presentation, use the **get\_Item()** method. This rule applies to Shapes, Paragraphs and Portions and so on.

### Collection Classes

Collection classes like Slides, SlidesEx, Shapes, ShapesEx, Paragrpahs, Portions, Authors, Comments and many others have been replaced by SlideCollection, SlideExCollection, ShapeCollection, ShapeExCollection, ParagraphCollection, PortionCollection and so on. All the changes are listed in the migration article shared above.

### Enumerations

In Aspose.Slides for Java 2.n.n, enumeration members were written with all caps. For example, SaveFormat.PPT, SaveFormat.PPTX, FillType.SOLID and AnchorText.BOTTOM\_CENTERED. All enumerations have been modified to use camel case, like in Aspose.Slides for .NET. They are now SaveFormat.Ppt, SaveFormat.Pptx, FillType.Solid and AnchorText.BottomCentered in Aspose.Slides for Java 3.0.0.

## PPT/ODP to PPTX Conversion

Last year, PPT to PPTX conversion – a much requested feature – was added to Aspose.Slides for .NET. Since Aspose.Slides for Java 3.0.0 is autoported from the .NET version, it too has this feature. Find out more about PPT to PPTX conversion in the documentation.

Support for accessing the open document presentation (ODP) format is also available in new API and it too can be converted to PPTX. [Read about accessing an ODT presentation][3] to find out more.

## Exporting Presentation to HTML

Exporting presentations to HTML so that they can be shared as web pages is another common request. Aspose.Slides for Java is now equipped with the functionality to export presentations to HTML format. [Find out how to convert PPTX to HTML][4].

## Printing Presentations

Many of our users have asked for a feature that lets them print presentations using Aspose.Slides for Java. We are pleased to share that we have included support for printing presentations, and a range of print options, in Aspose.Slides for Java 3.0.0. [Find out how to print a presentation][5].

## Protecting and Encrypting Presentations

Securing and password protecting presentations is a key feature provided by Microsoft PowerPoint. Aspose.Slides for Java 3.0.0 supports password protecting presentations, saving presentations in read only mode and saving presentations in protected mode but leaving access to the document properties. [Please visit the documentation][6] to find out more. The article also explains how to access password protected presentations and remove protection.

## Support for PowerPoint Charts

Chart rendering is a key feature of Microsoft PowerPoint but only Aspose.Slides for .NET supported working with charts. However, with the release of the Aspose.Slides for 3.0.0 API, charts are supported. Now, you can create, modify and render charts supported by Microsoft PowerPoint using Aspose.Slides for Java. [Find out how to work with charts][7].




[1]: http://www.aspose.com/Images/aspose.slides-logo2.jpg
[2]: https://blog.aspose.com/
[3]: https://blog.aspose.com/
[4]: https://blog.aspose.com/
[5]: https://blog.aspose.com/
[6]: https://blog.aspose.com/
[7]: https://blog.aspose.com/




