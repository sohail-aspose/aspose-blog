---
title: 'Autoporting Aspose.Words for Java Progress - 4th Oct 2010'
date: Mon, 04 Oct 2010 14:34:00 +0000
draft: false
url: /2010/10/04/autoporting-aspose-words-for-java-progress-4th-oct-2010/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

In the previous post we celebrated all unit tests passed for a completely autoportable Aspose.Foundation (or internal library).

Now we are back to making the remainder of Aspose.Words C# source autoportable.

I used to treat the actual number of classes in Aspose.Words as confidential and disclosed the progress as percentage only e.g. 73% done. But I just remembered that anyone can easily count the number of classes in any .NET assembly in ildasm or Reflector so I don't think it makes sense to keep it confidential anymore. Using actual numbers will make the stats more lively too.

So some interesting facts about Aspose.Words.

*   Total types (classes, enums, interfaces) 2522, out of that:
*   Public types approx 180.
*   Test classes 540
*   2388 are marked for automatic porting
*   21 for manual porting (platform independence layer)
*   113 not to be ported to Java (mostly excluded features)

For autoporting I count 2388 for automatic porting + 21 for manual porting = 2409 total. From these:

*   1837 compiles on Java okay = 76.2%.
*   572 still has autoporting problems to resolve = 23.7%.

I have also uploaded [one more video][1] about autoporting. This one is about how we are fixing the files that do not compile on Java.




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.words-for-.net/entry261646.aspx




