---
title: 'Childish Exception'
date: Tue, 24 Jan 2006 10:53:00 +0000
draft: false
url: /2006/01/24/40197/
author: DmitryV
summary: ''
tags: ['Dmitry Vorobyev']
---

When working on Aspose.Word.Viewer (under .NET 1.1), I suddenly got a System.ArgumentException. The "bad" line looked harmlessly:

Brush brush = pen.Brush;

The error message was: **You may not change this Pen because it does not belong to you**. The wording of the message was strange. What did I have to do to own that Pen and how could I change that Pen by reading its property?

Since the MSDN library knew nothing about exceptions that might be thrown when accessing Pen.Brush, I searched the Internet. The problem seemed to be covered pretty scantily. I found the only suitable clarification in this blog. The cause was simple. My Pen appeared to be one of the standard pens based on system-defined colors. Those pens are returned by the static properties of the Pens class. Once such an object is created, it gets cached so if you access for example the Pens.Red property several times, you will get the same object each time. That's why those pens are made immutable and any changes are forbidden.

Stupid thing here is that simple reading an object's property, even though it returns an internal object (brush), does not look like an attempt to change the object itself. I actually didn't want to modify the obtained brush in any way. But the error message is cool! As the blogger says, "it sounds like the Drawing namespace is a little kid that doesn't want me to play with its toys, although in that case it would probably just say "Mine!" :)

Fortunately, in .NET 2.0 the kid has grown up and the issue has been fixed.







