---
title: 'Convert KML to GPX and GPX to KML using C#'
seoTitle: "Convert KML to GPX and GPX to KML using C# | KML to GPX"
description: "Learn how to convert KML files to GPX format and GPX files to KML format using C# with the simple and easy-to-use Aspose.GIS for .NET API."
date: Fri, 19 Nov 2021 19:44:30 +0000
draft: false
url: /2021/11/19/convert-kml-to-gpx-and-gpx-to-kml-using-csharp/
author: Muhammad Ahmad
summary: 'There might be situations where you need to convert [KML][1] files to [GPX][2] format or vice versa. For such cases, this article will teach you **how to convert KML files to GPX format and GPX files to KML format using C#**.'
tags: ['Convert GPX to KML C#', 'Convert KML to GPX C#', 'GPX to KML', 'KML to GPX']
categories: ['Aspose.GIS Product Family']
---

There might be situations where you need to convert [KML][3] files to [GPX][4] format or vice versa. For such cases, this article will teach you **how to convert KML files to GPX format and GPX files to KML format using C#**.

*   [C# API for Converting KML to GPX and Vice Versa][5]
*   [Converting KML Files to GPX Format using C#][6]
*   [Converting GPX Files to KML Format using C#][7]

## C# API for Converting KML to GPX and Vice Versa {#CSharp-API-for-Converting-KML-to-GPX-and-Vice-Versa}

[Aspose.GIS for .NET][8] API allows you to render maps and create, read, and convert geographic data without additional software. Furthermore, the API allows you to convert KML files to GPX format and vice versa. You can either install the API through [NuGet][9] or download it directly from the [Downloads][10] section.

```
PM> Install-Package Aspose.GIS
```

## Convert KML Files to GPX Format using C# {#Convert-KML-Files-to-GPX-Format-using-CSharp}

The following are the steps to convert KML files to GPX format.

*   Create an instance of the [ConversionOptions][11] class.
*   Assign the [SpatialReferenceSystem.Wgs84][12] to the [ConversionOptions][13] object using the [DestinationSpatialReferenceSystem][14] property.
*   Convert the KML file to GPX format using the [VectorLayer.Convert(string sourcePath, FileDriver sourceDriver, string destinationPath, FileDriver destinationDriver, ConversionOptions options)][15] method.

The following sample code shows how to convert KML files to GPX format using C#.

{{< gist aspose-com-gists b477704606d99159e2fc23ae7c7c5105 "Convert_KML_To_GPX.cs" >}}

## Converting GPX Files to KML Format using C# {#Converting-GPX-Files-to-KML-Format-using-CSharp}

The following are the steps to convert GPX files to KML format.

*   Create an instance of the [ConversionOptions][16] class.
*   Assign the [SpatialReferenceSystem.Wgs84][17] to the [ConversionOptions][18] object using the [DestinationSpatialReferenceSystem][19] property.
*   Convert the GPX file to KML format using the [VectorLayer.Convert(string sourcePath, FileDriver sourceDriver, string destinationPath, FileDriver destinationDriver, ConversionOptions options)][20] method.

The following sample code shows how to convert a GPX file to KML format using C#.

{{< gist aspose-com-gists b477704606d99159e2fc23ae7c7c5105 "Convert_GPX_To_KML.cs" >}}

## Get a Free License

In order to try the API without evaluation limitations, you can request [a free temporary license][21].

## Conclusion

In this article, you have learned how to convert KML files to GPX format and vice versa using C#. The shared code snippets demonstrate how to achieve these conversions with just a few lines of code. Aspose.GIS for .NET is a powerful and feature-rich API that assists you in working with geospatial data. You can explore the API in detail by visiting the [official documentation][22]. In case of any questions, please feel free to reach us at our [free support forum][23].

## See Also

*   [Convert KML to GeoJSON and GeoJSON to KML using C#][24]




[1]: https://docs.fileformat.com/gis/kml/
[2]: https://docs.fileformat.com/gis/gpx/
[3]: https://docs.fileformat.com/gis/kml/
[4]: https://docs.fileformat.com/gis/gpx/
[5]: #CSharp-API-for-Converting-KML-to-GPX-and-Vice-Versa
[6]: #Convert-KML-Files-to-GPX-Format-using-CSharp
[7]: #Converting-GPX-Files-to-KML-Format-using-CSharp
[8]: https://products.aspose.com/gis/net/
[9]: https://www.nuget.org/packages/Aspose.GIS/
[10]: https://downloads.aspose.com/gis/net
[11]: https://apireference.aspose.com/gis/net/aspose.gis/conversionoptions
[12]: https://apireference.aspose.com/gis/net/aspose.gis.spatialreferencing/spatialreferencesystem/properties/wgs84
[13]: https://apireference.aspose.com/gis/net/aspose.gis/conversionoptions
[14]: https://apireference.aspose.com/gis/net/aspose.gis/conversionoptions/properties/destinationspatialreferencesystem
[15]: https://apireference.aspose.com/gis/net/aspose.gis.vectorlayer/convert/methods/3
[16]: https://apireference.aspose.com/gis/net/aspose.gis/conversionoptions
[17]: https://apireference.aspose.com/gis/net/aspose.gis.spatialreferencing/spatialreferencesystem/properties/wgs84
[18]: https://apireference.aspose.com/gis/net/aspose.gis/conversionoptions
[19]: https://apireference.aspose.com/gis/net/aspose.gis/conversionoptions/properties/destinationspatialreferencesystem
[20]: https://apireference.aspose.com/gis/net/aspose.gis.vectorlayer/convert/methods/3
[21]: https://purchase.aspose.com/temporary-license
[22]: https://docs.aspose.com/gis/net/
[23]: https://forum.aspose.com/c/gis/33
[24]: https://blog.aspose.com/2021/11/18/convert-kml-to-geojson-and-geojson-to-kml-using-csharp/




