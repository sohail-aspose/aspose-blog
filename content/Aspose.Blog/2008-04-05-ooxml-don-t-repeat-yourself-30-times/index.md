---
title: 'OOXML: Don''t Repeat Yourself 30 Times!'
date: Sat, 05 Apr 2008 07:06:00 +0000
draft: false
url: /2008/04/05/ooxml-don-t-repeat-yourself-30-times/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

It struck me from the first day I saw the OOXML specification how "strange" it is. You know borders in MS Word. I mean those text, paragraph and table borders. Complete specfication for a border takes 6 pages in OOXML. I'd say it is a bit too much for such a simple thing as a border, but that's okay, I guess the more detailed the spec the better.

The problem is that this 6 pages border specification is repeated in the OOXML document 30 times. Yes, for every left, right, bottom and top border and every type of object you get those 6 pages again and again.

As you know any decent programming book will tell you "don't repeat yourself" and "duplication is bad".

To me it looks like defining a simple base data type such as integer and repeating its full specification in every place in the documentation it gets used. I am completely lost at why this is the way things done in OOXML and borders is not the only thing that is duplicated.

By removing such basic duplication the OOXML spec could have been made a lot shorter. Just removing borders duplication could have made it almost 200 pages shorter.

It will be very interesting to see how OOXML spec turns out when it is final and published by ISO. I cannot find any info on this and my gut feel is that the duplication will remain and that will make it a very sad standard.

Here is more on DRY [http://en.wikipedia.org/wiki/Don't\_repeat\_yourself][1].

On the bright side, the more complex the standard - the better for component vendors such as Aspose!

You've got to be kidding trying to work with OOXML documents without a decent class library such as Aspose.Words. It took us a year to support OOXML to a reasonable level of conformance (with all MS Word formats experience we had before) and we are still working on it.




[1]: http://en.wikipedia.org/wiki/Don't_repeat_yourself




