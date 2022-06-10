---
title: 'Work with OneNote Documents using Aspose.Note for Java'
date: Tue, 10 Nov 2015 15:27:16 +0000
draft: false
url: /2015/11/10/introducing-aspose.note-for-java/
author: Muhammad Waqas
summary: ''
tags: []
categories: ['Aspose.Note Product Family']
---



{{< figure align=center src="images/aspose_note-for-java.png" alt="">}}


We are pleased to announce the launch of [Aspose.Note for Java][1], an API that empowers Java application developers to write applications for managing and manipulating Microsoft OneNote documents. Our .NET component for managing OneNote documents, [Aspose.Note for .NET][2], has been in the field for a long time already and has proven record for processing such documents.

## Aspose.Note for Java

Aspose.Note for Java is a Microsoft OneNote document reading and manipulation API for Java developers. At its base, Aspose.Note for Java has the strong foundations of its .NET ancestor which is already proven for empowering users to manipulate OneNote documents without the need of installing Microsoft OneNote or Office automation. In addition, users doesn’t have to worry about the underlying complexity of Microsoft OneNote format implementation.

## How to use Aspose.Note for Java

Like other Aspose components for Java, Aspose.Note for Java comes as a JAR file that can be included in applications like any other JAR file. With our vast range of articles and documentation samples, you can get started with the API in no time. Download a trial version of [Aspose.Note for Java][3] now, free of cost, and start processing OneNote documents right away.

## Aspose Perspective of Document Object Model

When Aspose.Note reads a OneNote document into memory, it creates objects of different types to represent various document elements. The API treats each of these elements as a Node and defines a class for every type of document node. The Aspose.Note Document object model represents the overall classes that the API uses for representing elements of a document.

## Supported File Formats

Aspose.Note for Java can read Microsoft OneNote 2010 as well as 2013 formats. It supports exporting document data to a number of file formats as following:

*   PDF
*   JPG
*   BMP
*   GIF
*   TIFF
*   PNG

Exporting to OneNote and HTML format is not supported at present and will be available in lateral versions of the API.

## Working with OneNote documents

Aspose.Note for Java can read Microsoft OneNote documents and arrange its contents in a well-structured manner for manipulation by users.  Reading a OneNote document is very easy and can be achieved using a single line of code as follow:

```
Document doc = new Document("Document.one");
```

Once loaded, the object can be used to carry out a number of operations on the document data as detailed in the subsequent sections.

## Conversion of Document data to Other Formats

Aspose.Note API has the capability to export OneNote documents to a number of other formats. Documents can be converted to PDF and image formats such as BMP, PNG, JPG, GIF and TIFF. Converting to other formats is as simple as loading a document and can be achieved using one liner code as follow.

```
Doc.save("output.pdf", SaveFormat.Pdf);
```

You can also specify additional save options for each type of output format using specific save options classes. For further examples about converting documents to other formats, please visit our documentation section, Conversion of Documents.

## Working with Contents of a Document

Aspose.Note API allows working with elements of OneNote document using its document object model. It provides the capability to:

*   Work with Pages of a Document
    *   Create OneNote Document with Root and Sub-Level pages
    *   Get all revisions of a specific page
    *   Get information of each page from the OneNote document
    *   Get number of pages from OneNote document
*   Work with Images
    *   Extract images from a OneNote document
    *   Get Information of each Image
    *   Insert an image on a OneNote document page
*   Work with Hyperlinks
    *   Adding a hyperlink to OneNote document
*   Work with Text
    *   Extract text from OneNote document
    *   Retrieve bullet or number list properties
*   Work with Tables
    *   Extracting plain text from the table of OneNote document
*   Work with Attachments
    *   Retrieve attached files from a OneNote document
*   Work with Tags
    *   Get Note Tag details from a OneNote document
*   Work with Tasks
    *   Get Outlook Task details from a OneNote document
*   Work with Text Styles

## API Resources

*   Documentation – Visit our documentation section for getting started with the API in no time
*   API Reference Guide – Gives detailed information about all the namespaces, classes and methods of the API
*   [Forum Support][4] – Post your queries on Aspose.Note forum to get assistance from our technical support team




[1]: https://products.aspose.com/note/java
[2]: https://products.aspose.com/note/java
[3]: https://products.aspose.com/note/java
[4]: http://www.aspose.com/community/forums/aspose.note-product-family/522/showforum.aspx




