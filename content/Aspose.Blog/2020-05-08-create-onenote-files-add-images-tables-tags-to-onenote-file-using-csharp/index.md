---
title: 'Create OneNote (.ONE) Documents Programmatically in C#'
seoTitle: ""
description: ""
date: Fri, 08 May 2020 18:47:36 +0000
draft: false
url: /2020/05/08/create-onenote-files-add-images-tables-tags-to-onenote-file-using-csharp/
author: Usman Aziz
summary: ''
tags: ['Add Pages to OneNote Document using Csharp', 'Add Tables to OneNote Page using Csharp', 'Insert Hyperlinks in OneNote Document using Csharp', 'Insert Images to OneNote Page using Csharp', 'Insert Tags in OneNote Document using Csharp', 'create OneNote documents using Csharp']
categories: ['Aspose.Note Product Family']
---



{{< figure align=center src="images/Create-OneNote-File-in-C-2.jpg" alt="Create OneNote File in C# 2">}}


[Aspose.Note for .NET][1] is a feature-rich OneNote document manipulation API that lets you create, read, and convert OneNote documents programmatically using C# or VB.NET. In a [previous article][2], we have covered how to use Aspose.Note for .NET to convert, read, and parse OneNote documents. Today, we'll check out how to create OneNote documents from scratch using C#.

