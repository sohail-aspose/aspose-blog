---
title: 'Read MS OneNote TOC Files using C# with Aspose.Note for .NET 2.3.0'
date: Sun, 08 May 2016 06:02:07 +0000
draft: false
url: /2016/05/08/reading-microsoft-onenote-toc-files-supported-with-aspose.note-for-.net-2.3.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Note Product Family']
---



{{< figure align=center src="images/Aspose.Note-for-.NET_.png" alt="Aspose.Note for .NET">}}


We are pleased to announce the release of [Aspose.Note for .NET 2.3.0][1]. This month’s release includes support for Microsoft OneNote .onetoc2 file format. In addition, it also fixes a number of issues related to the API functionality. For further details about what is new and fixed, please visit the Product release notes of Aspose.Note for .NET.

## Work with **Microsoft .onetoc2 File Format**

This month’s release includes a new feature for supporting Microsoft OneNote .onetoc2 file formats. This file format contains saved table of contents. The API introduces the NoteBook class to load this new file format.  The following code sample shows the usage of this feature.

```
var notebook = new Notebook("PathToNotebook.onetoc2");
foreach (var notebookChildNode in notebook)
{
    Console.WriteLine(notebookChildNode.DisplayName);
    if (notebookChildNode is Document)
    {
        // Do something with child document
    }
    else if (notebookChildNode is Notebook)
    {
        // Do something with child notebook
    }
}
```

## Other Improvements

The routine in-house testing of the API brings issues in our notice that are fixed after investigating them thoroughly. This month’s release also fixes some internal bugs of the API that further aids to the overall stability of the API.

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
[5]: https://apireference.aspose.com/net/note




