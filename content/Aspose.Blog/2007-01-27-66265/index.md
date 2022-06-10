---
title: 'Documentation for exceptions in the Aspose.Words public API'
date: Sat, 27 Jan 2007 14:48:00 +0000
draft: false
url: /2007/01/27/66265/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

It would be great if there was any guideline on writing the <exception> documentation tags.

The .NET Framework Guidelines book gives plenty of guidelines on using exceptions, but nothing about documenting exceptions thrown by a method.

I fully agree and support the idea that the exception specification is not part of the C# language, but documenting what exceptions are thrown by a method in a public API is an entirely different thing and I think it must be done. The .NET Framework itself documents thrown exceptions thoroughly.

We are developers of a popular commercial component and we were not documenting thrown exceptions, but the users ask for this and we must formulate a strategy.

The question basically is:

**I have a public API method A which calls heaps of internal methods and heaps of .NET framework methods and classes.** **What <exception> documentation should I include in the documentation of the method A?**

Possible answers:

a. Should I document only exceptions thrown explicitly by method A?

b. Should I document ALL possible exceptions that can be thrown by method A and ANY method that it calls?

  
If I do "a", then it is easy to mislead the users by "underdocumentation". For example I have a public method Load that does something simple and calls the more meaty internal method LoadCore. It makes no sense to document exceptions thrown only by the Load method since there are none. Then I must do "b".

However, it is very hard to do "b" properly because it requires a lot of maintenance! Basically it means the documentation for exceptions for a public method will depend on the actual implementation that could be deep down. For example, I changed the implementation of the Load method to use different .NET methods and classes and they throw different exceptions now. I should then manually find and update all exception documentation that could be affected!!!

So I think we will stick with NO <exception> documentation for the time being.

Please feel free to comment.








