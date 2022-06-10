---
title: 'Aspose.Words for Java API Reference now with code examples!'
date: Thu, 27 Sep 2007 17:28:00 +0000
draft: false
url: /2007/09/27/aspose-words-for-java-api-references-now-with-code-examples/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

We have finally added code examples to the Aspose.Words for Java API Reference.

Check it out, here is a page for the Body class [http://www.aspose.com/Products/Aspose.Words/Api/index.html?url=com/aspose/words/Body.html][1]

And of course I cannot resist not to tell you how cool our system for documentation generation is.

*   Code examples are initially written in C# and arranged as unit tests in a class library.
*   We compile and run the examples project to make sure all works and passes (you don't see the actual unit testing asserts in the final cut out).
*   We tag the code in examples with special comments, such as //ExStart, //ExEnd, //ExFor:class.member, //ExSummary:text etc.
*   We use a C# to VB.NET converter (in fact, this one [http://www.tangiblesoftwaresolutions.com/][2] to create a VB.NET copy of the examples.
*   Then, we [closely port][3] C# examples to Java. This is possible because Aspose.Words for .NET and Java APIs are virtually the same.
*   Finally, we use our own tools that cut example code according to the //ExStart etc tags and inject them into the IntelliSense XML documentation in the appropriate places. The XML file with examples is fed into Aspose.NDoc that produces HTML and CHM documentation.




[1]: http://www.aspose.com/Products/Aspose.Words/Api/index.html?url=com/aspose/words/Body.html
[2]: http://www.tangiblesoftwaresolutions.com/)
[3]: http://www.aspose.com/Products/Aspose.Words/Api/index.html?url=JavaandNETDifferencesinAsposeWords.html




