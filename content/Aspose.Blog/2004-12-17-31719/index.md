---
title: 'When to choose Aspose.Words over other solutions'
date: Fri, 17 Dec 2004 16:22:00 +0000
draft: false
url: /2004/12/17/31719/
author: Romank
summary: ''
tags: ['Roman Korchagin', 'Aspose.Words', 'aspose.words alternatives', 'aspose.words competitors', 'aspose.words vs competitors']
---

As I'm the architect of Aspose.Word, I happened to have some ideas floating around that I thought might help you to choose the right tool for your project quicker and easier. Please note, this is just my personal point of view and although I'll try to be objective, you can expect some bias just because I know more about Aspose.Words than other options.

If you are in the market for a component or solution to handle MS Word documents, you have several alternatives:

*   SoftArtisans WordWriter
*   TX Text Control
*   Microsoft Visual Studio Tools for Office
*   Aspose.Words

# SoftArtisans WordWriter

This component is to mail merge data into the document. That's it. You cannot do anything else. You cannot insert and modify document content and formatting. I think SoftArtisans are stuck with WordWriter because they have licensed latest Word binary format from Microsoft and I suspect the license agreement prohibits them from creating a richer API to access document content or to convert DOC files into other formats. On the other hand, their access to the DOC format documentation allows them to support (preserve between open and save) most document features compared to all other non Microsoft solutions. Their other strong hand is they have Java version of the component. Personally, I think the only reason to choose WordWriter is when you need a Java component for populating DOC files with data.

# TX Text Control

TX Text Control is a visual control, it is basically a rich text editor. I must note that support for DOC format is poor compared to other components. Many DOC file elements will be destroyed if you open and save a file using the control. For example, multiple sections with page setup, headers and footers for multiple sections, textboxes and shapes, bookmarks, most of the fields, form fields, document protection, document properties, footnotes and endotes, embedded objects, multiple columns - all will be destroyed. Basically, you choose this control only when you need to build a text editor into your application. Please note that although TX Text Control is available for .NET - it is only a .NET wrapper around old style DLL. So it is far from being all managed code. On another note, I think TX Text Control will be in direct competition with VSTO2005 and will loose a lot to it.

# Microsoft Visual Studio Tools for Office 2005

VSTO2005 allows to build document solutions where Word 2003 or Excel 2003 are used as a front-end. I think it is very good at this task and by all means users will prefer to work in Word 2003, rather than in TX Text Control. VSTO2005 also includes a mechanism to insert data islands into documents and populate documents with data on the server without Office installed. However, inserting data into data islands is all you can do without Office installed. So in essense VSTO2005 will directly compete with SoftArtisans WordWriter and TX Text Control and I think it will compete very successfully.

## **Aspose.Word**s

Aspose.Word is a pure .NET component that allows to do a number of interesting things, mainly with Word documents. Essentially, this is a “can do anything with a Word document at incredible speed“ tool. You can open and save DOC files with high degree of quality. You can mail merge data into the document or use our object model to navigate to various places in the document and insert content and formatting. You can search and replace and enumerate document content. You can copy and move portions inside and between documents. Also, you can open and save files in various formats including HTML, PDF and soon to be supported WordprocessingML and RTF. So, if you need to somehow manipulate a Word document without using Automation (be it on the server or client, ASP.NET or Windows Forms application, does not matter) you just naturally choose Aspose.Word. Also, don't forget that Aspose's unique business model with direct access to developers ensures that all your issues are promptly resolved and the most requested features are available on a regular basis in weeks or even days.







