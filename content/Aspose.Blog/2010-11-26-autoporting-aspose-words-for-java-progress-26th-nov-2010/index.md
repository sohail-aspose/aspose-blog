---
title: 'Autoporting Aspose.Words for Java Progress - 26th Nov 2010'
date: Fri, 26 Nov 2010 00:09:00 +0000
draft: false
url: /2010/11/26/autoporting-aspose-words-for-java-progress-26th-nov-2010/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

We have 9100 unit tests in Aspose.Words for Java and 923 of them pass right now.

On the surface it might look ugly that 90% of the tests fail. But there seems to be a few simple problems (stubs instead of code in some of the most basic platform abstraction methods such as formatting a double into a string). I am sure fixing those will get hundreds and thousands of unit tests to pass.








