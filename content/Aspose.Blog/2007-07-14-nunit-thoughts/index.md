---
title: 'NUnit Thoughts'
date: Sat, 14 Jul 2007 20:07:00 +0000
draft: false
url: /2007/07/14/nunit-thoughts/
author: Romank
summary: ''
tags: ['Roman Korchagin']
---

Here is short blurb on our experience with NUnit. Goods and not so goods.

We are using NUnit for Aspose products on our team. We've been using it from the start. Aspose.Words for .NET at the moment has around 5000 unit tests.

Aspose.Words is a class library and to run the tests, we have its project settings set to fire up NUnit Gui executable and pass Aspose.Words.dll as a command line parameter. When NUnit Gui starts, it loads the Aspose.Words.dll debug build that contains all unit tests together with the main code.

Running NUnit Gui this way allows us to step into debugger easily (just put a break point in code and the debugger will stop there). Having tests compiled into the same assembly allows us to test internal classes and methods (we have a lot more internal classes and methods than public ones).

Since there are so many tests and running all of them takes long time (around 10 minutes at the moment), most of the runs throughout the day are "local". We run NUnit Gui with checkboxes in the tree shown and we select the branches of tests that we want to run. Sometimes (after update and before checking) we run all unit tests of course.

**Test Selections are not Persistent**

One seriously missing feature in NUnit was the lack of persistence to the selected tests across the test sessions.

I code, then I compile and fire up the project (starts NUnit Gui with my dll loaded in it), then I select some tests (out of 5000!) and run them. If something fails, I close NUnit Gui, go back to my code, fix it, fire up the project again and have to select the same tests again! This is a frequent cycle, dozens of times per day.

How could that be this feature is missing from NUnit? Am I the only one suffering from this? I remember searching and asking in NUnit forums some time ago, but nobody seemed to have this issue. Do you guys enjoy reselecting your tests each time or am I doing something wrong?

We have modified NUnit 2.2.8 to automatically persist test selections between NUnit Gui sessions and were happy ever since.

**NUnit Gui Slow Startup Time**

Aspose.Words.dll with around 5000 tests causes NUnit Gui to spend about 10 seconds starting up on a fast machine. This is unacceptable since I want run my tests many times per hour.

Splitting Aspose.Words into smaller dlls - don't want to do this at this stage. Prefer to have as few assemblies as possible (in fact we have three assemblies during development).

Run NUnit under profiler and found some ugly code. For example, UITestNode is created far too many times. By design, there should be one UITestNode object per one Test object. However, the profiler shows that for 4800 unit tests there are over 55,000! UITestNode objects are created. Apparently UITestNode objects are created in the "recursively on recursively" mode :) Fixing that should half the loading time. The other 5 seconds are spend loading tests from the assembly, will look into this too.

**Summary**

NUnit is a great testing framework. Thumbs up for all the people who work on it.

However, I think you guys are overdoing the assertion syntax and the stuff (what I saw in the latest 2.4 I think is a clear overkill). A testing framework should be simple.

I'd rather see you spent more time on making the Gui more efficient and useful. Features and bugs like I mentioned.

Another bright idea: TDD is great, but even if all tests pass, there is still plenty of ugly bugs in the code. Step through your code too, it often helps.







