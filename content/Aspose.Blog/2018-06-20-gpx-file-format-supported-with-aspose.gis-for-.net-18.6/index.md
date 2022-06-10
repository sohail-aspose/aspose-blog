---
title: 'Work with GPX Files using C# with Aspose.GIS for .NET 18.6'
date: Wed, 20 Jun 2018 15:09:47 +0000
draft: false
url: /2018/06/20/gpx-file-format-supported-with-aspose.gis-for-.net-18.6/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.GIS Product Family']
---



{{< figure align=center src="images/aspose_gis-for-net-128x128.png" alt="">}}


We are excited to announce the release of [Aspose.GIS for .NET 18.6][1]. This new release of API introduces support for .NET Standard 2.0 which lets you use the API in a variety of other type of applications. This release also introduces a new feature of working with GPS Exchange Format (GPX) files. For a detailed note on what is new and fixed, please visit the [release notes][2] section of API documentation.

## Working with GPX Files using C#

This month’s release is not limited to providing support for additional Platforms. We are further pleased to share a new feature supported by the API where the API now provides the capability to [read GPS Exchange Format (GPX)][3] files. You can read the GPX files using the Gpx Drivers added to the API. Once loaded, you can:

*   Read waypoints from GPX file as Point Geometry of the API
*   Read routes from GPX file as Line String geometry
*   Read tracks from GPX file as Multi Line String geometry

```
using (var layer = Drivers.Gpx.Open(dataDir + "schiehallion.gpx"))
{
    foreach (var feature in layer)
    {
        switch (feature.Geometry.GeometryType)
        {
            // GPX waypoints are exported as features with point geometry.
            case GeometryType.Point:


                Console.WriteLine(feature.Geometry.Dimension);
                //HandleGpxWaypoint(feature);
                break;
            
            // GPX routes are exported as features with line string geometry.
            case GeometryType.LineString:

                //HandleGpxRoute(feature);
                LineString ls = (LineString)feature.Geometry;

                foreach (var point in ls)
                {
                    Console.WriteLine(point);
                }
                break;
            
                // GPX tracks are exported as features with multi line string geometry.
            // Every track segment is line string.
            case GeometryType.MultiLineString:

                //HandleGpxTrack(feature);
                Console.WriteLine(feature.Geometry);
                break;
            default: break;
        }
    }
}
```

## Support for .NET Standard 2.0 and Mono Framework

Our continuous efforts to expand the supported .NET Frameworks by the API, Aspose.GIS for .NET now supports .NET Standard 2.0. Just after five releases, we have achieved the ability to provide support for .NET Standard 2.0 on Windows as well as Linux. In addition, the API can also be used with Mono Framework on Windows and Linux.

## API Resources

*   [Product Home Page][4] – Gives you detailed overview about Aspose.GIS for .NET API
*   [API Reference Guide][5] – Details the namespaces and classes of the API
*   [GitHub Examples][6] – Provides ready to run API Examples
*   [Support Forum][7] – Write to us if you have any query or inquiry about the API




[1]: https://products.aspose.com/gis/net
[2]: https://docs.aspose.com/display/gisnet/Aspose.GIS+for+.NET+18.6+Release+Notes
[3]: https://docs.aspose.com/gis/net/
[4]: https://products.aspose.com/gis/net
[5]: https://apireference.aspose.com/net/gis
[6]: https://github.com/aspose-gis/Aspose.GIS-for-.NET
[7]: https://forum.aspose.com/c/gis




