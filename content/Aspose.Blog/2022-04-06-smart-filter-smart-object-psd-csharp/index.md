---
title: 'Work with Smart Filters and Smart Objects in PSD File with C#'
date: Wed, 06 Apr 2022 09:13:00 +0000
draft: false
url: /2022/04/06/smart-filter-smart-object-psd-csharp/
author: 'Farhan Raza'
summary: 'you can add one or more smart filters provided a layer is a smart object. This article covers how to **edit and update smart filters as well as add new filters like GaussianBlurSmartFilter, AddNoiseSmartFilter, etc. to an image programmatically in C#.**'
tags: ['Edit Smart Filters in C#', 'PSD Smart Filters in C#', 'Smart Filters in PSD', 'Smart Filters on Smart Objects PSD']
categories: ['Aspose.PSD Product Family']
---



{{< figure align=center src="images/Smart-Filters-Smart-Object-1024x397.jpeg" alt="Smart Filters Smart Objects PSD csharp">}}


Smart filters are used to enable the non-destructive editing of an image. They are re-editable as they retain the filter settings and can be adjusted or removed from the image if needed. Moreover, you can add one or more smart filters provided a layer is a smart object. This article covers how to edit and update smart filters as well as add new filters like GaussianBlurSmartFilter, AddNoiseSmartFilter, etc. to an image programmatically in C#.

*   [Work with Smart Filters and Smart Objects in PSD File – C# API Installation][1]
*   [Add, Edit and Update Smart Filters and Smart Objects in C#][2]

## Work with Smart Filters and Smart Objects in PSD File – C# API Installation {#section1}

You need to install [Aspose.PSD for .NET][3] API to work with PSD images programmatically in C# .NET. Quickly download its DLL file from the Downloads section or use the [NuGet][4] installation command in the Visual Studio IDE:

```
PM> Install-Package Aspose.PSD
```

## Add, Edit and Update Smart Filters and Smart Objects in C# {#section2}

You can edit, update, or add new smart filters to the smart objects in a PSD file by following the steps below:

*   Load the input PSD image using the [Image][5] class.
*   Load the smart object layer from the input file.
*   Edit the smart filter and check its properties like radius, blend mode, opacity, etc.
*   Update filter properties and add new smart filters like Gaussian blur, Add Noise, etc.
*   Save the output file with updated filters and check updated properties.

The code snippet below shows how to edit, update, or add smart filters on smart objects in a PSD image programmatically in C#:



The screenshot below shows the sample output produced on the console after executing the above code snippet:



{{< figure align=center src="images/Smart-Filters-Output.jpeg" alt="">}}


Moreover, you may download the input and output files from [this link][6] for reference.

## Explore API Features

There are many other classes and properties to work with the PSD and other images. You can visit the [documentation][7] section for more information.

## Get a Free Evaluation License

You can evaluate the API without any evaluation limitations by requesting a [free temporary license][8].

## Conclusion

In this article, you have learned how to work with Smart Filters on Smart Objects in a PSD image programmatically in C#. It discusses how to edit and update existing smart filters in an image, as well as add new smart filters like GaussianBlurSmartFilter, AddNoiseSmartFilter, etc. to an image. Furthermore, it is noteworthy here that you do not need to install any Photoshop, or any other image processing application to work with this feature because the API is not dependent on any other tool. In case you have any queries or concerns, please write to us at the [forum][9].

## See Also

[Add Signature to an Image Programmatically in C#][10]




[1]: #section1
[2]: #section2
[3]: https://products.aspose.com/psd/net/
[4]: https://www.nuget.org/packages/Aspose.Psd/
[5]: https://apireference.aspose.com/psd/net/aspose.psd/image
[6]: https://drive.google.com/file/d/1RGE4-ljdxYV6Mg_l5-vdglSeYtEtXmFr/view?usp=sharing
[7]: https://docs.aspose.com/psd/net/
[8]: https://purchase.aspose.com/temporary-license
[9]: https://forum.aspose.com/c/psd
[10]: https://blog.aspose.com/2022/03/18/sign-image-csharp/




