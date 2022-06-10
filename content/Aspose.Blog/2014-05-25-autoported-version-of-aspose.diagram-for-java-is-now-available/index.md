---
title: 'Autoported Version of Aspose.Diagram for Java is Now Available!'
date: Sun, 25 May 2014 11:05:31 +0000
draft: false
url: /2014/05/25/autoported-version-of-aspose.diagram-for-java-is-now-available/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.Diagram Product Family']
---

[![Aspose.Diagram for Java logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2014/02/aspose_diagram-for-java.png)We are pleased to announce that the first release of Aspose.Diagram for Java is available. Aspose.Diagram for Java is a ported version of Aspose.Diagram for .NET. We port it to ensure that our Java customers get the same set of features as our .NET customers and can play with Microsoft Visio objects. We are pleased to present the first release of the autoported Aspose.Diagram for Java. This product is enriched and offers the same quality standards as its ancestors.

Over the years, we’ve learned to improve the user experience for our file format APIs,  now available for various development platforms, including Java. Instead of learning a file format inside out, our APIs let developers get on with coding solutions quickly and easily. Aspose manages complex binary formats efficiently.

In the coming week we will add help topics for the Aspose.Diagram for Java API. To help you out, it is fairly easy to write your own code in Java using existing .NET examples. For example, the following code snippet shows how to convert a Visio drawing Page to an image.

## Convert Visio Drawings

**Save a Visio Drawing Page as an image** \- The Aspose.Diagram API allows developers to save Microsoft Office Visio page to image file so making a thumbnail is easy. Below is the code.

**C# Sample Code**

```
// Load Visio drawing
Diagram diagram = new Diagram("input.vsd");
// Save diagram as PNG
ImageSaveOptions options = new ImageSaveOptions(SaveFileFormat.PNG);
// Save one page only, by page index
options.PageIndex = 1;
// Save as PNG
diagram.Save("D:\\Diagram.png", options); 
```

**Java Sample Code**

```
// Load Visio drawing
Diagram diagram = new Diagram("input.vsd");
// Save diagram as PNG
ImageSaveOptions options = new ImageSaveOptions(SaveFileFormat.PNG);
// Save one page only, by page index
options.setPageIndex(1);
// Save as PNG
diagram.save("D:\\Diagram.png", options); 
```

## Manipulate Visio File Formats Programmatically

Aspose.Diagram is aimed at software developers who need to work with Microsoft Office Visio in their Java applications. It is a well-structured API for loading, creating, saving and manipulating Visio objects. Visio drawing conversion is one of the most common tasks that the API is used for, but it has extensive functionality beyond this. The drawing features are useful for adding shapes, building up new drawings.

## Supported Platforms

Aspose.Diagram for Java supports any operating system that runs Java runtime, including Microsoft Windows desktops and servers, Linux, Ubuntu, and Mac OS X. It runs on J2SE 1.4.x, J2SE 5.0 (1.5), J2SE 6.0 (1.6) or higher.

## Free Trial Version

[Aspose.Diagram for Java is available for download][2]. Start a free trial today and see what Aspose.Diagram for Java can do for you and your organization.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/02/aspose_diagram-for-java-e1401178596961.png "Aspose.Diagram for Java logo"
[2]: http://www.aspose.com/community/files/72/java-components/diagram-java/default.aspx "Aspose.Diagram for Java"




