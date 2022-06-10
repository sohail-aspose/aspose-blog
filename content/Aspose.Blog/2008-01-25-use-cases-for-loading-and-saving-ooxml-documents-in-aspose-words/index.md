---
title: 'Use Cases for Loading and Saving OOXML documents in Aspose.Words'
date: Fri, 25 Jan 2008 12:50:00 +0000
draft: false
url: /2008/01/25/use-cases-for-loading-and-saving-ooxml-documents-in-aspose-words/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

I'm inviting you to participate in shaping up of the Aspose.Words API again.

## Brief Description of the Problem

DOCX is macro-free files and .DOCM is the macro-enabled format and Microsoft Word 2007 is quite serious about enforcing the "file extension vs actual file type" relationship.

Rename a .DOCM file with a VBA project into a .DOCX file and open in MS Word, it will fail to say the document is invalid. It will not give any other explanation, it will just say XML is invalid or something like that.

With the existing Aspose.Words API it will be very easy for users to generate .DOCX files that contain VBA projects. For example, when converting .DOC into .DOCX. Such files will fail to open in MS Word 2007 saying the document is invalid.

This will bring a storm of support requests. We need to do better than that and make it clear to the users what they are doing.

## Analysis of the Existing Open/Save API

Users can open a file (load into Aspose.Words.Document object in memory) from a stream or from a file using the Document constructors. The user can specify the format of the file or Aspose.Words will detect the format automatically.

```
// Use Case 1: Open a file detect the file format automatically.
// The name of the file or extension does not matter.
//
// All of the options below do essentially the same thing.
Document doc = new Document(“MyFile.doc”);
Document doc = new Document(“MyFile.doc”, LoadFormat.Auto, “”);
Document doc = new Document(myStream);
Document doc = new Document(myStream, “”, LoadFormat.Auto, “”);

// Use Case 2: Open a file, user specifies the file format explicitly.
// Aspose.Words tries to open the specified document using the specified load format.
// If the format is wrong, it throws an exception.
//
// Why one would use this option? Only if the user thinks he knows the file format for sure.
// This approach allows to avoid auto format detection which incurs a small performance hit.
Document doc = new Document(“MyFile.doc”, LoadFormat.Rtf, “”);

// Use Case 3: Save, the file format is detected automatically.
// Aspose.Words automatically chooses the save file format based on the extension of the file name you provided.
//
// This is a very easy to use, most common method when you are saving into a disk file.
doc.Save(“MyFile.doc”);   // Saves in Microsoft Word Binary DOC format.
doc.Save(“MyFile.rtf”);  // Saves in RTF format.

// Use Case 4: Save, the user specifies the file format.
//
// As you can see, this method is very useful when you are saving into a stream. Otherwise how would you specify what format to save in?
doc.Save(myStream, SaveFormat.Rtf);
doc.Save(“MyFile.doc”, SaveFormat.Doc);
```

## Problem Highlighted```
// I think this code will be quite common. Convert a DOC file to OOXML.
Document doc = new Document("MyFile.doc");
doc.Save("MyFile.docx");
```

If MyFile.doc has a VBA project in it, it will be faithfully preserved by Aspose.Words and saved to MyFile.docx. Now, if you open MyFile.docx in MS Word 2007 you will get:

_The Office Open XML file MyFile.docx cannot be opened because there are problems with the contents. Details... No error detail available._

I think a more useful error message from MS Word 2007 would have been a good thing here, but we have to move on.

What does the user do now? Ah, oh... let's report the problem to the Aspose.Words forum because that 3rd party Aspose component must be doing something wrong.

Clearly, we must do something with Aspose.Words to prevent this problem situation. I have some ideas, but this time I want to offer everybody to brainstorm starting with a blank canvas.








