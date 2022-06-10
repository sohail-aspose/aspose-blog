---
title: 'Authoring API Help for .NET Projects'
date: Mon, 03 Oct 2005 16:02:00 +0000
draft: false
url: /2005/10/03/32926/
author: Romank
summary: ''
tags: ['Roman Korchagin']
---

I'm looking for a tool that will help me efficiently author quaility API documentation for Aspose.Word and other components. I've looked at several commercial and free tools and nothing really suits. It looks like my requirements for a help authoring tool come from a different planet.

1\. I want to use C# XML comments to create the API documentation. Therefore, the documentation will essentially be in XML format.

2\. I want the documentation for public classes and methods to be stored in separate files, not inside the .cs files. Inside my .cs files I want just to include the documentation using the include syntax:  
 /// <include file='Ue\\Document.xml' path='Topics/Topic\[@name="Document"\]/\*'/>  
 public class Document : CompositeNode  
...

Keeping documentation for public classes and methods inside your source code files is really a bad idea. Good documentation topics can grow big, topics sometimes need to include duplicate text that is already written somewhere, they need to include C# and VB.NET code examples, they need to be reviewed by a writer who is not a developer. It is a real mess trying to maintain such topics in source code in a commercial component.

3\. At the moment I have moved the API documentation into XML files and included them like shown above, but the problem is writing documentation in XML files and editing all those tags manually is not what I'd like to be doing. There needs to be a nice editor that will help to create topics with styles and consistent formatting, insert standard topic sections, allow to document parameters, return values etc easily. It would be ideal if the editor was Microsoft Word, not some custom editor.

4\. I need a way to compose topics from smaller topics. In other words, to be able to include topics into other topics. Why this is needed? You must have seen in MSDN in a lot of places same text is repeated in several topics. It is a real mess if you actually copy and paste such information in your help - this creates duplication (multiplication should I say), all gets out of sync and starts to stink. At the moment I somewhat workaround this problems, thanks the C# XML include syntax allows to use several includes to build one topic.

For example:

  /// <include file='Ue\\Node.xml' path='Topics/Topic\[@name="Node.Accept"\]/\*'/>  
  /// <include file='Ue\\Node.xml' path='Topics/Topic\[@name="Paragraph.Accept"\]/\*'/>  
 public override bool Accept(DocumentVisitor visitor)  
...  
  
In Aspose.Word object model Node.Accept is overridden by all classes that derive from Node. Each implementation of the Accept method requires its own topic with specific wording, but all of the topics need to include a paragraph or two of text that are common to all. It would be a disaster to copy and paste that common text to all Accept topics. Therefore, I have it separated. The authoring tool must allow defining reusable topics or subtopics that can be included.

5\. I need a system to maintain code examples. Aspose.Word has over 100 public classes or enumerations, each has around a dozen methods. It would be great to have a code example for every method. The plain approach of manually writing a small C# code example, converting it to VB.NET and including in the help topic is a disaster.

First, the code that goes into the example must be compiled and tested before it is included in the help file. So it would be ideal if all the example code existed as real source code in a project that can be compiled and run, preferably as some sort of unit tests that verify that the example code does indeed work correctly.

Another good reason for example code to originate from a compilable and working project is just to make sure the example code does not go stale and is always up to date with so many changes we make to the component API.

The end result I want is that writing and testing of code examples should be done in a working project with unit tests and the inclusion of the code examples into the API documentation should be completely automatic.

6\. Although I have many methods and classes in the public API and every one of them needs an example, I don't have to have that many examples. I could have one example that demonstrates use of several classes and methods. So I need a similar system for making reusable code examples and including them in different topics as I want for text topics.

7\. I'm not even talking that a good authoring tool should help to translate C# code examples into VB.NET code.

Let me know if you are aware of a suitable tool that can help to improve our documentation or if you think my requirements do come from another planet.







