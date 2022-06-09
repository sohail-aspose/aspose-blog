---
title: 'Export Features to a CSV File using C#'
seoTitle: "Export Features to a CSV File using C# | Add Features to CSV Layer"
description: "Learn how to export features to CSV files using C#. Use the .NET GIS API to add features to CSV layers within your .NET applications."
date: Tue, 09 Nov 2021 19:32:36 +0000
draft: false
url: /2021/11/09/export-features-to-a-csv-file-using-csharp/
author: Muhammad Ahmad
summary: 'There might be situations where you need to export features of a vector layer to a CSV file. For such cases, this article will teach you **how to export features to a CSV file using C#**.'
tags: ['Add Features to CSV Files C#', 'Export Features to CSV Files C#']
categories: ['Aspose.GIS Product Family']
---

There might be situations where you need to export features of a vector layer to a CSV file. For such cases, this article will teach you **how to export features to a CSV file using C#**.

*   [C# API for Exporting Features to a CSV File][1]
*   [Export Features to a CSV File][2]

## C# API for Exporting Features to a CSV File {#CSharp-API-for-Exporting-Features-to-a-CSV-File}

We will use the [Aspose.GIS for .NET][3] API to export features for a CSV file. It is an API that supports working with geospatial data stored in various file formats. It also provides the ability to render maps and create, read, and convert geographic data without any additional software. You can either install the API through [NuGet][4] or download it directly from the [Downloads][5] section.

```
PM> Install-Package Aspose.GIS
```

## Export Features to a CSV File using C# {#Export-Features-to-a-CSV-File-using-CSharp}

The following are the steps to export features to a CSV file.

*   Create the CSV file using the [Drivers.Csv.CreateLayer(string path, CsvOptions options)][6] method.
*   Add attributes to the layer using the [VectorLayer.Attributes.Add(FeatureAttribute attribute)][7] method.
*   Add features to the layer using the [VectorLayer.Add(Feature feature)][8] method.

The following sample code shows how to export features to a CSV file using C#.

{{< gist aspose-com-gists afa4cdd274f018b334b9dcd202c7a578 "Export_Features_To_CSV.cs" >}}

## Get a Free License

In order to try the API without evaluation limitations, you can request [a free temporary license][9].

## Conclusion

In this article, you have learned how to export features to a CSV file using C#. The shared code snippet demonstrates how to achieve this with just a few lines of code. Aspose.GIS for .NET is a robust API for working with geospatial data. You can explore the API in detail by visiting the [official documentation][10]. In case of any questions, please feel free to reach us at our [free support forum][11].

## See Also

*   [Read Vector Layer Features, Points, and Geometries from CSV Files][12]




[1]: #CSharp-API-for-Exporting-Features-to-a-CSV-File
[2]: #Export-Features-to-a-CSV-File-using-CSharp
[3]: https://products.aspose.com/gis/net/
[4]: https://www.nuget.org/packages/Aspose.GIS/
[5]: https://downloads.aspose.com/gis/net
[6]: https://apireference.aspose.com/gis/net/aspose.gis.formats.csv.csvdriver/createlayer/methods/3
[7]: https://apireference.aspose.com/gis/net/aspose.gis/featureattributecollection/methods/add
[8]: https://apireference.aspose.com/gis/net/aspose.gis/vectorlayer/methods/add
[9]: https://purchase.aspose.com/temporary-license
[10]: https://docs.aspose.com/gis/net/
[11]: https://forum.aspose.com/c/gis/33
[12]: https://blog.aspose.com/2021/11/05/read-vector-layer-features-points-and-geometries-from-csv-files/




