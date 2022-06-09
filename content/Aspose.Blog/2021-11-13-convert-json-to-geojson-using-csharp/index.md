---
title: 'Convert JSON to GeoJSON using C#'
seoTitle: "Convert JSON to GeoJSON using C# | JSON to GeoJSON"
description: "Learn how to convert JSON to GeoJSON using C#. Use the GIS .NET API to convert your JSON files to GeoJSON format with just a few lines of code."
date: Sat, 13 Nov 2021 08:39:21 +0000
draft: false
url: /2021/11/13/convert-json-to-geojson-using-csharp/
author: Muhammad Ahmad
summary: 'There might be situations where you need to convert JSON files to GeoJSON. If you have multiple files, doing this task programmatically will prove to be helpful. To that end, this article will teach you **how to convert JSON files to GeoJSON using C#**.'
tags: ['Convert JSON to GeoJSON C#', 'JSON to GeoJSON', 'JSON to GeoJSON C#']
categories: ['Aspose.GIS Product Family']
---

There might be situations where you need to convert JSON files to GeoJSON. If you have multiple files, doing this task programmatically will prove to be helpful. To that end, this article will teach you **how to convert JSON files to GeoJSON using C#**.

*   [C# API for Converting JSON to GeoJSON][1]
*   [Convert JSON to GeoJSON using C#][2]

## C# API for Converting JSON to GeoJSON {#CSharp-API-for-Converting-JSON-to-GeoJSON}

[Aspose.GIS for .NET][3] API allows you to render maps and create, read, and convert geographic data without additional software. Furthermore, the API enables you to convert JSON to GeoJSON. You can either install the API through [NuGet][4] or download it directly from the [Downloads][5] section.

```
PM> Install-Package Aspose.GIS
```

## Convert JSON to GeoJSON using C# {#Convert-JSON-to-GeoJSON-using-CSharp}

The following are the steps to convert JSON to GeoJSON.

*   Create an instance of the [ConversionOptions][6] class.
*   Assign the [SpatialReferenceSystem.Wgs84][7] to the [ConversionOptions][8] object using the [DestinationSpatialReferenceSystem][9] property.
*   Convert the JSON to GeoJSON using the [VectorLayer.Convert(string sourcePath, FileDriver sourceDriver, string destinationPath, FileDriver destinationDriver, ConversionOptions options)][10] method.

The following sample code shows how to convert JSON to GeoJSON using C#

{{< gist aspose-com-gists e8b5629e0277795abe9a7c699fdfbe76 "Convert_JSON_To_GeoJSON.cs" >}}

## Get a Free License

In order to try the API without evaluation limitations, you can request [a free temporary license][11].

## Conclusion

In this article, you have learned how to convert JSON to GeoJSON using C#. The shared code snippet shows how to achieve this with just a few lines of code.  Aspose.GIS for .NET is a robust and feature-rich API that assists you in working with geospatial data. You can explore the API in detail by visiting the [official documentation][12]. In case of any questions, please feel free to reach us at our [free support forum][13].

## See Also

*   [Convert Shapefile to GeoJSON and GeoJSON to Shapefile using C#][14]




[1]: #CSharp-API-for-Converting-JSON-to-GeoJSON
[2]: #Convert-JSON-to-GeoJSON-using-CSharp
[3]: https://products.aspose.com/gis/net/
[4]: https://www.nuget.org/packages/Aspose.GIS/
[5]: https://downloads.aspose.com/gis/net
[6]: https://apireference.aspose.com/gis/net/aspose.gis/conversionoptions
[7]: https://apireference.aspose.com/gis/net/aspose.gis.spatialreferencing/spatialreferencesystem/properties/wgs84
[8]: https://apireference.aspose.com/gis/net/aspose.gis/conversionoptions
[9]: https://apireference.aspose.com/gis/net/aspose.gis/conversionoptions/properties/destinationspatialreferencesystem
[10]: https://apireference.aspose.com/gis/net/aspose.gis.vectorlayer/convert/methods/3
[11]: https://purchase.aspose.com/temporary-license
[12]: https://docs.aspose.com/gis/net/
[13]: https://forum.aspose.com/c/gis/33
[14]: https://blog.aspose.com/2021/11/11/convert-shapefile-to-geojson-and-geojson-to-shapefile-using-csharp/




