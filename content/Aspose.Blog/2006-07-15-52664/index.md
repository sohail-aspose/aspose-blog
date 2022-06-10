---
title: 'Download Cache Problem'
date: Sat, 15 Jul 2006 19:40:00 +0000
draft: false
url: /2006/07/15/52664/
author: DmitryV
summary: ''
tags: ['Dmitry Vorobyev']
---

Just have eliminated a bug (I think it's a bug indeed!) that was really hard to pinpoint. After doing a fresh checkout I added some new code, built the solution and ran NUnit as usual. It amazed me that no code changes reflected in the tests. Rebuilding the solution didn't give any effect. OK, I removed the _\\bin_ and _\\obj_ subdirs from the project to avoid possible copying of the old assembly that still didn't contain the changes and built the solution again. Still no luck! I disassembled the produced dll to make sure the new code was really there - it did present in the assembly. I began to suspect recently installed ReSharper 2.0 and even NUnit itself...

Of course, that was caching. I searched for other instances of the assembly over the whole file system and found the old version of the dll in _C:\\Documents and Settings\\Dmitry\\Local Settings\\Application Data\\assembly\\_. It's clear that this is the .NET download cache; however, it's still incomprehensible why VS placed there the local assembly and why it redirected the requests for this assembly to the cached version so that even an external program (NUnit) was deceived. It's also strange why this happened only once - I had never dealt with such behaviour before.

So after cleaning the cache using _gacutil /cdl_ the problem disappeared.







