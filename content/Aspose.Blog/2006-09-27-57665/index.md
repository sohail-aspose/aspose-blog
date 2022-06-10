---
title: 'ExpoRTFaster!'
date: Wed, 27 Sep 2006 21:47:00 +0000
draft: false
url: /2006/09/27/57665/
author: DmitryV
summary: ''
tags: ['Dmitry Vorobyev']
---

I'm glad to report that one of the numbers published by Roman in his recent post is now out of date. I'm talking of the Aspose.Words RTF export speed. We wanted to optimize the export before v4.0 final is released and we've succeeded Basically, exporting documents to RTF format is more time and memory consuming process than to DOC or WordML. It's because of some specifics of the format. For example, "correct" RTF (such as that produced by AW ) should include extra fragments to satisfy old readers and the emission of those fragments might take an extra time. But now, after applying a number of optimizations RTF export is reasonably close to DOC and WordML export processes. We've succeeded to improve performance by more than 30% so that the large, complex, 212 pages document mentioned by Roman is now saved to RTF in around 2 seconds! A similar improvement (over 30%) has been made to memory allocation so that the amount of memory consumed by the RTF exporter is now close to those consumed by other AW exporters.

And this is not a limit of course It's like a challenge to us - if we can make it even more faster, accurate, powerful. Even more AWesome!







