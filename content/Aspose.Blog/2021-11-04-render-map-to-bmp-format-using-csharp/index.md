---
title: 'Render Map to BMP Format using C#'
seoTitle: "Render Map to BMP Format using C#"
description: "Map data can be available in different formats like KML, GeoTiff, GeoJSON, Shapefile, etc. There might be situations where you need to render the map data as BMP images. For that, this article will teach you how to render map data in BMP format using C#."
date: Thu, 04 Nov 2021 04:44:41 +0000
draft: false
url: /2021/11/04/render-map-to-bmp-format-using-csharp/
author: Muhammad Ahmad
summary: 'Map data can be available in different formats like KML, GeoTiff, GeoJSON, Shapefile, etc. There might be situations where you need to render the map data as BMP images. For that, this article will teach you **how to render map data in BMP format using C#**.'
tags: ['Add Marker with Custom Style to Map C#', 'Render Map as BMP C#', 'Render Map with Specific Projection C#']
categories: ['Aspose.GIS Product Family']
---

Map data can be available in different formats like KML, GeoTiff, GeoJSON, Shapefile, etc. There might be situations where you need to render the map data as BMP images. For that, this article will teach you **how to render map data in BMP format using C#**.

*   [C# API for Rendering Map to BMP Format][1]
*   [Render Map to BMP Format using C#][2]
*   [Rendering Map to Specific Projection using C#][3]
*   [Add Marker with Custom Style using C#][4]

## C# API for Rendering Map to BMP Format {#CSharp-API-for-Rendering-Map-to-BMP-Format}

We will use the [Aspose.GIS for .NET][5] API to render maps to BMP format. It is an API that supports working with geospatial data stored in various file formats. It also provides the ability to render maps and create, read, and convert geographic data without any additional software. You can either install the API through [NuGet][6] or download it directly from the [Downloads][7] section.

```
PM> Install-Package Aspose.GIS
```

## Render Map to BMP Format using C# {#Render-Map-to-BMP-Format-using-CSharp}

The following are the steps to render maps to BMP format.

*   Create an instance of the [Map][8] class.
*   Create a vector layer from the shapefile and add it to the map.
*   Render the map as a BMP using the [Map.Render(string outputPath, Renderer renderer)][9] method.

The following sample code shows how to render a map to BMP format using C#.

{{< gist aspose-com-gists feecc1fed3bf6a385dacf6b4ed0011fb "Map_To_BMP.cs" >}}

## Rendering Map to Specific Projection using C# {#Rendering-Map-to-Specific-Projection-using-CSharp}

The following are the steps to render a map to a specific projection.

*   Create an instance of the [Map][10] class.
*   Create a vector layer from the shapefile and add it to the map.
*   Set the map's spatial reference system using the [Map.SpatialReferenceSystem][11] property.
*   Save the map as a BMP image using the [Map.Render(string outputPath, Renderer renderer)][12] method.

The following sample code shows how to render a map to a specific projection using C#.

{{< gist aspose-com-gists feecc1fed3bf6a385dacf6b4ed0011fb "Map_To_Specific_Projection.cs" >}}

## Add Marker with Custom Style using C# {#Add-Marker-with-Custom-Style-using-CSharp}

The following are the steps to add a marker with custom style to a map.

*   Create an instance of the [Map][13] class.
*   Create an instance of the [SimpleMarker][14] class.
*   Set the properties of the [SimpleMarker][15] object according to your requirements.
*   Create a vector layer from the geojson file and add it to the map along with the markers.
*   Save the map as a BMP image using the [Map.Render(string outputPath, Renderer renderer)][16] method.

The following sample code shows how to add a custom-style marker to a map using C#.

{{< gist aspose-com-gists feecc1fed3bf6a385dacf6b4ed0011fb "Add_Marker_With_Custom_Style.cs" >}}

## Get a Free License

In order to try the API without evaluation limitations, you can request [a free temporary license][17].

## Conclusion

In this article, you have learned how to render map data as BMP images using C#. Moreover, you have seen how to set the map projections and add markers with custom styling. Aspose.GIS for .NET is a robust API that provides a bunch of additional features for working with map data. You can explore the API in detail by visiting the [official documentation][18]. In case of any questions, please feel free to reach us at our [free support forum][19].

## See Also

*   [Read Features from OpenStreetMap (OSM) Files using C#][20]




[1]: #CSharp-API-for-Rendering-Map-to-BMP-Format
[2]: #Render-Map-to-BMP-Format-using-CSharp
[3]: #Rendering-Map-to-Specific-Projection-using-CSharp
[4]: #Add-Marker-with-Custom-Style-using-CSharp
[5]: https://products.aspose.com/gis/net/
[6]: https://www.nuget.org/packages/Aspose.GIS/
[7]: https://downloads.aspose.com/gis/net
[8]: https://apireference.aspose.com/gis/net/aspose.gis.rendering/map
[9]: https://apireference.aspose.com/gis/net/aspose.gis.rendering.map/render/methods/1
[10]: https://apireference.aspose.com/gis/net/aspose.gis.rendering/map
[11]: https://apireference.aspose.com/gis/net/aspose.gis.rendering/map/properties/spatialreferencesystem
[12]: https://apireference.aspose.com/gis/net/aspose.gis.rendering.map/render/methods/1
[13]: https://apireference.aspose.com/gis/net/aspose.gis.rendering/map
[14]: https://apireference.aspose.com/gis/net/aspose.gis.rendering.symbolizers/simplemarker
[15]: https://apireference.aspose.com/gis/net/aspose.gis.rendering.symbolizers/simplemarker
[16]: https://apireference.aspose.com/gis/net/aspose.gis.rendering.map/render/methods/1
[17]: https://purchase.aspose.com/temporary-license
[18]: https://docs.aspose.com/gis/net/
[19]: https://forum.aspose.com/c/gis/33
[20]: https://blog.aspose.com/2021/08/23/read-features-from-open-street-map-osm-files-using-csharp/




