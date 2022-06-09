---
title: 'Read GPX Files using C#'
seoTitle: "Read GPX Files using C# | Read Features from GPX File using C#"
description: "Programmatically read GPX files using C# with Aspose.GIS for .NET API. Read features, points, and geometries from GPX files in your .NET applications."
date: Fri, 06 May 2022 13:33:54 +0000
draft: false
url: /2022/05/06/read-gpx-files-using-csharp/
author: Muzammil Khan
summary: 'As a C# developer, you can easily read GPX files and extract GPS data such as waypoints, tracks, routes, etc. In this article, you will learn **how to read GPX files using C#**.'
tags: ['C# API to Read GPX files', 'Extract GPS from GPX C#', 'GPX', 'GPX in C#', 'Load GPX C#', 'Read Features from GPX File using C#', 'Read GPX files in C#', 'Read Points from GPX C#', 'Read Routes from GPX C#', 'Read Tracks from GPX C#']
categories: ['Aspose.GIS Product Family']
---



{{< figure align=center src="images/read-gpx-files-using-csharp.jpg" alt="Read GPX Files using C#">}}


A [GPX][1] file contains GPS data saved in GPS Exchange Format. It is an XML schema to describe geographic information such as waypoints, tracks, routes, etc. It allows transferring GPS data between GPS units and software applications. We can easily load the GPX file and extract GPS information programmatically in .NET applications. In this article, we will learn **how to read GPX files using C#**.

The article shall cover the following topics:

