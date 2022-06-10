---
title: 'Manipulate Conflict Pages with Aspose.Note for .NET 17.11'
date: Fri, 10 Nov 2017 14:23:43 +0000
draft: false
url: /2017/11/10/manipulate-conflict-pages-with-aspose.note-for-.net/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Note Product Family']
---



{{< figure align=center src="images/Aspose.Note-for-.NET_.png" alt="aspose-note-for-net">}}


We are pleased to announce the release of [Aspose.Note for .NET 17.11][1]. This month’s release is sort of maintenance release and includes API improvements in terms of bug fixes. It also provides ability to identify conflict pages from a page’s history. For a complete note on what is new and fixed, please visit the release notes section of API documentation.

## Improvements

This release of API provides an enhancement where a page version from history can be identified as [conflict page][2]. Conflict pages are skipped by default while saving the file. Using the API, if it is marked as non-conflict using the IsConflictPage property, it will be saved as usual one in the history without being ignored as shown in the following code sample.

```
// Load OneNote document
Document doc = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

var history = doc.GetPageHistory(doc.FirstChild);
for (int i = 0; i < history.Count; i++)
{
    var historyPage = history[i];
    Console.Write("    {0}. Author: {1}, {2:dd.MM.yyyy hh.mm.ss}",
                    i,
                    historyPage.PageContentRevisionSummary.AuthorMostRecent,
                    historyPage.PageContentRevisionSummary.LastModifiedTime);
    Console.WriteLine(historyPage.IsConflictPage ? ", IsConflict: true" : string.Empty);
    // By default conflict pages are just skipped on saving.
    // If mark it as non-conflict then it will be saved as usual one in the history.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One); 
```

## Other Improvements

This version of API also includes bug fixes which further adds to the overall stability of the API. These improvements are related to working with document pages using the API.

## API Resources

You can get started with Aspose.Note for .NET by making use of information available in the following.

**[API Documentation][3]**– Helps getting started with the API using code samples and examples

**[Forum Support][4]**– Post your inquiries to get help from our technical support team

**[Examples][5]**– Try the ready-to-use examples of the API by downloading from our GitHub repository

**[API Reference Guide][6]**– Provides information about all the namespaces, classes and properties of the API



[1]: https://www.nuget.org/packages/Aspose.Note/17.11.0
[2]: https://docs.aspose.com/display/notenet/Working+with+Pages#WorkingwithPages-WorkingwithConflictPages
[3]: https://docs.aspose.com/note/net/
[4]: https://forum.aspose.com/c/note
[5]: https://github.com/asposenote/Aspose_Note_NET
[6]: http://www.aspose.com/api/net/note




