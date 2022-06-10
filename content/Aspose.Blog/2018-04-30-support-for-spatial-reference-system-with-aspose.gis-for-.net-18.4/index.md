---
title: 'Support for Spatial Reference System with Aspose.GIS for .NET 18.4'
date: Mon, 30 Apr 2018 13:52:22 +0000
draft: false
url: /2018/04/30/support-for-spatial-reference-system-with-aspose.gis-for-.net-18.4/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.GIS Product Family']
---



{{< figure align=center src="images/aspose_gis-for-net-128x128.png" alt="">}}


We are pleased to announce the release of [Aspose.GIS for .NET 18.4][1]. This month’s release brings exciting new feature of spatial reference system implementation for geo-spatial objects. The API allows to apply spatial reference system to vector layers as well as geometrical objects. For a detailed note on what is new and fixed, please visit the [release notes][2] section of API documentation.

## Support for Spatial Reference Systems

This month’s release introduces a new feature for supporting Spatial Reference Systems (SRS). After the launch of this API, this is the first time we have implemented support for  SRS. THE API not only lets you create new Datums but also generate new SRS with Custom parameters.

## Work with WKT using C#

Well-known text (WKT) is a text markup language for representing vector geometry objects on a map, spatial reference systems of spatial objects and transformations between spatial reference systems. Aspose.GIS API lets you create Spatial Reference System from WKT as well as export an existing SRS to WKT format. The following sample code shows creating SRS from WKT.

```
string wkt = @"
GEOGCS[""WGS 84"",
DATUM[""WGS_1984"",
SPHEROID[""WGS 84"",6378137,298.257223563,
AUTHORITY[""EPSG"",""7030""]],
AUTHORITY[""EPSG"",""6326""]],
PRIMEM[""Greenwich"",0,
AUTHORITY[""EPSG"",""8901""]],
UNIT[""degree"",0.01745329251994328,
AUTHORITY[""EPSG"",""9122""]],
AUTHORITY[""EPSG"",""4326""]]
";
var srs = SpatialReferenceSystem.CreateFromWkt(wkt);
```

## Create Vector Layer with SRS

You can also use the API to create a [vector layer with SRS][3]. The ProjectedSpatialReferenceSystemParameters lets you define the parameters for the SRS which are then used while creating new vector layer.

```
var parameters = new ProjectedSpatialReferenceSystemParameters
{
    Name = "WGS 84 / World Mercator",
    Base = SpatialReferenceSystem.Wgs84,
    ProjectionMethodName = "Mercator_1SP",
    LinearUnit = Unit.Meter,
    XAxis = new Axis("Easting", AxisDirection.East),
    YAxis = new Axis("Northing", AxisDirection.North),
    AxisesOrder = ProjectedAxisesOrder.XY,
};
parameters.AddProjectionParameter("central_meridian", 0);
parameters.AddProjectionParameter("scale_factor", 1);
parameters.AddProjectionParameter("false_easting", 0);
parameters.AddProjectionParameter("false_northing", 0);

var projectedSrs = SpatialReferenceSystem.CreateProjected(parameters, Identifier.Epsg(3395));

using (var layer = Drivers.Shapefile.Create(dataDir + "filepath_out.shp", new ShapefileOptions(), projectedSrs))
{
    var feature = layer.ConstructFeature();
    feature.Geometry = new Point(1, 2);
    layer.Add(feature);

    feature = layer.ConstructFeature();
} 
```

## Set the Spatial Reference System for Geometry

In addition to creating a vector layer with SRS, you can also set [SRS for a Geometry][4] like Point, Line, etc. The SpatialReferenceSystem property of Geometry objects let you set the SRS for the specified shape. In such case, child objects take the SRS of parent while parent’s object SRS is set to child’s on first point addition.

## API Resources

*   [Product Home Page][5] – Gives you detailed overview about Aspose.GIS for .NET API
*   [API Reference Guide][6] – Details the namespaces and classes of the API
*   [GitHub Examples][7] – Provides ready to run API Examples
*   [Support Forum][8] – Write to us if you have any query or inquiry about the API




[1]: https://www.nuget.org/packages/Aspose.GIS/
[2]: https://docs.aspose.com/display/gisnet/Aspose.GIS+for+.NET+18.4+Release+Notes
[3]: https://docs.aspose.com/gis/net/developer-guide/
[4]: https://docs.aspose.com/gis/net/developer-guide/
[5]: https://products.aspose.com/gis/net
[6]: https://apireference.aspose.com/net/gis
[7]: https://github.com/aspose-gis/Aspose.GIS-for-.NET
[8]: https://forum.aspose.com/c/gis




