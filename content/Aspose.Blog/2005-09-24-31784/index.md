---
title: 'Abstract Factory in C# impossible?'
date: Sat, 24 Sep 2005 13:44:00 +0000
draft: false
url: /2005/09/24/31784/
author: Romank
summary: ''
tags: ['Roman Korchagin']
---

This question is a brain teaser for me at the moment. Maybe it is easy for you, let me know. Still I hope it could be interesting for you because it is directly from Aspose.Word source code.

I have a “package” that contains classes of the document model, let's call it Model and “packages” that are responsible for reading or writing the Model in a specific format, for example DocWriter, PdfWriter, HtmlWriter, HtmlReader and so on. I call them packages (UML packages) because foremost it is logical partitioning, not physical (they are all in the same assembly). The packages are in different namespaces of course, but this is irrelevant for the problem.

The problem is that at the moment the dependency is both ways. DocWriter needs to know about the Model so it can write it. Also, the Model needs to know the DocWriter so it can instantiate and invoke it when writing the document. The dependency from DocWriter to Model is “thick” - in that DocWriter knows about all or almost all classes of the Model. The dependency from Model to DocWriter is “thin” - Model only needs to instantiate DocWriter and call Save on its IDocumentWriter interface.

I wanted to make a simple tidy up and completely eliminate the thin dependency from Model to DocWriter (and other readers and writers) by using the Factory design pattern. That is by abstracting the process of creating readers and writers I was hoping to stop Model being dependent on concrete readers and writers classes.

Ha! It turned out not so trivial.

I created something like a registry of writer factories for different document formats. It is basically a map of SaveFormat enumerated value to a writer factory object. By looking up the SaveFormat key I obtain the factory object and request it to create a writer that exposes the IDocumentWriter interface. Nice and simple, the dependency from Model to writers was eliminated. The registry of factories, the factory interface and the IDocumentWriter interface are all defined in the Model package. The writers such as DocWriter, PdfWriter and HtmlWriter need only to register their factories so they can be instantiated when needed.

The real problem is how to register the writer factories?

I tried using static constructors and static variables but they don't get called or initialized until the class is first used. So it is a catch 22 situation. For example, DocWriter needs to register DocWriterFactory, but DocWriter's stratic ctor is not called until DocWriter is used, but I don't want DocWriter to be used directly from the Model package. Do you see the problem?

What could be useful here is some sort of an attribute that can be applied to a static constructor that forces that ctor to execute on startup regardless of whether the class is used or not.







