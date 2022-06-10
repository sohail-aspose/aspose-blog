---
title: 'What Aspose word processing component do you need'
date: Sun, 10 Dec 2006 21:37:00 +0000
draft: false
url: /2006/12/10/63095/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Great, now have two components: [Aspose.Words][1] and [Aspose.Editor][2] that deal with Microsoft Word documents and I would like to take this opportunity to explain the difference between them. The difference might be already clear to you, yet I hope this post will still be useful.

The shortest descriptions I could give:

_**Aspose.Words** is class library that enables .NET and Java applications to read, modify and write Word documents without utilizing Microsoft Word._

_**Aspose.Editor** is a word processor control for Windows Forms .NET that displays, edits and prints documents a lot like Microsoft Word, but inside your application._

* * *

Use **Aspose.Words** when you need to:

*   Generate documents, fast (generation).
*   Convert documents, with high fidelity, fast (conversions).
*   Populate documents with data from various data sources (reporting).
*   Programmatically examine/modify/merge/split documents (manipulation).
*   Work in a server environment, ASP or ASP.NET, Java.
*   Work in a client environment, but no visual editing is required.

In the past, we had one question asked very often: "Where do I see Aspose.Words in the Visual Studio Control Toolbox and how do I drag it onto my form?"

Remember, Aspose.Words is just a .NET assembly (a single jar in the Java version) that provides classes for you to perform the above stated tasks. You do not see Aspose.Words in the Control Toolbox and you do not get to drag it onto your form - you just code with it, like with System.Collections, for example. Also, your users never get to see Aspose.Words with their eyes. They can only see documents that your application generates with Aspose.Words.

Here is an example:

Aspose.Words.Document doc = new Aspose.Words.Document(MyPath + "DinnerInvitationDemo.doc"));

DataTable customers = ExecuteDataTable("SELECT TOP 5 \* FROM AsposeWordCustomers WHERE Country = 'USA'");

doc.MailMerge.Execute(customers);

doc.Save(myFileName);

* * *

Use **Aspose.Editor** when you need to:

*   Let your users WYSIWIG view or edit documents.
*   Let your users convert between different formats.
*   Programmatically access or modify the document and control selection, cursor etc.
*   Build a Windows Forms .NET application.

An interesting note is that Aspose.Editor provides a rich programming model, very similar to the one found in Microsoft Word Automation. You get all the "familiar" classes and fuctionality such as Document, Range, Selection, Paragraph, Style and so on.

It is worth mentioning, that Aspose.Editor internally embeds portions of Aspose.Words. Therefore Aspose.Editor is capable of loading, converting and saving documents in all formats supported by Aspose.Words, but you do not have direct access to Aspose.Words features embedded inside Aspose.Editor. If you need both a server document processing component and an editor control, you need to purchase both Aspose.Words and Aspose.Editor (possible in the Aspose.Total or Aspose.Custom suite).

Check out [Aspose.Editor Feature Overview][3] for screenshots and code examples.

* * *

To summarize:

Aspose.Words and Aspose.Editor were designed for different purposes and they are different codebases.

Aspose.Words is mostly used on the server, where fast and scalable processing of documents is needed. _There is no user interface features like selection, cursor or undo are built into Aspose.Words._ This all is to promote performance and scalability. After all, no-one expects unlimited undo from system-level classes.

On the other hand, Aspose.Editor is used in front-end application, where you want your users to be able to view or edit documents in a Windows Forms .NET application in a way, somewhat similar to Microsoft Word. _Aspose.Editor provides full support for keyboard, mouse, selection cursor, unlimited undo and redo._

This brings me to another interesting topic:

Be wary of other components that claim to be designed for server-based applications, yet they have a full set of features that are expected from an editor control. Undo, redo, selection, cursor etc are important to have in an editor control and they do not impose a performance impact that the end-user could notice, but there is no place for these features on the server usually. This is one of the reasons, why Microsoft Word Automation is not suitable to use on the server after all.




[1]: /Products/Aspose.Words/Default.aspx
[2]: /Products/Aspose.Editor/Default.aspx
[3]: /Products/Aspose.Editor/Api/




