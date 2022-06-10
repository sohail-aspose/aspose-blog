---
title: 'Does anybody use XPath in Aspose.Words?'
date: Tue, 16 Nov 2010 23:25:00 +0000
draft: false
url: /2010/11/16/does-anybody-use-xpath-in-aspose-words/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Did you know you can use use XPath queries to find nodes in the Aspose.Words document tree?

Here is the API topic with some code examples http://www.aspose.com/documentation/.net-components/aspose.words-for-.net/aspose.words.compositenode.selectnodes.html

On the surface it looks like a pretty cool feature. Aspose.Words loads a document (a document in almost any wordprocessing format) into a tree-like model in memory. The model resembles OOXML, but is more "refined' meaning you don't have to deal with relationships to other parts and other raw stuff. Then you can use XPath to select some things for processing, some examples: comments, all shapes in headers footers, all paragraphs that are in tables, all first paragraphs of each section etc.

But I think there are at least two usability issues with XPath in Aspose.Words and at least two internal technical issues that suggest the idea of removing XPath support from Aspose.Words.

Here are the problems with XPath in Aspose.Words:

1\. Only expressions with element names are supported at the moment. Expressions that use attribute names are not supported. E.g. you can select all paragraphs in a table (they all are elements), but you cannot select paragraphs formatted using the Heading 1 style for example using XPath in Aspose.Words. This limitation comes from the fact that formatting attributes in Word documents are inheritable in rather complex ways and it will present problems for queries. For example, do you want to select all bold text that is formatted as bold directly or only if the bold formatting is applied using a character style.

2\. Everything that can be done with XPath in Aspose.Words can be done using the "normal" node selection API. For example see http://www.aspose.com/documentation/.net-components/aspose.words-for-.net/aspose.words.compositenode.getchildnodes\_overload\_2.html. It might require a few more lines of code than using XPath, but generally nothing too dificult.

3\. Aspose.Words for Java uses the Jaxen XPath engine, which is good, but a. one more open source library dependency, b. adds some weight to the Aspose.Words JAR and is probably not used too often. It could be a good idea to shave it off if nobody is using it.

4\. As you probably know we are autoporting Aspose.Words for .NET to Java at the moment. It is possible to port XPath support (we already have it), but it will take some time to make this code autoportable and I am looking for ways to complete autoporting sooner, so removing XPath will help somewhat.

Feel free to let us know whether:

a. Do you use XPath in Aspose.Words or not. How important is it to you?

b. Do you need support for attributes in XPath queries in Aspose.Words?

c. Will it hurt if we remove XPath support from Aspose.Words?








