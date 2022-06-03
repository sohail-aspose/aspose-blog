---
title: 'Generate and Display Barcode Image in ASP.NET MVC'
date: Mon, 04 Apr 2022 16:16:39 +0000
draft: false
url: /2022/04/04/generate-and-display-barcode-image-in-asp-net-mvc/
author: ''Muzammil Khan''
summary: 'As a .NET developer, you can easily generate various types of barcodes and display them in Razor pages. In this article, you will learn **how to generate and display a barcode in an ASP.NET MVC application.**'
tags: ['.NET BarCode Generation API', 'Display Barcode Image', 'Display Barcode in ASP.NET MVC', 'Generate Barcode in ASP.NET MVC', 'Generate Barcodes', 'MVC Barcode Generator']
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/ASP-NET-MVC-Barcode-Generator.jpg" alt="Generate and Display Barcode Image in ASP.NET MVC">}}


A barcode visually represents data in a machine-readable form. Usually, it contains data or information about a product or a company, encoded in the form of numbers and/or a pattern of parallel lines. In ASP.NET MVC, we can generate various types of barcodes such as Data Matrix, Aztec, Code 128, etc. In this article, we will learn **how to generate and display a barcode image in the ASP.NET MVC** application. After following the mentioned steps, we will have our own **ASP.NET MVC Barcode Generator**. So let’s begin.

The article shall cover the following topics:

*   [Features of ASP.NET MVC Barcode Generator][1]
*   [.NET API to Generate and Display Barcode Image][2]
*   [Steps to Generate and Display Barcode Image][3]
*   [Demo ASP.NET MVC Barcode Generator][4]
*   [Download Source Code][5]

## Features of ASP.NET MVC Barcode Generator {#Features-of-ASP-NET-MVC-Barcode-Generator}

Our ASP.NET barcode generator will have the following features.

1.  Generate the following types of barcode symbologies:
    *   Code128
    *   Code11
    *   Code39
    *   QR
    *   Datamatrix
    *   EAN13
    *   EAN8
    *   ITF14
    *   PDF417
2.  Save the generated barcode image in the following formats:
    *   PNG
    *   JPEG
    *   BMP
    *   EMF
    *   SVG
3.  Preview the generated barcode image.
4.  Download the generated barcode image to your local disk.

## .NET API to Generate and Display Barcode Image in ASP.NET MVC {#Dot-NET-API-to-Generate-and-Display-Barcode-Image-in-ASP-NET-MVC}

For generating barcode images and displaying them in the ASP.NET MVC application, we will be using the Aspose.BarCode for .NET API. It allows us to generate and recognize a wide range of 1D & 2D [barcode types][6]. Please either [download][7] the DLL of the API or install it using [NuGet][8].

```
PM> Install-Package Aspose.BarCode
```

## Steps to Generate and Display Barcode Image in ASP.NET MVC {#Steps-to-Generate-and-Display-Barcode-Image-in-ASP-NET-MVC}

We can generate and display a barcode image in the ASP.NET MVC application by following the steps given below:

*   Firstly, create a new project and select the **ASP.NET Web Application (.NET Framework)** project template.



{{< figure align=center src="images/select_project_template.-1024x668.jpg" alt="" caption="Select the project template.">}}


*   Next, in **Create a new ASP.NET Web Application** dialog, choose **MVC** and then choose to **create**.



{{< figure align=center src="images/Select_mvc-1024x672.png" alt="Select MVC" caption="Select MVC">}}


*   Then, open _**NuGet Package Manager**_ and install [Aspose.BarCode for .NET][9] package.



{{< figure align=center src="images/Install_Aspose_Barcode_Nuget-1024x597.jpg" alt="Install Aspose.BarCode for .NET" caption="Install Aspose.BarCode for .NET">}}


*   Next, create a new folder “_Images_” to save the generated barcode images.



{{< figure align=center src="images/Create-Images-Folder.jpg" alt="Create Images folder." caption="Create Images folder.">}}


