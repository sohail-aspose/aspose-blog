---
title: 'Read MapInfo TAB and MapInfo Interchange Files in C# with Aspose.GIS for .NET'
date: Mon, 11 Feb 2019 18:16:37 +0000
draft: false
url: /2019/02/11/read-mapinfo-tab-and-mapinfo-interchange-file-formats-with-aspose.gis/
author: Muhammad Ahmad
summary: ''
tags: []
categories: ['Aspose.GIS Product Family']
---



{{< figure align=center src="images/aspose_gis-for-net-128x128.png" alt="">}}


We are pleased to announce the release of [Aspose.GIS for .NET 19.2][1]. This release gives you the ability to work with MapInfo TAB and MapInfo Interchange file formats. For a complete list of what is new and fixed, please visit the [release notes][2] section of the API documentation.

## Read MapInfo TAB File in C#

The following code sample shows how to read MapInfo TAB files using C#:

```
string TestDataPath = RunExamples.GetDataDir();
using (var layer = Drivers.MapInfoTab.OpenLayer(Path.Combine
(TestDataPath, "data.tab")))
{
    Console.WriteLine($"Number of features is {layer.Count}.");

    var lastGeometry = layer[layer.Count - 1].Geometry;
    Console.WriteLine($"Last geometry is {lastGeometry.AsText()}.");

    foreach (Feature feature in layer)
    {
        Console.WriteLine(feature.Geometry.AsText());
    }
 }
```

## Read MapInfo Interchange File in C#

The following code sample shows how to read the MapInfo Interchange File in C#.

```
string TestDataPath = RunExamples.GetDataDir();
using (var layer = Drivers.MapInfoInterchange.OpenLayer(
Path.Combine(TestDataPath, "data.mif")))
{
    Console.WriteLine($"Number of features is {layer.Count}.");

    var lastGeometry = layer[layer.Count - 1].Geometry;
    Console.WriteLine($"Last geometry is {lastGeometry.AsText()}.");

    foreach (Feature feature in layer)
    {
        Console.WriteLine(feature.Geometry.AsText());
    }
}
```

The following API resources can be of help to you in getting started with Aspose.GIS:

## API Resources

*   [Product Home Page][3] – Gives you a detailed overview of Aspose.GIS for .NET API
*   [API Reference Guide][4] – Details the namespaces and classes of the API
*   [GitHub Examples][5] – Provides ready to run API Examples
*   [Support Forum][6] – Write to us if you have any query or inquiry about the API




[1]: https://www.nuget.org/packages/Aspose.GIS/19.2.0
[2]: https://docs.aspose.com/display/gisnet/Aspose.GIS+for+.NET+19.2+Release+Notes
[3]: https://products.aspose.com/gis/net
[4]: https://apireference.aspose.com/net/gis
[5]: https://github.com/aspose-gis/Aspose.GIS-for-.NET
[6]: https://forum.aspose.com/c/gis




