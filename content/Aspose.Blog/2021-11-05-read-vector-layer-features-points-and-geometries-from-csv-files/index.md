---
title: 'Read Vector Layer Features, Points, and Geometries from CSV Files'
seoTitle: "Read Vector Layer Features, Points, and Geometries from CSV Files"
description: "Use the Aspose.GIS for .NET API to read features, points, and geometries from vector layers in CSV files. Read geospatial data from CSV files."
date: Fri, 05 Nov 2021 20:28:06 +0000
draft: false
url: /2021/11/05/read-vector-layer-features-points-and-geometries-from-csv-files/
author: Muhammad Ahmad
summary: 'There might be situations where you have geospatial data in CSV format, and you want to read that data from within your .NET application. For such cases, this article will teach you **how to read vector layer features, points, and geometries from CSV files using C#**.'
tags: ['Read Features from CSV C#', 'Read Geometries from CSV C#', 'Read Points from CSV C#']
categories: ['Aspose.GIS Product Family']
---

There might be situations where you have geospatial data in CSV format, and you want to read that data from within your .NET applications. For such cases, this article will teach you **how to read vector layer features, points, and geometries from CSV files using C#**.

*   [C# API for Reading Vector Layer Features, Points, and Geometries from CSV Files][1]
*   [Read Features from CSV Files using C#][2]
*   [Reading Points from CSV Files using C#][3]
*   [Read Geometries from CSV Files using C#][4]

## C# API for Reading Vector Layer Features, Points, and Geometries from CSV Files {#CSharp-API-for-Reading-Vector-Layer-Features-Points-and-Geometries-from-CSV-Files}

[Aspose.GIS for .NET][5] API allows you to work with geospatial data stored in various file formats. It provides you the ability to render maps and create, read, and convert geographic data without additional software. Furthermore, the API allows you to read vector layer features, points, and geometries from CSV files. You can either install the API through [NuGet][6] or download it directly from the [Downloads][7] section.

```
PM> Install-Package Aspose.GIS
```

## Read Features from CSV Files using C# {#Read-Features-from-CSV-Files-using-CSharp}

The following are the steps to read features from a vector layer in a CSV file.

*   Load the CSV file using the [Drivers.Csv.OpenLayer(string path)][8] method.
*   Loop through the attributes and features in the layer and print their values.

The following sample code shows how to read features from a vector layer in a CSV file using C#.

{{< gist aspose-com-gists 504b09424d4da605ce3e21f1021cf957 "Read_Features_From_CSV.cs" >}}

## Reading Points from CSV Files using C# {#Reading-Points-from-CSV-Files-using-CSharp}

The following are the steps to read points from a vector layer in a CSV file.

*   Load the CSV file using the [Drivers.Csv.OpenLayer(string path, CsvOptions options)][9] method.
*   Set the [ColumnX][10], [ColumnY][11], [ColumnZ][12], and [ColumnM][13] properties of the [CsvOptions][14] object.
*   Loop through the features in the layer and print the points.

The following sample code shows how to read points from a vector layer in a CSV file using C#.

{{< gist aspose-com-gists 504b09424d4da605ce3e21f1021cf957 "Read_Points_From_CSV.cs" >}}

## Read Geometries from CSV Files using C# {#Read-Geometries-from-CSV-Files-using-CSharp}

The following are the steps to read geometries from the vector layer in a CSV file.

*   Load the CSV file using the [Drivers.Csv.OpenLayer(string path, CsvOptions options)][15] method.
*   Set the [ColumnWkt][16] property of the [CsvOptions][17] object.
*   Loop through the features in the layer and print the geometries to the console.

The following sample code shows how to read geometries from a vector layer in a CSV file using C#.

{{< gist aspose-com-gists 504b09424d4da605ce3e21f1021cf957 "Read_Geometries_From_CSV.cs" >}}

## Get a Free License

In order to try the API without evaluation limitations, you can request [a free temporary license][18].

## Conclusion

In this article, you have learned how to read features from CSV files using C#. Furthermore, you have seen how to read points and geometries from CSV files using Aspose.GIS for .NET API. It is a powerful API that provides many additional features for working with geospatial data. You can explore the API in detail by visiting the [official documentation][19]. In case of any questions, please feel free to reach us at our [free support forum][20].

## See Also

*   [Read Features from OpenStreetMap (OSM) Files using C#][21]




[1]: #CSharp-API-for-Reading-Vector-Layer-Features-Points-and-Geometries-from-CSV-Files
[2]: #Read-Features-from-CSV-Files-using-CSharp
[3]: #Reading-Points-from-CSV-Files-using-CSharp
[4]: #Read-Geometries-from-CSV-Files-using-CSharp
[5]: https://products.aspose.com/gis/net/
[6]: https://www.nuget.org/packages/Aspose.GIS/
[7]: https://downloads.aspose.com/gis/net
[8]: https://apireference.aspose.com/gis/net/aspose.gis.filedriver/openlayer/methods/2
[9]: https://apireference.aspose.com/gis/net/aspose.gis.formats.csv.csvdriver/openlayer/methods/2
[10]: https://apireference.aspose.com/gis/net/aspose.gis.formats.csv/csvoptions/properties/columnx
[11]: https://apireference.aspose.com/gis/net/aspose.gis.formats.csv/csvoptions/properties/columny
[12]: https://apireference.aspose.com/gis/net/aspose.gis.formats.csv/csvoptions/properties/columnz
[13]: https://apireference.aspose.com/gis/net/aspose.gis.formats.csv/csvoptions/properties/columnm
[14]: https://apireference.aspose.com/gis/net/aspose.gis.formats.csv/csvoptions
[15]: https://apireference.aspose.com/gis/net/aspose.gis.formats.csv.csvdriver/openlayer/methods/2
[16]: https://apireference.aspose.com/gis/net/aspose.gis.formats.csv/csvoptions/properties/columnwkt
[17]: https://apireference.aspose.com/gis/net/aspose.gis.formats.csv/csvoptions
[18]: https://purchase.aspose.com/temporary-license
[19]: https://docs.aspose.com/gis/net/
[20]: https://forum.aspose.com/c/gis/33
[21]: https://blog.aspose.com/2021/08/23/read-features-from-open-street-map-osm-files-using-csharp/




