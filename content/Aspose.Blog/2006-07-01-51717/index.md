---
title: 'Aspose.Words supports new List Formatting API'
date: Sat, 01 Jul 2006 00:12:00 +0000
draft: false
url: /2006/07/01/51717/
author: Romank
summary: ''
tags: ['Roman Korchagin']
---

I'm happy to announce we've extended the public API of Aspose.Words to include classes that allow you to fully control list formatting in your documents. This feature has been requested by many customers a long time ago, so we think its time.  

Here is what you can do now (what we've been designing the API for):

*   Create bulleted and numbered lists based on any of the Microsoft Word's list templates (there is 21 template in Microsoft Word, they include bulleted, numbered, and outline lists).
*   Copy list formatting to create new lists based on existing list formatting. You can copy list formatting between different documents too.
*   Access and modify the formatting of any list and list level. You now have access to numbering style, number format, start value, number position, tab position, and so on.
*   Apply for bullets and numbers and set a list level for any paragraph in the document directly or when using DocumentBuilder.
*   Create, modify list styles, and apply list styles to paragraphs.

Here is a short code example:

```
Document doc = new Document();
DocumentBuilder builder = new DocumentBuilder(doc);

// Create a numbered list based on one of the Microsoft Word list templates and
// apply it to the current paragraph in the document builder.
builder.ListFormat.List = doc.Lists.Add(ListTemplate.NumberArabicDot);

// There are 9 levels in this list, let's try them all.
for (int i = 0; i < 9; i++)
{
    builder.ListFormat.ListLevelNumber = i;
    builder.Writeln("Level " + i.ToString());
}
```

The new and updated classes are Lists, List, ListLevels, ListLevel, and ListFormat. Check them out in the API Reference, they come with plenty of code examples. We will also update the information about lists in the Programmers Guide soon.







