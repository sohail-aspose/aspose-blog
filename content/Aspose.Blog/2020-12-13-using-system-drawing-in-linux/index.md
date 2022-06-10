---
title: 'Using System.Drawing in Linux without libgdiplus'
seoTitle: "Using System.Drawing in Linux | C# Graphics API for Linux"
description: "Use C# .NET Graphics API to use System.Drawing in Linux without libgdiplus. Use Aspose.Drawing in .NET Core applications without rendering issues."
date: Sun, 13 Dec 2020 12:20:08 +0000
draft: false
url: /2020/12/13/using-system-drawing-in-linux/
author: Usman Aziz
summary: 'If you ever had to run your .NET Core applications on Linux you may have noticed that one of the main problems is the lack of [System.Drawing][1] assembly in standard .NET Core package. Even though Microsoft recommends to use [System.Drawing.Common][2], that is not the ultimate solution. You have to run ‘_sudo_’ on each user machine to have [libgdiplus][3] library installed. And even after that, your rendering results will be slightly different from those you have on Windows machines. In order to cope with this issue, this article covers **how to use the System.Drawing in Linux without libgdiplus** library.'
tags: ['csharp 2d graphics', 'csharp graphics library in linux', 'graphics API for linux', 'system.drawing in linux']
categories: ['Aspose.Drawing Product Family']
---



{{< figure align=center src="images/Graphics-API-Linux.jpg" alt="System.Drawing in Linux">}}


If you ever had to run your .NET Core applications on Linux you may have noticed that one of the main problems is the lack of [System.Drawing][4] assembly in standard .NET Core package. Even though Microsoft recommends to use [System.Drawing.Common][5], that is not the ultimate solution. You have to run ‘_sudo_’ on each user machine to have [libgdiplus][6] library installed. And even after that, your rendering results will be slightly different from those you have on Windows machines. In order to cope with this issue, this article covers **how to use the System.Drawing in Linux without libgdiplus** library.

*   [Using System.Drawing on Linux][7]
*   [.NET Graphics API - Easy to Install][8]
*   [No Unpredictable Platform Issues][9]
*   [Identical Rendering Results][10]
*   [Try Aspose.Drawing for Free][11]
*   [Conclusion][12]

## Using System.Drawing on Linux {#System.Drawing-on-Linux-with-Aspose.Drawing}

Fortunately, now we have a solution. Below we will demonstrate how our .NET Graphics API, [Aspose.Drawing for .NET][13], can help you use _System.Drawing_ in Linux. Using Aspose.Drawing, you can get rid of graphics libraries with native code and have your images look the same on all platforms.

## .NET Graphics API - Easy to Install

For installation of _Aspose.Drawing_ on a target Linux machine you just need to have .NET Core installed. Put _Aspose.Drawing.dll_ in your project folder and run the program. That's all. Now you can use classes in _System.Drawing_ namespace just like you do it from your .NET Framework applications on Windows.

To get _Aspose.Drawing_ binaries, please [download][14] the latest version from the official website. Alternatively, you can include the API directly in your project by running the following command.

```
dotnet add package Aspose.Drawing
```

No additional components are required. _Aspose.Drawing_ does all the drawing itself without referencing any native library. You will never receive messages like:

```
Unable to load DLL 'libgdiplus': The specified module could not be found.
```

And you don’t have to care about the version of the graphics system installed on your platform.

## No Unpredictable Platform Issues {#No-Unpredictable-Platform-Issues}

With _System.Drawing.Common_ you can get unpredictable errors on Linux when running code that was successfully run on Windows:

```
WARNING *: Path conversion requested 34759680 bytes (2480 x 3504). Maximum size is 8388608 bytes.
ERROR:region.c:1155:GdipCombineRegionPath: assertion failed: (region->bitmap)
```

_Aspose.Drawing_ doesn't depend on _libgdiplus_, so you will be free of such problems. We have a fully managed drawing engine which means that we have no dependencies on native graphics libraries. You will no longer encounter incomprehensible platform errors and unpredictable behavior of your program.

## Identical Rendering Results {#Identical-Rendering-Results}

Another benefit of using _Aspose.Drawing_ is identical rendering results on all supported platforms. If you use _System.Drawing.Common_ in .NET Core, your rendering results may look different on Windows and Linux, see the example below.



{{< figure align=center src="images/image-comparison-aspose.drawing.png" alt="System.Drawing on Linux and Windows">}}


With _Aspose.Drawing_ you can create cross-platform graphic applications for Windows, Linux, or Android and you will always get the same rendering results on each platform. This was achieved by the creation of a platform-independent 2D rendering engine instead of relying on 3rd party graphics libraries.

Aside from graphical primitives, font rendering is the same across all platforms. And even though system fonts on Linux differ from Windows, you can use _PrivateFontCollection_ to load your own set of fonts. Another way is to install a pack of Microsoft fonts into a Linux system and call text rendering functions as usual.

## Try Aspose.Drawing for Free {#Try-Aspose.Drawing-for-Free}

Aspose.Drawing is available on [NuGet][15]. You can also [download][16] binaries or the MSI installer. You can use _Aspose.Drawing_ library with restrictions or request a [free trial license][17].

So why not try it today?

## Conclusion {#Conclusion}

In this article, you have seen how easy it is to use _System.Drawing_ on all platforms without any dependencies and get the same result. You can learn more about _Aspose.Drawing_ at the official [page][18]. For any questions, please use the [forum][19] and stay tuned for future posts and guides.

## See Also

*   [Draw Graphics and Create 2D Drawings using C#][20]




[1]: https://docs.microsoft.com/en-us/dotnet/api/system.drawing?view=dotnet-plat-ext-5.0
[2]: https://www.nuget.org/packages/System.Drawing.Common/
[3]: https://www.mono-project.com/docs/gui/libgdiplus/
[4]: https://docs.microsoft.com/en-us/dotnet/api/system.drawing?view=dotnet-plat-ext-5.0
[5]: https://www.nuget.org/packages/System.Drawing.Common/
[6]: https://www.mono-project.com/docs/gui/libgdiplus/
[7]: #System.Drawing-on-Linux-with-Aspose.Drawing
[8]: #HEasytoinstall
[9]: #No-Unpredictable-Platform-Issues
[10]: #Identical-Rendering-Results
[11]: #Try-Aspose.Drawing-for-Free
[12]: #Conclusion
[13]: https://products.aspose.com/drawing
[14]: https://downloads.aspose.com/drawing/net
[15]: https://www.nuget.org/packages/Aspose.Drawing
[16]: https://downloads.aspose.com/drawing/net
[17]: https://purchase.aspose.com/temporary-license
[18]: https://products.aspose.com/drawing/net
[19]: https://forum.aspose.com/c/drawing
[20]: https://blog.aspose.com/2020/06/30/draw-graphics-and-create-2d-drawings-using-csharp-or-vb.net/





