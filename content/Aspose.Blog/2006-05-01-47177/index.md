---
title: 'Code Examples for Aspose.Words'
date: Mon, 01 May 2006 15:43:00 +0000
draft: false
url: /2006/05/01/47177/
author: Romank
summary: ''
tags: ['Roman Korchagin']
---

Aspose.Words (and probably other Aspose components) have been plagued by lack of code examples in the API Reference.

Now we have a great new system that allows us, developers, to build code examples easily and we are putting it into heavy use. As of Aspose.Words 3.6 we included a great deal of new code examples, both for C# and VB.NET into the[ Aspose.Words API Reference][1]. Our first goal is to provide at least one code example for each class, but our final goal is to provide examples for all public members of the API. Now we will add more code examples with every release or a hotfix.

The "classical" way of including code examples as comments into C# XML documentation is really bad:

1.  Code examples are never run and compiled after they've been written and put as comments into the XML documentation. Thus code examples can become stale, obsolete and plain wrong as the API evolves.
2.  Code examples that look like commented code inside production code confuses developers and makes code hard to maintain (I always tend to uncomment or delete it).
3.  Some public members might share a single code example (because they used in that example together), this requires including the same code example in several places. This is duplication which is always bad.
4.  Source files become very long and hard to read through, hard to maintain.

To overcome the above problems we developed a new system that makes writing code examples for a .NET component an enjoyable experience:

1.  The examples ares never obsolete, in fact, they are all unit tested against the latest build of the component.
2.  One code example can be included in documentation for multiple members in the API.
3.  Automatic conversion of examples from C# into other languages is performed.
4.  Examples can be written by anybody, not developers only. Examples can be written by QA, documentation or other personnel.




[1]: http://www.aspose.com/Products/Aspose.Words/Api/index.html



