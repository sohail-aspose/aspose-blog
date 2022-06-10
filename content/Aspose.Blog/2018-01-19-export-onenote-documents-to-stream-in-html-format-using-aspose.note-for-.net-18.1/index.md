---
title: 'Export OneNote Documents to Stream in HTML Format using Aspose.Note for .NET 18.1'
date: Fri, 19 Jan 2018 16:08:39 +0000
draft: false
url: /2018/01/19/export-onenote-documents-to-stream-in-html-format-using-aspose.note-for-.net-18.1/
author: Kashif Iqbal
summary: ''
tags: ['Convert OneNote files to HTML', 'Export OneNote documents to HTML in CSharp']
categories: ['Aspose.Note Product Family']
---



{{< figure align=center src="images/Aspose.Note-for-.NET_.png" alt="aspose-note-for-net">}}


We are pleased to announce the release of [Aspose.Note for .NET 18.1][1]. This month’s release includes a new feature of saving OneNote document as HTML to stream. It also introduces support for saving document to HTML with Callbacks. For a detailed note on API changes included in this month’s release, please visit the [release notes][2] section of API documentation.

# Saving OneNote Document to HTML Stream

Aspose.Note API lets you save OneNote document to file as HTML. From this release onwards, the API now supports exporting [OneNote document to MemoryStream][3] as HTML. The HtmlSaveOptions now introduces the capability to save resources associated with document as Embedded resources of converted HTML or save explicitly on disc.

Following code samples show the usage of this feature for exporting OneNote documents to HTML.

# Save to Memory Stream with Embedded Resources

```
 string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Aspose.Note.Document(dataDir + "Aspose.one");

var options = new HtmlSaveOptions()
{
    ExportCss = ResourceExportType.ExportEmbedded,
    ExportFonts = ResourceExportType.ExportEmbedded,
    ExportImages = ResourceExportType.ExportEmbedded,
    FontFaceTypes = FontFaceType.Ttf
};
var r = new MemoryStream();
document.Save(r, options); 
```

# Save as HTML with Resources in Separate Files

```
 string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Aspose.Note.Document(dataDir + "Aspose.one");

var options = new HtmlSaveOptions()
{
    ExportCss = ResourceExportType.ExportAsFile,
    ExportFonts = ResourceExportType.ExportAsFile,
    ExportImages = ResourceExportType.ExportAsFile,
    FontFaceTypes = FontFaceType.Ttf
};
document.Save(dataDir + "document_out.html", options); 
```

# API Resources

You can get started with Aspose.Note for .NET by making use of information available in the following.

**[API Documentation][4]** – Helps getting started with the API using code samples and examples

**[Forum Support][5]** – Post your inquiries to get help from our technical support team

**[Examples][6]** – Try the ready-to-use examples of the API by downloading from our GitHub repository

**[API Reference Guide][7]** – Provides information about all the namespaces, classes and properties of the API




[1]: https://www.nuget.org/packages/Aspose.Note/
[2]: https://docs.aspose.com/display/notenet/Aspose.Note+for+.NET+18.1+Release+Notes
[3]: https://docs.aspose.com/display/notenet/Create+and+Load+a+OneNote+Document#CreateandLoadaOneNoteDocument-SavetoMemoryStreamwithEmbeddedResources
[4]: https://docs.aspose.com/display/notenet/Home
[5]: https://forum.aspose.com/c/note
[6]: https://github.com/asposenote/Aspose_Note_NET
[7]: http://www.aspose.com/api/net/note




