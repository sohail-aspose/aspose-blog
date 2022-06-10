---
title: '&quot;Dog Food&quot; Again - Aspose.Words Documentation Split'
date: Fri, 11 Jun 2010 14:49:00 +0000
draft: false
url: /2010/06/11/dog-food-again-aspose-words-documentation-split/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

**Everything is Split into .NET and Java**

As you might know our Aspose.Words for .NET and Aspose.Words for Java are "twin brother" products. We code in Aspose.Words for .NET and then port that code almost line-by-line to Aspose.Words for Java. The result is the two APIs are virtually the same.

Because of this similarity of two products we had only one set of online documentation and it was called _Aspose.Words for .NET and Java Documentation_. But because the two products are not really equal, some features are not yet available in Aspose.Words for Java or they are unique to Java, the customers were confused when they had to figure out the differences themselves on every page they read.

There has been a big undertaking by all Aspose teams to remove this confusion by separating all information for Aspose products for the .NET and Java platforms. This all has been done quite some time ago actually, the only thing that was not split - the Aspose.Words Documentation.

**Why it Took so Long for Aspose.Words Documentation to Split**

Because Aspose.Words for .NET and Java are so similar we really wanted to keep single-sourcing the documentation. It is especially important because we are putting a lot of effort into making Aspose.Words for .NET and Java even more similar in the features they offer. So it would be a big waste to try and manually maintain two sets of very similar documentation.

I wrote earlier that we have developed our own process and tools for building product documentation. Essentially we keep documentation in Microsoft Word documents, then we use some tools to inject code examples into it, split into topics and convert to HTML for online viewing. We eat our own dog food and of course use Aspose.Words to perform these document processing tasks.

Now, the task to split documentation into .NET and Java version has been accomplished by adding one more step to the documentation build process and this step also uses  Aspose.Words.

We accepted a technique to mark .NET or Java specific fragments of text and use Aspose.Words to delete the fragments that are not needed for the target platform.

Below is the screenshot of how the marked single source document looks like.

And here are the links to the resulting .NET and Java versions of the page:

*   .NET - http://www.aspose.com/documentation/.net-components/aspose.words-for-.net/feature-overview.html
*   Java - http://www.aspose.com/documentation/java-components/aspose.words-for-java/feature-overview.html

There is more work underway for us. We are now working on another tool to add to our documentation build process that will allow to make sure the topic pages have correct names and hyperlinks to the public API members both in .NET and Java pages.








