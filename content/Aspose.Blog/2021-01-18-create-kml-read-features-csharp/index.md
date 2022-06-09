---
title: 'Create KML File or Read its Features Programmatically using C#'
seoTitle: "Create KML File or Read its Features Programmatically using C#"
description: "Create KML file Programmatically in C#. Read KML file features. You can work with different GIS file formats in your .NET based applications."
date: Mon, 18 Jan 2021 10:23:00 +0000
draft: false
url: /2021/01/18/create-kml-read-features-csharp/
author: Farhan Raza
summary: 'KML is abbreviated for Keyhole Markup Language which is extended from XML. It is a GIS file format and is used to display geographical information. You can **create KML files** programmatically, as well as **read information** from them using C# language.'
tags: ['create kml file', 'kml file c#', 'read kml features c#', 'read kml file']
categories: ['Aspose.GIS Product Family']
---



{{< figure align=center src="images/Create-Edit-KML-file.png" alt="Create Edit KML File">}}


[KML][1] is abbreviated for Keyhole Markup Language which is extended from XML notation. It is a [GIS file format][2] and is used to display geographical information. You can **create KML files** programmatically, as well as **read information** from them using [C#][3] language. Let us explore the following sections related to KML file format:

*   [Creating or Reading KML Files – API Installation][4]
*   [Create KML File Programmatically using C#][5]
*   [Read Features from KML files Programmatically using C#][6]

## Creating or Reading KML Files – API Installation {#section1}

[Aspose.GIS for .NET][7] API supports working with KML files along with several other [supported file formats][8]. Let us install the API to manipulate the vector files in .NET based applications. You need to download the API from [New Releases][9] section, or from [NuGet][10] gallery with the following installation command:

```
PM> Install-Package Aspose.GIS
```

After configuring the API, you are all set to create or manipulate KML files. Now you do not need to worry about minor details because you only need to make simple API calls. Let us move on to further details:

## Create KML File Programmatically using C# {#section2}

KML files follow the tag-based structure like the [XML][11] files. You can use KML files to pinpoint locations, planning or tracking your trips and many other important scenarios. You can create KML files programmatically using C# with below steps:

1.  Create a [layer][12]
2.  Initialize [feature][13] for geometry and attributes
3.  Set value of different attributes
4.  Add the feature to a specific Layer

The following code snippet is a basic and simple demonstration as how to create KML files programmatically in C#:

{{< gist aspose-com-gists 1b3c7212ef9fdf07d196eec8c1395f47 "Create-KML-file.cs" >}}

## Read Features from KML files Programmatically using C# {#section3}

The basic features of a KML file may include Placemarks, Descriptions, Paths, etc. Let us proceed with the KML file that we have created in above example. You can read any feature of a KML file with below steps:

1.  Load input KML file with [OpenLayer][14] method
2.  Get features’ count
3.  Access a [feature][15] at a specific index
4.  Read features of the KML file

The code snippet below shows how to read features from a KML file programmatically in C#:

{{< gist aspose-com-gists 1b3c7212ef9fdf07d196eec8c1395f47 "Read-KML-Features.cs" >}}

## Conclusion

In this article, we have explored how to work with KML files. We have learned how to create a KML file or read its features programmatically with the help of C# sample code. Likewise, you can explore how to work with several other GIS file formats. You may visit [Product Documentation][16] or write to us at [Free Support Forum][17] to discuss any of your concerns. We would love to assist you!

## See Also

[Render Basic Map and Export to SVG using C#][18]




[1]: https://docs.fileformat.com/gis/kml/
[2]: https://docs.fileformat.com/gis/
[3]: https://docs.fileformat.com/programming/cs/
[4]: #section1
[5]: #section2
[6]: #section3
[7]: https://products.aspose.com/gis/net
[8]: https://docs.aspose.com/gis/net/supported-file-formats/
[9]: https://downloads.aspose.com/gis/net
[10]: https://www.nuget.org/packages/Aspose.Gis
[11]: https://docs.fileformat.com/web/xml/
[12]: https://apireference.aspose.com/gis/net/aspose.gis.formats.kml/kmldriver/methods/createlayer/index
[13]: https://apireference.aspose.com/gis/net/aspose.gis/featureattribute
[14]: https://apireference.aspose.com/gis/net/aspose.gis.formats.kml/kmldriver/methods/openlayer/index
[15]: https://apireference.aspose.com/gis/net/aspose.gis/feature
[16]: https://docs.aspose.com/gis/net/
[17]: https://forum.aspose.com/c/gis
[18]: https://blog.aspose.com/2019/05/20/basic-map-rendering-and-export-to-svg-using-aspose.gis-for-.net-19.4/





