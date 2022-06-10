---
title: 'Read OneNote Online Format File using C#'
date: Mon, 28 Mar 2016 16:15:38 +0000
draft: false
url: /2016/03/28/read-onenote-online-format-file-using-csharp/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Note Product Family']
---



{{< figure align=center src="images/Aspose.Note-for-.NET_.png" alt="">}}


We are pleased to announce the release of [Aspose.Note for .NET 2.2.0][1]. This month’s release includes new features, enhancements, and bug fixes that further improve the overall stability and usability of the API. To get an idea about what is new and fixed, please visit Aspose.Note for .NET 2.2.0 Release Notes section for further information. You may also visit the Public API Changes section of our documentation for a list of all changes that are part of this month’s release.

## Work with OneNote Online (SharePoint) File Format

We are pleased to share that Aspose.Note for .NET now supports OneNote online file format that is usually known as OneNote SharePoint File Format. However, there are following limitations with respect to this new feature:

*   Hand written drawings are not supported
*   Embedded Files/Images are also not supported

These limitations are due to the lack of available specifications for reading such contents. However, we are investigating all possible methods for supporting these and hope to include these in one of nearest releases.

## Add Alternative Text for Image

This month’s release also provides an enhancement where alternative text can be added for image. This can be achieved by setting the _AlternativeText_ property of the Image class for the desired alternative text as shown in the following code sample.

```
var document = new Document();
var page = new Page(document);
var image = new Image(document, "image.jpg");
image.AlternativeText = "ImageAlternativeText";
page.AppendChild(image);
document.AppendChild(page);
document.Save("output.one"); 
```

## Set Resultant Image Resolution

With this month’s release, Aspose.Note for .NET now provides support for setting resultant image resolution. The Resolution property of ImageSaveOptions class can be used to set the resolution of the resultant image.

## Other Improvements

This month’s release also fixes a number of bugs that were reported with our last month’s release. Fixing them aids to the overall stability of the API for usage.

## API Resources

You can get started with Aspose.Note for .NET by making use of information available in the following.

*   **[API Documentation][2]** – Helps getting started with the API using code samples and examples
*   **[Forum Support][3]** – Post your inquiries to get help from our technical support team
*   **[Examples][4]** – Try the ready-to-use examples of the API by downloading from our GitHub repository
*   **[API Reference Guide][5]** – Provides information about all the namespaces, classes and properties of the API




[1]: https://products.aspose.com/note/net
[2]: https://docs.aspose.com/note/net
[3]: https://forum.aspose.com/c/note
[4]: https://github.com/asposenote/Aspose_Note_NET
[5]: https://apireference.aspose.com/note/net




