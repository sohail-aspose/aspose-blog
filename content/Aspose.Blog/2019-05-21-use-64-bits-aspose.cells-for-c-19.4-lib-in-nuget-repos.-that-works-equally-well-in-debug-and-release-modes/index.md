---
title: 'Use 64-bits Aspose.Cells for C++ 19.4 Library'
date: Tue, 21 May 2019 09:46:35 +0000
draft: false
url: /2019/05/21/use-64-bits-aspose.cells-for-c-19.4-lib-in-nuget-repos.-that-works-equally-well-in-debug-and-release-modes/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose_cells-for-cpp-150x150.png" alt="">}}


You cannot deny some useful features of NuGet repos. Obviously using the NuGet you can have simple and portable compilation of your codes. Without NuGet, you have to load library for all developers before compiling it on their environments. Surely, for industrialization, it would be simple to have the library on NuGet gallery.

Previously we included 64-bits lib (for VS2017) package in NuGet repos. But there was a drawback in it for certain users. We found x64 based program (using the [Aspose.Cells for C++][1] library) compiles fine in Release mode but fails in Debug mode. Some users wanted to use it in debug mode for their scenarios, they needed some objects like lists which were not accessible in Release mode. In this release, we have gone one step further. We have published the new library in NuGet repos. which can make your program compiled successfully in Debug mode as well.

We also fixed a bug in formula calculation engine where it was throwing an exception and was terminating the program. The formula calculations is another reliable aspect provided by component and you may utilize it efficiently to calculate the formulas/functions in the spreadsheet.

I would recommend you to try the release [Aspose.Cells for C++ v19.4][2]. And, if you have more time, browse [Developers' Guide][3] for your complete reference on what you can deliver using the API. You are always welcome to share your review, concerns or feedback on forums.




[1]: https://products.aspose.com/cells/cpp
[2]: https://www.nuget.org/packages/Aspose.Cells.Cpp/19.4.0
[3]: https://docs.aspose.com/cells/cpp/developer-guide/




