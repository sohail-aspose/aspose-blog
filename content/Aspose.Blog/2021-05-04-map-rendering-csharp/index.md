---
title: 'Map Rendering to SVG, JPG, or PNG Image using C#'
seoTitle: "Map Rendering to SVG, JPG, or PNG Image using C# | Shapefile GeoTIFF"
description: "Map rendering can be used to render geospatial infromation from Shapefile, GeoTiff files to SVG, PNG, TIFF, programmatically using C# .NET."
date: Tue, 04 May 2021 14:45:00 +0000
draft: false
url: /2021/05/04/map-rendering-csharp/
author: Farhan Raza
summary: 'Map Rendering refers to making visual maps from geospatial data. You can render maps from KML, GeoJSON, GeoTIFF, as well as the Shapefile. You can render maps to different image formats like PNG, SVG, JPG, etc. The following sections explain map rendering in detail.'
tags: ['Map rendering to svg', 'geotiff to svg', 'map rendering to jpg', 'map rendering to png', 'render map in csharp', 'shapefile to image']
categories: ['Aspose.GIS Product Family']
---



{{< figure align=center src="images/Map-Rendering.png" alt="Map rendering">}}


Map Rendering refers to making visual maps from geospatial data. You can render maps from [KML][1], [GeoJSON][2], GeoTIFF, as well as the [Shapefile][3] to different file formats. You can render maps to different image formats like [PNG][4], [SVG][5], [JPG][6], etc. The following sections will elaborate the map rendering to images:

*   [Map Rendering from a Shapefile to Images – C# API Installation][7]
*   [Render Map from Shapefile to SVG Programmatically using C#][8]
*   [Render Map from Shapefile to PNG Image Programmatically in C#][9]
*   [Custom Map Rendering with Advance Style using C#][10]
*   [Render Map from GeoTIFF format to SVG Programmatically using C#][11]

## Map Rendering from a Shapefile to Images – C# API Installation {#section1}

[Aspose.GIS for .NET][12] API lets you work with different geographical and geo-spatial file formats. You can render maps from supported file formats to SVG, PNG, and other file formats as per your requirements. Please configure the API by downloading it from the [New Releases][13] section, or you can use the following [NuGet][14] installation command on the package manager console.

```
PM> Install-Package Aspose.GIS
```

## Render Map from Shapefile to SVG Programmatically using C# {#section2}

You can render map from a shapefile to an SVG file with the following steps:

1.  Create a new instance of the [Map][15] class.
2.  Create a vector map layer and add it to the map.
3.  Render the map into a file.

The code below elaborates how to render a map from a Shapefile to SVG programmatically using C#;

{{< gist aspose-com-gists bec62bc052abf4345db42913308dc663 "shapefile-svg.cs" >}}

## Render Map from Shapefile to PNG Image Programmatically in C# {#section3}

You can render map from a shapefile to raster image formats like PNG, JPG, BMP, etc. The following are the steps for rendering map from shapefile to PNG image:

1.  Initialize [Map][16] class object with dimensions.
2.  Create and add a vector map layer.
3.  Render the map to a PNG image.

The following code shows map rendering from Shapefile to PNG image programmatically using C#:

{{< gist aspose-com-gists bec62bc052abf4345db42913308dc663 "shapefile-png.cs" >}}

## Custom Map Rendering with Advance Style using C# {#section4}

You can customize the appearance of a map with advance feature styles. Please follow the steps below for custom map rendering:

1.  Initialize [Map][17] class object.
2.  Initialize [SimpleFill][18] for a simple polygon symbolizer.
3.  Open the layer from the input shapefile for reading.
4.  Render the map into a file.

The code below explains how to do custom map rendering with advanced style using C#:

{{< gist aspose-com-gists bec62bc052abf4345db42913308dc663 "custom-map-rendering.cs" >}}

## Render Map from GeoTIFF format to SVG Programmatically using C# {#section5}

You can render a map from GeoTIFF to SVG file with the following steps:

1.  Instantiate [Map][19] class object.
2.  Open the layer for reading using the driver for the GeoTIFF or TIFF format.
3.  Render map into a file.

The code snippet below demonstrates how to render map from GeoTIFF format to SVG programmatically using C#:

{{< gist aspose-com-gists bec62bc052abf4345db42913308dc663 "GeoTIFF-SVG.cs" >}}

## Get Free API License {#section6}

You can evaluate the API with a [Free Temporary License][20] for testing the API without any limitations.

## Conclusion

In this article, you have learned map rendering from shapefile or GeoTIFF format to SVG, or other raster image formats like PNG, JPG, TIFF, etc. You can explore other features of the API by visiting the [Documentation][21]. Please feel free to contact us via [Free Support Forum][22] in case of any queries.

## See Also

[Create KML File or Read its Features Programmatically using C#][23]




[1]: https://docs.fileformat.com/gis/kml/
[2]: https://docs.fileformat.com/gis/geojson/
[3]: https://docs.fileformat.com/gis/shp/
[4]: https://docs.fileformat.com/image/png/
[5]: https://docs.fileformat.com/page-description-language/svg/
[6]: https://docs.fileformat.com/image/jpeg/
[7]: #section1
[8]: #section2
[9]: #section3
[10]: #section4
[11]: #section5
[12]: https://products.aspose.com/gis/net
[13]: https://downloads.aspose.com/gis/net
[14]: https://www.nuget.org/packages/Aspose.GIS/
[15]: https://apireference.aspose.com/gis/net/aspose.gis.rendering/map
[16]: https://apireference.aspose.com/gis/net/aspose.gis.rendering/map
[17]: https://apireference.aspose.com/gis/net/aspose.gis.rendering/map
[18]: https://apireference.aspose.com/gis/net/aspose.gis.rendering.symbolizers/simplefill
[19]: https://apireference.aspose.com/gis/net/aspose.gis.rendering/map
[20]: https://purchase.aspose.com/temporary-license
[21]: https://docs.aspose.com/gis/net/
[22]: https://forum.aspose.com/c/gis/33
[23]: https://blog.aspose.com/2021/01/18/create-KML-Read-Features-csharp/





