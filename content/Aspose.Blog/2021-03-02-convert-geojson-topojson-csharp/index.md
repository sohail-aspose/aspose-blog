---
title: 'Convert GeoJson to TopoJson and vice versa using C#'
seoTitle: "Convert GeoJson to TopoJson and vice versa Programmatically using C#"
description: "Convert GeoJSON to TopoJSON with or without quantization, as well as TopoJSON to GeoJSON programmatically using C# language. A converter in C#."
date: Tue, 02 Mar 2021 07:15:00 +0000
draft: false
url: /2021/03/02/convert-geojson-topojson-csharp/
author: Farhan Raza
summary: 'GeoJSON is used for representing geographical features with non-spatial features. Whereas, TopoJSON is an extension of GeoJSON that utilizes Topology. You can convert GeoJSON to TopoJSON as well as TopoJSON to GeoJSON as per your requirements.'
tags: ['convert geojson c#', 'convert topojson c#', 'geojson to topojson', 'topojson to geojson']
categories: ['Aspose.GIS Product Family']
---



{{< figure align=center src="images/convert-geojson-topojson-csharp.png" alt="convert-geojson-topojson-csharp">}}


[GeoJSON][1] is used for representing geographical features with non-spatial features. Whereas, TopoJSON is an extension of GeoJSON that utilizes Topology. You can convert GeoJSON to TopoJSON as well as TopoJSON to GeoJSON as per your requirements. Let us explore the following use cases in details:

*   [GeoJSON and TopoJSON inter-conversion – C# .NET API Installation][2]
*   [Convert GeoJSON to TopoJSON Programmatically using C#][3]
*   [Convert GeoJSON to TopoJSON with Quantization using C#][4]
*   [Convert TopoJSON to GeoJSON Programmatically in C#][5]

## GeoJSON and TopoJSON inter-conversion – C# .NET API Installation {#section1}

[Aspose.GIS for .NET][6] API can be used to manipulate or convert geographical data. You can easily configure the API by downloading its DLL file from the [Downloads][7] section, or via the [NuGet][8] gallery with the following installation command:

```
PM> Install-Package Aspose.GIS
```

## Convert GeoJSON to TopoJSON Programmatically using C# {#section2}

GeoJSON to TopoJSON file conversion is helpful because it encodes geospatial features and is smaller in file size. It is smaller in file size because of topology and eliminating redundancy. Furthermore, even when there is no shared topology, the fix-precision encoding is way more efficient than floating point encoding of GeoJSON file format. You can convert GeoJSON to TopoJSON with the following steps:

1.  Load input GeoJSON file
2.  Convert GeoJSON to TopoJSON

The following code snippet shows how to convert GeoJSON to TopoJSON programmatically using C#:

{{< gist aspose-com-gists 2da6c458edc3e9005980432ae333d3f6 "Convert-GeoJSON-to-TopoJSON.cs" >}}

## Convert GeoJSON to TopoJSON with Quantization using C# {#section3}

GeoJSON to TopoJSON conversion is popular because of the fixed-precision efficiency and lesser file size. Moreover, quantization reduces the precision of coordinates. Resultantly, it optimizes the file size by representing the coordinates as integers. So you can convert GeoJSON to TopoJSON with quantization with the steps below:

1.  Initialize [ConversionOptions][9] class object
2.  Specify Quantization Number
3.  Or set [Transform][10] property
4.  Convert GeoJSON to TopoJSON with quantization

The code below shows how to convert GeoJSON to TopoJSON with quantization. It explains two alternative approaches for the conversion:

{{< gist aspose-com-gists 2da6c458edc3e9005980432ae333d3f6 "Convert-GeoJSON-to-TopoJSON-quantization.cs" >}}

## Convert TopoJSON to GeoJSON Programmatically in C# {#section4}

Aspose.GIS for .NET API supports TopoJSON to GeoJSON file conversion. So you can add this feature in your .NET applications. Moreover, GeoJSON file are usually preferred in server-side manipulation of geometries which do not require topologies. You can follow the following steps for TopoJSON to GeoJSON conversion:

1.  Load input TopoJSON file
2.  Converting TopoJSON to GeoJSON

The following code shows how to convert TopoJSON to GeoJSON programmatically using C#:

{{< gist aspose-com-gists 2da6c458edc3e9005980432ae333d3f6 "Convert-TopoJSON-to-GeoJSON.cs" >}}

## Conclusion

In this article, you have learned the differences and suitability of GeoJSON and TopoJSON file formats. Moreover, you have explored how to convert them into each other as per your requirements. Aspose.GIS for .NET API can efficiently and quickly perform the inter-conversion in your applications. Furthermore, you can learn more by visiting the API [Documentation][11]. In case of any query or concerns, please feel free to write back to us at the [Free Support Forums][12].

## See Also

[Create KML File or Read its Features Programmatically using C#][13]




[1]: https://en.wikipedia.org/wiki/GeoJSON
[2]: #section1
[3]: #section2
[4]: #section3
[5]: #section4
[6]: https://products.aspose.com/gis/net
[7]: https://downloads.aspose.com/gis/net
[8]: https://www.nuget.org/packages/Aspose.GIS/
[9]: https://apireference.aspose.com/gis/net/aspose.gis/conversionoptions
[10]: https://apireference.aspose.com/gis/net/aspose.gis.formats.topojson/topojsonoptions/properties/transform
[11]: https://docs.aspose.com/gis/net/
[12]: https://forum.aspose.com/c/gis/33
[13]: https://blog.aspose.com/2021/01/18/create-KML-Read-Features-csharp/





