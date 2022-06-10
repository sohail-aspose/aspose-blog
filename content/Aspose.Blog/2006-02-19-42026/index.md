---
title: 'Why Find and Replace Could be so Complex in Aspose.Words'
date: Sun, 19 Feb 2006 14:38:00 +0000
draft: false
url: /2006/02/19/42026/
author: Romank
summary: ''
tags: ['Roman Korchagin']
---

The other day a customer asked how he can replace a piece of text in a Word document with a hyperlink To answer this seemingly simple question, Vladimir quickly created an example. I think the example is very smart, many thanks to Vladimir. You can see the code here http://www.aspose.com/Community/Forums/41863/ShowPost.aspx

But the example at the same time is very complex. I cringe that our Aspose.Words object model requires to write such tricky code to do a simple operation such as this find and replace. I hope you don't settle on the idea that we are complete nerds here trying to create the most complicated API to work with Word documents. We are trying our best to create a simple and intuituve API to work with Word documents.

This example with find and replace is complicated because it touches one of the fundamental "plain vs tree" object model differences. We chose to represent a Word document as a tree of nodes (DOM) so it is somewhat similar to System.Xml and to WordML too, but this brings up a number of issues that could have been non-existent if we made a "flatter" object model.

To understand why replace is not always trivial in Aspose.Words, ask yourself why there is no "find and replace" functionality in System.Xml. Or how would you search for a piece of text in an XML file that spans across several elements at different levels and replace it with a few other nodes. That's exactly what Aspose.Words is doing when you invoke find and replace.







