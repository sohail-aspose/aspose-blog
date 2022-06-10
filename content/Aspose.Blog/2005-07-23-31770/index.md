---
title: 'The story behind Aspose.Word 3.0 new object model'
date: Sat, 23 Jul 2005 13:58:00 +0000
draft: false
url: /2005/07/23/31770/
author: Romank
summary: ''
tags: ['Roman Korchagin']
---

Our initial plans were to develop an API that is similar, if not compatible with Microsoft Word Object Model so any solution that utilizes Microsoft Word Automation could be easily migrated to Aspose.Word and the learning curve for developers who a familiar with MS Word Automation will be short. That was the original plan going back almost 2 years ago when we started working on Aspose.Word and we were exposing classes with interfaces that looked like the ones you would find in the VBA object model.  

Over time we became aware that implementing an API similar to Microsoft Word Object Model is not really suitable due to a number of reasons. One reason  it was too technically difficult to implement the Range object with its collections that are always maintained in sync.We were also concerned that the amount of synchronization the model needs to make to keep itself always consistent with itself could make it as slow as MS Word Automation and we would lose one of the big advantages Aspose.Word offers when compared to the automation approach - speed and scalability when working on a server.  

But the demand from users to expose more of the object model and allow detailed programmatic access to document elements was high so we had to find another model for the API. At that point in time Aspose.Word could have been compared to an iceberg with only 10% of the classes public and the rest several hundred classes internal and not visible to the user. Ironically, a fully functional document object model was already there and it was only a question of exposing it nicely to the users, but we did not want to expose a very custom API and impose a lot of learning on to the users.  

We chose an approach that is ought to be familiar to many .NET developers and exposed the document object model in a way similar to XmlDocument. If you worked with classes from the System.Xml namespace you should find many ideas, classes, methods and properties are similar to ones found in the Aspose.Word 3.0 object model.

*   Document conceptually is roughly equivalent to XmlDocument, it is a Composite consisting of a tree of document nodes.
*   Node and CompositeNode are somewhat similar to XmlNode and XmlElement with the exception that the methods to work with child nodes appear only in CompositeNode.
*   Node offers many methods and properties like NextSibling, PreviousSibling, ParentNode etc similar to the methods found in XmlNode.
*   CompositeNode offers many methods and properties ChildNodes, InsertBefore, InsertAfter, RemoveChild, FirstChild, LastChild etc that are doing exactly what the corresponding methods of XmlElement are doing.
*   Aspose.Word 3.0 object model defines concrete classes for all different Word document node types such as Section, Paragraph, Run, Table, Row, Cell etc.
*   There are also typed collection wrappers such as Document.Sections, Section.HeadersFooters, Body.Paragraphs, Paragraph.Runs and so on that provide easy and typed access to the child nodes. Such collections do not store the nodes, but merely provide shortcut access in a type safe manner. The child nodes are always stored in their parent node, for example Section nodes are always stored inside a Document node.
*   Unlike System.Xml, Aspose.Word 3.0 does not represent attributes as nodes. Formatting properties of nodes are exposed directly as properties of the corresponding objects, for example Run.Font, Paragraph.ParagraphFormat, Cell.CellFormat and so on.
*   XPath navigation over Aspose.Word document model is supported, see Document.SelectNodes and Document.SelectSingleNode.

To summarize: Aspose.Word 3.0 object model represents a Word document as an XmlDocument-like tree of document nodes and you can easily add, remove and modify almost any node of the document.  

We are working to add more documentation and diagrams about the new object model to the [Aspose.Word Programmers Guide][1]. Happy exploring of the new Aspose.Word API.




[1]: https://docs.aspose.com/words/net/developer-guide/



