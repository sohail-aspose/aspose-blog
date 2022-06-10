---
title: 'Aspose.Word Object Model Background'
date: Wed, 06 Oct 2004 06:02:00 +0000
draft: false
url: /2004/10/06/31698/
author: Romank
summary: ''
tags: ['Roman Korchagin']
---

One of the main goals of Aspose.Word is to allow programmatic manipulation of document content, such as insert, enumerate, find and replace document elements and formatting.

We studied a number of document APIs before and during Aspose.Word development. We looked at MS Word Object Model, Open Office and a number of other products. 

Those of you who are familiar with MS Word Object Model, probably agree that once you grasp few basic concepts such as working with Range, it all becomes very easy and comfortable. That's why we decided Aspose.Word Object Model should look similar. You can see this approach in the existing Aspose.Word classes Document, Section, Range, FormField, Bookmark.

However, it proves very challenging for us to mimic even the basics of MS Word Object Model successfully. Have you ever considered that all those collections and objects you use in VBA always remain coupled and synchronized? If you are interested, look at some objects in MS Word, for example Range, Paragraphs and Paragraph closely.

Create several Range objects, insert or remove text in one of them and observe that other Ranges' Start, End, Text and Paragraphs are all updated. This is only one aspect. Everything else is related to each other too including fields, bookmarks, words, sentences and so an and on.

Although we are not an open source project where everyone can contribute their effort freely, we are very happy for our users to contribute ideas for new features. Now, I want to take this one step further and invite users to contribute any design ideas too. The one I'm particularly interested in is:

How to make an object model as user friendly outside and as complex inside as in MS Word?







