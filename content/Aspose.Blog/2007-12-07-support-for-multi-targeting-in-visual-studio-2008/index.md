---
title: 'Support for Multi-Targeting in Visual Studio 2008'
date: Fri, 07 Dec 2007 12:12:00 +0000
draft: false
url: /2007/12/07/support-for-multi-targeting-in-visual-studio-2008/
author: Muhammad Rashid
summary: ''
tags: ['Muhammad Rashid']
---

Like many other developers working with .NET Framework, I too have both Visual Studio 2003 and Visual Studio 2005 installed on my system. The reason being that I occasionally need to develop applications which must work on target systems which only have .NET Framework 1.1. Now I have become quite used to the IDE of Visual  Studio 2005 and enjoy the various features which make programming easy. So when ever I have to switch to Visual Studio 2003 for development, I can’t help but frown.

On Monday, Nov. 19, Microsoft announced that Visual Studio 2008 and the .NET Framework 3.5 were released to manufacturing (RTM). Visual Studio 2008 contains more than 250 new features. But the one feature that I was really waiting for is Multi-Targeting. This means that Visual Studio will now support targeting multiple versions of the .NET Framework, and developers will be able to take advantage of the new features that Visual Studio provides without having to migrate their existing projects and deployed applications to use a new version of the .NET Framework. Now when we open an existing project or create a new one with VS 2008, we can pick which version of the .NET Framework to work with. The IDE will update its compilers and feature-set to match the chosen .NET Framework. Features, controls, projects, item-templates, and references that do not work with the selected version of the Framework will be made unavailable or will be hidden.  
   
I know you are over whelmed with joy, but don’t throw away that copy of Visual Studio 2003 just yet. There is a slight problem. Unfortunately the VS 2008 multi-targeting support only works with .NET 2.0, .NET 3.0 and .NET 3.5 - and not against older versions of the framework.  The reason that Microsoft gives is that there were significant CLR engine changes between .NET 1.x and 2.x that make debugging very difficult to support.  In the end the costing of the work to support that was so large and impacted so many parts of Visual Studio that they weren't able to add support for 1.1 in this release. VS 2008 does run side-by-side, though, with VS 2005, VS 2003, and VS 2002.  So it is definitely possible to continue targeting .NET 1.1 projects using VS 2003 on the same machine as VS 2008.

So now I won’t have to keep three versions of Visual Studio, instead I can do just fine with only Visual Studio 2003 and Visual Studio 2008 installed on my system. Hmm… is that an improvement, as I seem to recall that I previously had two versions as well.







