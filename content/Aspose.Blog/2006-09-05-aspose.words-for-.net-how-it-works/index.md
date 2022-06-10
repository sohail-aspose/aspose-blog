---
title: 'Aspose.Words for .NET 1.0, 1.1 and 2.0, How it Works'
date: Tue, 05 Sep 2006 09:39:00 +0000
draft: false
url: /2006/09/05/aspose.words-for-.net-how-it-works/
author: Romank
summary: ''
tags: ['Roman Korchagin']
---

Before [Aspose.Words][1] 4.0 we worked in VS.NET 2003 and built Aspose.Words.dll for .NET Framework 1.1 only. It worked on the different .NET version as follows:

*   .NET 1.0 - you had to add some entries in the application configuration file so Aspose.Words.dll targets .NET 1.0 runtime.
*   .NET 1.1 - built for it.
*   .NET 2.0 - worked, thanks to .NET forward compatibility (assemblies built for .NET 1.1 usually work fine in .NET 2.0). A few issues were reported, especially when running on 64-bit Windows.

But when reading excellent Jeffrey Richter's CLR via C# I realized that when Aspose.Words.dll built for .NET 1.1 runs on a 64-bit Windows it actually runs in 32-bit mode using the WoW64 process. Apparently, we had to do something about it.

Starting with Aspose.Words 4.0 we build two Aspose.Words.dll assemblies for .NET 1.1 and .NET 2.0 separately. We still code and work in VS.NET 2003 and not using any of the new language or framework features to make sure we can provide Aspose.Words for .NET 1.1. But we also build the same project in VS.NET 2005 for .NET 2.0 and include both dlls in the installer.

The assemblies and accompanying xml with IntelliSense documentation are installed into:

*   C:\\Program Files\\Aspose\\Aspose.Words\\bin\\net1.1
*   C:\\Program Files\\Aspose\\Aspose.Words\\bin\\net2.0

When adding a reference to Aspose.Words into your project you will see two Aspose.Words entries in the Add Reference dialog box. There is a column that specifies the runtime used by the assembly. There is also a column that displays full path to the assembly. Make sure you select a correct build of Aspose.Words when adding a reference to your project.

Note that the demo projects shipped with Aspose.Words are VS.NET 2003 projects and still reference the .NET 1.1 version of Aspose.Words.dll. However, you can open these projects and compile in VS.NET 2003 and VS.NET 2005 without problems.




[1]: https://products.aspose.com/words



