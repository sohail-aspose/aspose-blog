---
title: 'Tracked Changes API, Interruption Handling and Numerous Other Improvements in Aspose.Words 11.6.0'
date: Thu, 02 Aug 2012 01:52:41 +0000
draft: false
url: /2012/08/02/tracked-changes-api-interruption-handling-and-numerous-other-improvements-in-aspose.words-11.6.0/
author: Adam Skelton
summary: ''
tags: ['API', 'Interruption', 'Revisions', 'Thread', 'Track changes', 'rendering']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose.words-logo2.jpg" alt="">}}


We have just released this month’s improvements to Aspose.Words for .NET and Java. This month’s release includes around 90 improvements to many areas of our component.

You can immediately download our latest Aspose.Words release from the following links:

*   [Aspose.Words for .NET 11.6.0][1]
*   [Aspose.Words for Java 11.6.0][2]

Here is a look at the two biggest features in this release:

## Introduction of the Revisions API

Revisions (tracked changes) are a feature built-in to Microsoft Word which stores all modifications made to a document during editing. Having more detailed access to these revisions is a hotly requested feature and is now possible with the release of Aspose.Words 11.6.0.

The brand new API provides the following features:

<figure class="wp-block-table"><table class=""><tbody><tr><td>**Feature</strong></td><td><strong>Code Sample (C#)**</td></tr><tr><td>Access individual or all revisions in a document</td><td>Document document = new Document(); RevisionCollection revisions = document.Revisions; Revision revision = revisions[0];</td></tr><tr><td>Get/Set individual revision properties</td><td>// Read/write access to the author of the revision. revision.Author = "Aspose.Words"; // Read/write access to DateTime of the revision. revision.DateTime = new DateTime(2012, 04, 18); // Get the parent node of the revision. revision.Parent;</td></tr><tr><td>Accept/Reject individual or all revisions</td><td>// Accept one revision. document.Revisions[0].Accept(); // Accept all revisions. document.Revisions.AcceptAll(); // Reject one revision. document.Revisions[0].Reject(); // Reject all revisions. document.Revisions.RejectAll();</td></tr><tr><td>Retrieve the type of the revision</td><td>revision.RevisionType; // Insertion, Deletion or FormatChange.</td></tr></tbody></table></figure>

## Interrupt Aspose.Words during a Long Conversion Process

Aspose.Words now provides the functionality to “cancel” a task if requested by the user. For instance, if a large document is deemed to be taking too long to convert then the process can be interrupted.

**Note: Currently this feature is only supported during rendering to fixed page formats such as PDF, XPS, image etc.**

### Interruption in Aspose.Words for .NET

An instance of the **InterruptionToken** class can be bound to the current thread and the **Interrupt** method called to forcibly halt processing of Aspose.Words, for example in order to implement a specific timeout period during conversion.

When the interruption is handled by Aspose.Words a **ThreadInterruptedException** is thrown to be handled by the calling code.

### Interruption in Aspose.Words for Java

Aspose.Words for Java takes advantage of the standard Java thread interruption implementation by using **Thread.Interrupt** and **InterruptedException.** Simply perform the Aspose.Words conversion on a new thread and use the interrupt method if required.




[1]: https://downloads.aspose.com/words/net
[2]: https://downloads.aspose.com/words/JAVA




