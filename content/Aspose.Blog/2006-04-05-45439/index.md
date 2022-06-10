---
title: 'MS Word and Brown Fox'
date: Wed, 05 Apr 2006 06:48:00 +0000
draft: false
url: /2006/04/05/45439/
author: DmitryV
summary: ''
tags: ['Dmitry Vorobyev']
---

If you are not aware of this feature, type the following text in a Word document:

**\=rand()**

and hit Enter. Are you surprised? :)

This is not a bug but an undocumented (in the online Help) Word function intended to insert some dummy text. By default, it inserts 3 paragraphs, each containing 5 sentences. Each sentence is "The quick brown fox jumps over the lazy dog," which contains every letter in the English alphabet. You can control the number of the appearing paragraphs and sentences by "passing" appropriate values to the function, something like this:

**\=rand(2, 3)**

For more details see the Microsoft Knowledge Base article [How to insert sample text into a document in Word][1].




[1]: http://support.microsoft.com/?kbid=212251



