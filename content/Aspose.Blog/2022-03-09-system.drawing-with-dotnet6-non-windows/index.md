---
title: 'Using System.Drawing with .NET 6 on non-Windows Platform'
date: Wed, 09 Mar 2022 09:18:00 +0000
draft: false
url: /2022/03/09/system.drawing-with-dotnet6-non-windows/
author: 'Farhan Raza'
summary: 'The System.Drawing.Common is the actual implementation of the System.Drawing library. However, it is now attributed as a Windows-specific library in .NET 6 Framework. Therefore, you can use Aspose.Drawing to **create a cross-platform .NET 6 Framework-based application.**'
tags: ['System.Drawing in macOS', 'System.Drawing in non-windows platform', 'system.drawing in linux']
categories: ['Aspose.Drawing Product Family']
---



{{< figure align=center src="images/System-Drawing-in-dotnet6-1024x355.jpeg" alt="System.Drawing in dotnet6">}}


The System.Drawing.Common is the actual implementation of the System.Drawing library. However, it is now attributed as a Windows-specific library in .NET 6 Framework. Therefore, you can use Aspose.Drawing to create a cross-platform .NET 6 Framework-based application. This article covers how to draw text or vector graphics using Brushes in non-Windows platforms like Linux, macOS with .NET 6 Framework.

## API Configuration from NuGet Gallery

[Aspose.Drawing for .NET][1] provides truly cross-platform support as it is written with fully managed code. You can easily access the API by downloading its DLL file from the [Downloads][2] section or from the [NuGet][3] gallery with the following installation command:

```
PM> Install-Package Aspose.Drawing
```

## Using System.Drawing in .NET 6 on non-Windows Platform

### Pre-requisites

*   .NET Framework 6.0
*   Microsoft Visual Studio 2022 (Latest Preview Version)

First of all, you need to download [Microsoft Visual Studio 2022 Preview][4] until the stable version is released. Installing Visual Studio 2022 Preview will also install .NET Framework 6.0 in a few minutes, based on your internet connection. Now we are good to proceed with further steps.

It is worth mentioning here that you can easily use System.Drawing in .NET 6 on the non-Windows environment like Linux, macOS, etc. However, you will find this demonstration using the macOS environment.

## Create a C# Console Application

Once the Visual Studio installation is complete, you need to create a C# Console Application and proceed to install Aspose.Drawing from the NuGet gallery, as explained already.



{{< figure align=center src="images/Screenshot-2022-03-10-at-1.31.40-PM-1024x411.png" alt="">}}


Next, you can draw a gradient on an image with [Bitmap][5] and [Brush][6] classes. Simply copy-paste the following code in the Program.cs file of your project:



## Output Drawing Preview

After running the code snippet above, an image containing the gradient like the following snapshot will be created on your end.



{{< figure align=center src="images/Screenshot-2022-03-10-at-1.57.10-PM-1024x861.png" alt="">}}


## Get Free Temporary License

You can avoid the watermark and evaluation limitations by getting a [free temporary license][7]. This will enable you to test the API in its full capacity.

## Conclusion

In this article, you have learned how to work with System.Drawing features in .NET 6 based application on non-windows platforms. You may like to visit the [documentation][8] section for further details about drawing text or processing drawings, etc. Furthermore, please feel free to discuss any of your concerns or inquiries with us via the [forum][9].

## See Also

[Using System.Drawing with ASP.NET Core or ASP.NET Service][10]




[1]: https://products.aspose.com/drawing/net
[2]: https://downloads.aspose.com/drawing/net
[3]: https://nuget.org/packages/Aspose.Drawing
[4]: https://visualstudio.microsoft.com/vs/
[5]: https://docs.microsoft.com/en-us/dotnet/api/system.drawing.bitmap?view=dotnet-plat-ext-6.0
[6]: https://docs.microsoft.com/en-us/dotnet/api/system.drawing.brush?view=dotnet-plat-ext-6.0
[7]: https://purchase.aspose.com/temporary-license
[8]: https://docs.aspose.com/drawing/net/
[9]: https://forum.aspose.com/c/drawing/44
[10]: https://blog.aspose.com/2021/05/20/using-system-drawing-in-asp-net-core-or-asp-net-service/