MS OneNote provides you a way of organizing and managing the information in the form of digital notes ([.ONE][3]. The pages in the OneNote documents are used to contain the user-defined content which may consist of text, tables, images, lists and etc. In this article, we'll cover all the basic aspects of creating pages and their content in OneNote documents.

*   [Create an Empty OneNote Document][4]
*   [Add Pages to the OneNote Document][5]
*   [Insert Images to OneNote Documents][6]
*   [Add Table in OneNote Documents][7]
*   [Add Tags in OneNote Documents][8]
*   [Insert Hyperlinks in OneNote Documents][9]

## Create OneNote (.ONE) Document using C# {#Create-an-Empty-OneNote-Document}

Let's start by creating an empty OneNote document with a page title only. The following are the steps to create the OneNote document with an empty page and save it as _.one_ file.

*   Create an instance of the Document class.
*   Create a new page by initializing the Page object with the Document class's object.
*   Set page's title using Page.Title property.
*   Call Document.AppendChild() method and pass the Page object.
*   Finally, save the OneNote document using Document.Save() method.

The following code sample shows how to create an empty OneNote document using C#.

{{< gist aspose-com-gists f1c4460425d3a75dd63cd514a9833946 "Examples-CSharp-Loading-and-Saving-CreateDocWithPageTitle-CreateDocWithPageTitle.cs" >}}

## Add Pages to OneNote Document using C# {#Add-Pages-to-the-OneNote-Document}

In this section, we'll go one step ahead and add text to the page in OneNote document. A page in the OneNote document can either be the main page or a subpage. For instance, you are creating an annual report which further contains the subsections for the monthly reports. In such a case, you can put the description of the report on the main page and the monthly reports on the subpages. In the OneNote document, this can be handled using the page levels.

The following are the steps to create pages in OneNote document.

*   Create a new OneNote document using Document class.
*   Create new pages for the document and set their level using Page class.
*   Use Outline and OutlineElement classes to create notes.
*   Add notes to the pages using Page.AppendChildLast() method.
*   Add pages to OneNote document using Document.AppendChildLast() method.
*   Save the document using Document.Save() method.

The following code sample shows how to create and add pages to OneNote documents using C#.

{{< gist aspose-com-gists f1c4460425d3a75dd63cd514a9833946 "Examples-CSharp-Pages-CreateDocWithRootAndSubPages-CreateDocWithRootAndSubPages.cs" >}}

## Insert Images to OneNote Document using C# {#Insert-Images-to-OneNote-Documents}

You can also insert images to the OneNote pages. The following are the steps to create a OneNote document having images.

*   Create an instance of Document class for a new OneNote document.
*   Use Page class to create a new page for the document.
*   Create a new instance of Image class and initialize it with the image's path.
*   Add image to the page using OutlineElement.AppendChildLast() method.
*   Add page to the document using Document.AppendChildLast() method.
*   Save the OneNote document.

The following code sample shows how to insert images to the OneNote document using C#.

{{< gist aspose-com-gists f1c4460425d3a75dd63cd514a9833946 "Examples-CSharp-Images-BuildDocAndInsertImage-BuildDocAndInsertImage.cs" >}}

## Add Tables to OneNote Document using C# {#Add-Table-in-OneNote-Documents}

Tables are a fine way of organizing and summarizing the data in the form of rows and columns. Along with efficient organization, tables let you locate the desired data quickly. OneNote documents also support tables. The following are the steps to add tables in OneNote documents.

*   Create a new OneNote document using Document class.
*   Create a new page using Page class.
*   Add a new table row and table cells using TableRow and TableCell classes respectively.
*   Insert elements to the table cells using TableCell.AppendChildLast method.
*   Add cells to the table row using TableRow.AppendChildLast() method.
*   Create an instance of Table class and add table row to it.
*   Add the table to the page using OutlineElement and Outline classes.
*   Add page to the document and save the document using Document.Save() method.

The following code sample shows how to add a table to the OneNote document using C#.

{{< gist aspose-com-gists f1c4460425d3a75dd63cd514a9833946 "Examples-CSharp-Tables-InsertTable-InsertTable.cs" >}}

## Insert Tags in OneNote Document using C# {#Add-Tags-in-OneNote-Documents}

Tags are used to categorize or prioritize the notes in OneNote documents. You can apply tags to text or paragraph to quickly find or filter the related notes. The following are the steps to create and add tags in OneNote documents.

*   Create an instance of Document class.
*   Create a new page using Page class.
*   Initialize Outline and OutlineElement objects.
*   Create a new RichText object and set its text and other properties.
*   Add a tag to the text using RichText.Tags.Add() method.
*   Append text to the page.
*   Add page to the OneNote document and save it.

The following code sample shows how to add tags to text in OneNote documents using C#.

{{< gist aspose-com-gists f1c4460425d3a75dd63cd514a9833946 "Examples-CSharp-Tags-AddTextNodeWithTag-AddTextNodeWithTag.cs" >}}

## Insert Hyperlinks in OneNote Document using C# {#Insert-Hyperlinks-in-OneNote-Documents}

Last but not the least, let's see how to insert hyperlinks to the OneNote documents using the following steps.

*   Create an instance of the Document class.
*   Create a new page for the document using Page class.
*   Set the text style of the hyperlink and its URL using the TextStyle class.
*   Create an instance of RichText class, add its text and initialize it with previously created text style for the hyperlink.
*   Add text to the page of the OneNote document.
*   Save the document as _.one_ file.

The following code sample shows how to insert a hyperlink to the OneNote document using C#.

{{< gist aspose-com-gists f1c4460425d3a75dd63cd514a9833946 "Examples-CSharp-Hyperlinks-AddHyperlink-AddHyperlink.cs" >}}

## Conclusion

In this article, you have learned how to create OneNote (.ONE) documents from scratch using C#. Furthermore, the article also covered how to insert pages, images, tables, tags, and hyperlinks to the OneNote documents programmatically. You can explore the other interesting features of Aspose.Note for .NET using the [documentation][10].

## Related Articles

*   [Convert and Read Microsoft OneNote Files using C#][11]




[1]: https://products.aspose.com/note/net
[2]: https://blog.aspose.com/2014/03/04/read-convert-extract-and-manipulate-the-microsoft-onenote-files-using-aspose.note-for-.net-1.0.0/
[3]: https://wiki.fileformat.com/note-taking/one/)
[4]: #Create-an-Empty-OneNote-Document
[5]: #Add-Pages-to-the-OneNote-Document
[6]: #Insert-Images-to-OneNote-Documents
[7]: #Add-Table-in-OneNote-Documents
[8]: #Add-Tags-in-OneNote-Documents
[9]: #Insert-Hyperlinks-in-OneNote-Documents
[10]: https://docs.aspose.com/display/notenet/Product+Overview
[11]: https://blog.aspose.com/2014/03/04/read-convert-extract-and-manipulate-the-microsoft-onenote-files-using-aspose.note-for-.net-1.0.0/





