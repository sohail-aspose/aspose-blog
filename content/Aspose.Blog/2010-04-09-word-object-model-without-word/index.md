---
title: 'Word Object Model without Word'
date: Fri, 09 Apr 2010 15:39:00 +0000
draft: false
url: /2010/04/09/word-object-model-without-word/
author: Mf
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

_This article is a call for your feedback. In the August 2009 we had to drop Aspose.Editor but left are functional pieces which can be reused in Aspose.Words, well, if you need them…_

In past times developers relied on Word Object Model and VBA for their automation needs. Today Microsoft recommends VSTO and OOXML but still out there could be useful applications written in VBA, or you might be interested to port those to .NET, or you'd like to leverage on your existing skills. Whatever your reasons to be interested in Word Object Model are you might get this API in Aspose.Words, and soon.

The API of Aspose.Words is well-thought and represents document as a data tree, where nodes are Sections, Paragraphs and Runs and they have “parent-child” relationship. It is straightforward, fast and convenient for many tasks however there are some exceptions which are hard to implement on the tree. For example, consider task of replacing content of a bookmark, or finding text using regular expressions, or joining paragraphs. These are much simpler to implement on flat document model and live collections of objects, like those in the Word Object Model.

Now I want to ask you one question: we have partial implementation of this API on the branch, do you want it integrated into the product?

You’d be able to work with it like this:

document.GetRange().Text = "Sample first paragraph\\r\\nAnd next paragraph";

document.Bookmarks\["MyBookmark"\].GetRange().Text = "New Text Of Bookmark";

document.Shapes.AddImage(range.Paragraphs\[2\].GetRange(), imageStream);

document.GetRange(7, 15).Delete();

range.Find.Execute("\[0-9\]\*");

range.Fields.Add(range, FieldType.FieldPage);

Also you'd be able to almost automatically port VBA scripts to C# and get huge performance increase.

Interested? Leave your comment.

\- Michael