*   [C# API to Read GPX Files][2]
*   [Read Waypoints from the GPX File][3]
*   [Read Routes from the GPX File][4]
*   [Extract Tracks from GPX File][5]
*   [Read GPX Nested Attributes][6]

## C# API to Read GPX Files {#CSharp-API-to-Read-GPX-Files}

For reading features from GPX files, we will be using the [Aspose.GIS for .NET][7] API. It allows you to render maps, and create, read, and convert geographic data without additional software. It also enables you to convert KML files to GPX format and vice versa. Please either [download][8] the DLL of the API or install it using [NuGet][9].

```
PM> Install-Package Aspose.GIS
```

## Read Waypoints from the GPX File in C# {#Read-Waypoints-from-the-GPX-File-in-CSharp}

We can read waypoints from the GPX file as Point Geometry by following the steps given below:

1.  Firstly, load the GPX file using the [OpenLayer][10] method.
2.  Next, for each feature in the layer, check if [GeometryType][11] is [Point][12].
3.  After that, get the geometry of the feature as a **_Point_**.
4.  Finally, show X and Y coordinate points.

The following code sample shows **how to read waypoints from a GPX file using C#**.

{{< gist aspose-com-gists 9d89bd3d5ce5d0447a62b629d0fc2337 "ReadGPXFiles_CSharp_ReadWayPoints.cs" >}}

```
POINT (-90.29408 38.63473) X: -90.29408 Y: 38.63473
POINT (-90.28679 38.63368) X: -90.28679 Y: 38.63368
POINT (-90.29323 38.63408) X: -90.29323 Y: 38.63408
POINT (-90.29019 38.63533) X: -90.29019 Y: 38.63533
POINT (-90.28976 38.63677) X: -90.28976 Y: 38.63677
POINT (-90.28948 38.63496) X: -90.28948 Y: 38.63496
POINT (-90.29458 38.63421) X: -90.29458 Y: 38.63421
POINT (-90.29083 38.63633) X: -90.29083 Y: 38.63633
POINT (-90.28715 38.63395) X: -90.28715 Y: 38.63395
POINT (-90.28769 38.63347) X: -90.28769 Y: 38.63347
```

## Read Routs from the GPX File in C# {#Read-Routs-from-the-GPX-File-in-CSharp}

We can read routes from the GPX file as Line String geometry by following the steps given below:

1.  Firstly, load the GPX file using the [OpenLayer][13] method.
2.  Next, for each feature in the layer, check if [GeometryType][14] is [LineString][15].
3.  After that, get the geometry of the feature as **_LineString_**.
4.  Finally, show X, Y, and Z coordinate points.

The following code sample shows **how to read routes from a GPX file using C#**.

{{< gist aspose-com-gists 9d89bd3d5ce5d0447a62b629d0fc2337 "ReadGPXFiles_CSharp_ReadRoutes.cs" >}}

```
=====================================================
 X: -4.03601769647726 Y: 56.6758328268945 Z: 351.247702398777
 X: -4.03583038137853 Y: 56.6753865835736 Z: 344.690721458414
 X: -4.03614000315429 Y: 56.6735618299578 Z: 349.066837113628
 X: -4.03711323311608 Y: 56.6726922276694 Z: 352.76479861559
 X: -4.03921535478461 Y: 56.6708156570976 Z: 358.078238232484
 X: -4.04184722532733 Y: 56.668930361342 Z: 371.315914270806
 X: -4.04446052766014 Y: 56.668213511889 Z: 372.334546538997
 X: -4.04552528394144 Y: 56.6682858833434 Z: 398.610199355698
 X: -4.04660281552745 Y: 56.6678413316366 Z: 439.24188764472
 X: -4.04765411258453 Y: 56.6661616045966 Z: 430.695575764036
.
.
.
```

## Extract Tracks from the GPX File in C# {#Extract-Tracks-from-the-GPX-File-in-CSharp}

We can read tracks from the GPX file as MultiLineString geometry by following the steps given below:

1.  Firstly, load the GPX file using the [OpenLayer][16] method.
2.  Next, for each feature in the layer, check if [GeometryType][17] is [MultiLineString][18].
3.  After that, get the geometry of the feature as **_MultiLineString_**.
4.  Finally, show the tracks.

The following code sample shows **how to read tracks from a GPX file using C#**.

{{< gist aspose-com-gists 9d89bd3d5ce5d0447a62b629d0fc2337 "ReadGPXFiles_CSharp_ReadTracks.cs" >}}

```
LINESTRING (0 0, 1 1, 2 2, 3 3)
LINESTRING EMPTY
LINESTRING EMPTY
LINESTRING (10 10, 11 11, 12 12, 13 13)
```

## Read GPX Nested Attributes in C# {#Read-GPX-Nested-Attributes-in-CSharp}

We can read features for each point in the segment and extract nested attribute values by following the steps given below:

1.  Firstly, create an instance of the [GpxOptions][19] class.
2.  Next, set the **_ReadNestedAttributes_** to true.
3.  Then, load the GPX file using the [OpenLayer()][20] method with the **_GpxOptions_** object as an argument.
4.  Next, for each feature in the layer, check if [GeometryType][21] is [MultiLineString][22].
5.  Then, get the geometry of the feature as **_MultiLineString_**.
6.  After that, read the segment as **_LineString_** from each **_MultiLineString_**.
7.  Finally, read points in the segment and show the attribute values.

The following code sample shows **how to read GPX nested attributes from a GPX file using C#**.

{{< gist aspose-com-gists 9d89bd3d5ce5d0447a62b629d0fc2337 "ReadGPXFiles_CSharp_ReadGPSNestedAttributes.cs" >}}

## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][23] to try the library without evaluation limitations.

## Conclusion

In this article, we have learned how to:

*   load a GPX file using OpenLayer in C#;
*   read waypoints, routes, and tracks from the GPX file programmatically;
*   read the nested attribute from a GPX file using C#.

Besides, you can learn more about Aspose.GIS for .NET API using the [documentation][24]. In case of any ambiguity, please feel free to contact us on the [forum][25].

## See Also

*   [Convert KML to GPX and GPX to KML using C#][26]
*   [Read Vector Layer Features, Points, and Geometries from CSV Files][27]




[1]: https://docs.fileformat.com/gis/gpx/
[2]: #CSharp-API-to-Read-GPX-Files
[3]: #Read-Waypoints-from-the-GPX-File-in-CSharp
[4]: #Read-Routs-from-the-GPX-File-in-CSharp
[5]: #Extract-Tracks-from-the-GPX-File-in-CSharp
[6]: #Read-GPX-Nested-Attributes-in-CSharp
[7]: https://products.aspose.com/gis/net/
[8]: https://downloads.aspose.com/gis/net
[9]: https://www.nuget.org/packages/Aspose.GIS/
[10]: https://apireference.aspose.com/gis/net/aspose.gis.filedriver/openlayer/methods/2
[11]: https://apireference.aspose.com/gis/net/aspose.gis.geometries/geometrytype
[12]: https://apireference.aspose.com/gis/net/aspose.gis.geometries/point
[13]: https://apireference.aspose.com/gis/net/aspose.gis.filedriver/openlayer/methods/2
[14]: https://apireference.aspose.com/gis/net/aspose.gis.geometries/geometrytype
[15]: https://apireference.aspose.com/gis/net/aspose.gis.geometries/linestring
[16]: https://apireference.aspose.com/gis/net/aspose.gis.filedriver/openlayer/methods/2
[17]: https://apireference.aspose.com/gis/net/aspose.gis.geometries/geometrytype
[18]: https://apireference.aspose.com/gis/net/aspose.gis.geometries/multilinestring
[19]: https://apireference.aspose.com/gis/net/aspose.gis.formats.gpx/gpxoptions
[20]: https://apireference.aspose.com/gis/net/aspose.gis.formats.gpx.gpxdriver/openlayer/methods/2
[21]: https://apireference.aspose.com/gis/net/aspose.gis.geometries/geometrytype
[22]: https://apireference.aspose.com/gis/net/aspose.gis.geometries/multilinestring
[23]: https://purchase.aspose.com/temporary-license
[24]: https://docs.aspose.com/gis/net/
[25]: https://forum.aspose.com/c/gis/33
[26]: https://blog.aspose.com/2021/11/19/convert-kml-to-gpx-and-gpx-to-kml-using-csharp/
[27]: https://blog.aspose.com/2021/11/05/read-vector-layer-features-points-and-geometries-from-csv-files/