*   Now, create a model in the “_Models_” folder with the name “_Barcode_” to store the barcode information.

{{< gist aspose-com-gists 78c04f45434d446c01e3543fdd084192 "GenerateAndDisplayBarcode_ASP.NET_MVC_Barcode.cs" >}}

*   Also, add enumeration to list the supported barcode symbologies. It can be added in a separate class under the _“Models”_ folder, or we can add it in the Barcode.cs class file.

{{< gist aspose-com-gists 78c04f45434d446c01e3543fdd084192 "GenerateAndDisplayBarcode_ASP.NET_MVC_BarcodeType.cs" >}}

*   Similarly, add enumeration to list the supported image formats.

{{< gist aspose-com-gists 78c04f45434d446c01e3543fdd084192 "GenerateAndDisplayBarcode_ASP.NET_MVC_ImageType.cs" >}}

*   Next, open _Views/Home/index.cshtml_ and replace its content with the following script.

{{< gist aspose-com-gists 78c04f45434d446c01e3543fdd084192 "GenerateAndDisplayBarcode_ASP.NET_MVC_index.cshtml" >}}

*   Then, open the “_HomeController_” class and add a new action result to handle the post request.

{{< gist aspose-com-gists 78c04f45434d446c01e3543fdd084192 "GenerateAndDisplayBarcode_ASP.NET_MVC_Index.cs" >}}

*   After that, add a new action result to handle the image download request in the “_HomeController_”.

{{< gist aspose-com-gists 78c04f45434d446c01e3543fdd084192 "GenerateAndDisplayBarcode_ASP.NET_MVC_Download.cs" >}}

*   Finally, run the application.

## Demo ASP.NET MVC Barcode Generator {#Demo-ASP-NET-MVC-Barcode-Generator}

The following is the demonstration of the ASP.NET MVC Barcode Generator application we have just created.



{{< figure align=center src="images/asp-net-mvc-barcode-generator.gif" alt="Demo ASP.NET MVC Barcode Generator" caption="Demo ASP.NET MVC Barcode Generator">}}


## Download Source Code {#Download-Source-Code}

You can download the complete source code of the ASP.NET MVC Barcode Generator application from [GitHub][10].

## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][11] to try the library without evaluation limitations.

## Conclusion

In this article, we have learned **how to **generate and display a barcode image in an ASP.NET MVC**** application. We have also seen **how to download the generated barcode image** programmatically. Besides, you can learn more about Aspose.BarCode for .NET API using the [documentation][12]. In case of any ambiguity, please feel free to contact us on the [forum][13].

## See Also

*   [](https://blog.aspose.com/2020/10/20/scan-and-read-barcodes-using-csharp/)[Generate and Read Royal Mail Mailmark 2D Barcode using C#][14]
*   [Generate Barcodes using C# – .NET Barcode API][15]




[1]: #Features-of-ASP-NET-MVC-Barcode-Generator
[2]: #Dot-NET-API-to-Generate-and-Display-Barcode-Image-in-ASP-NET-MVC
[3]: #Steps-to-Generate-and-Display-Barcode-Image-in-ASP-NET-MVC
[4]: #Demo-ASP-NET-MVC-Barcode-Generator
[5]: #Download-Source-Code
[6]: https://docs.aspose.com/barcode/net/barcode-supported-symbologies/
[7]: https://downloads.aspose.com/barcode/net
[8]: https://www.nuget.org/packages/aspose.barcode
[9]: https://products.aspose.com/barcode/net
[10]: https://github.com/Muzammil-khan/ASP.NET-MVC-Barcode-Generator
[11]: https://purchase.aspose.com/temporary-license
[12]: https://docs.aspose.com/barcode/net/
[13]: https://forum.aspose.com/c/barcode/13
[14]: https://blog.aspose.com/2022/03/03/generate-and-read-royal-mail-mailmark-2d-barcode-using-csharp/
[15]: https://blog.aspose.com/2020/10/19/generate-barcodes-using-csharp/




