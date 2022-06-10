---
title: 'How good Java package design is for commercial components?'
date: Mon, 28 Nov 2005 15:52:00 +0000
draft: false
url: /2005/11/28/36479/
author: Romank
summary: ''
tags: ['Roman Korchagin']
---

We are working on a port of Aspose.Word from C# to Java and I'm baffled by some Java features (or a lack of them) that we take for granted in C#. I don't intend to abuse Java in anyway, but I think if this language is to survive, they are ought to move and rework these things faster.

One thing that strikes me a lot is the lack of "internal" accessibility level for classes and methods. I think it is a must to have feature to be able to produce commercial software.

Aspose.Word has over 600 classes and only less than 100 of them are public. In C# code we have those 600 classes neatly split into several namespaces (read "packages"). For example Aspose.Word.RW, Aspose.Word.RW.Doc, Aspose.Word.RW.Doc.Reader, Aspose.Word.RW.Doc.Writer. The "RW" designation is of course a bit cryptic (it means Readers/Writers) but the rest is easy to understand. Aspose.Word.RW is the package that contains all readers and writers for different formats. Aspose.Word.RW.Doc contains classes that are specific to the DOC format, but used during read and write. Aspose.Word.RW.Doc.Reader contains classes that read a DOC file and so on.

The interesting thing is that all classes in the readers/writers namespaces are internal and therefore even the names of the namespaces themselves are not visible in the Aspose.Word public API. The user has nothing to do with those hundreds of classes that make reading/writing a DOC file possible. The users only see the high-level document object model in the Aspose.Word namespace that contains Document, Section, Paragraph etc classes.

The problem is that I don't see a rational way of expressing this innocent design in Java, yet Java is considered to be so successfull OO language. In Java a class can be either made public and be publicly accessible from all packages, or it can be made "non public" and be accessible only from within the package it is declared in. So I have at least 3-4 packages that have to have dependencies between them, yet I don't want those dependencies (and in fact all of these packages) to be public. That is the real question for me. How could Java be so praised if it does not allow such essential things or maybe I miss something basic?

In the end we had to workaround by putting all 600! classes into one! package Aspose.Word. We just kept the original folder structure intact of course. This does not look like a powerfull OO language to me.

Setting Java aside, I would be interested to hear of your experience with packaging classes into namespaces and dependencies between namespaces in C#. I'll probably write another post about this.







