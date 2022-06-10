---
title: 'Just 42 files remain to autoport for Aspose.Words for Java - 14th Nov 2010'
date: Sun, 14 Nov 2010 22:35:00 +0000
draft: false
url: /2010/11/14/just-42-files-remain-to-autoport-for-aspose-words-for-java-14th-nov-2010/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

If you are not sure what we are talking about, here is the previous post in this series.

Today's Aspose.Words for Java stats are:

*   Total source files 2533
*   42 files have autoporting problems
*   All other files - we automatically convert them from C# to Java using our porting tool.

What's next:

1\. We are going to sort out the remaining 42 files in the next week or so. There is basically one major porting problem now - use of ADO.NET class for mail merge. We do have a solution for this though. We already have ported this code to Java manually in the before, you can see Aspose.Words for Java supports mail merge and uses Java database classes ResultSet etc. We just need to dance a bit around it to make it _automatically_ portable as much as we can.

2\. Then we will be running unit tests on Aspose.Words for Java and making them all pass. I will be reporting how many tests still fail.

3\. Once code compiles and unit tests pass, we will be ready to gear up for releasing Aspose.Words for .NET and Java that are (almost) equal in features. So far it looks we still can make it in December.








