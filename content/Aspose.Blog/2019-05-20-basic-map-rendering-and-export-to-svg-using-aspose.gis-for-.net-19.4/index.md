---
title: 'Render Basic Map and Export to SVG using C#'
date: Mon, 20 May 2019 23:12:31 +0000
draft: false
url: /2019/05/20/basic-map-rendering-and-export-to-svg-using-aspose.gis-for-.net-19.4/
author: Ahsaniqbal
summary: ''
tags: []
categories: ['Aspose.GIS Product Family']
---



{{< figure align=center src="images/aspose_gis-for-net-128x128.png" alt="">}}


So when we talk about some GIS API, rendering advanced map files seems to be the first thing which comes in mind. Good news is that the new release  [Aspose.GIS for .NET 19.4][1] contains this feature. This is not all about this release as there are many other upgrades as well. You should go through the [release notes][2] to get a complete list of what is new and fixed. Let us see what is inspiring there in this release.

## Redner Basic Map using C#

It seems you were waiting since long to render maps using Aspose.GIS and that's it, the wait is over as this feature is provided in the latest API to render [Shapefile][3], [FileGDB][4], [GeoJSON][5], [KML][6] or other [supported file formats][7] to [SVG][8]. We have put special effort to keep this process simple i.e. render maps using very few lines of code for the sake of simplicity and quick results without setting a large number of properties. Just have a look at how simple is it to render a map using [C#][9].

{{< gist aspose-com-gists 10f3783b9581d10bc69dbada42705d2c "Examples-CSharp-Rendering-RenderMap-RenderWithDefaultSettings.cs" >}}

See how easy it is by just setting the resultant image resolution, selecting the driver according to the input file type and that's all. The map is ready to render as SVG.

Here is the output of the program:



{{< figure align=center src="images/Screenshot-2019-05-16-at-9.21.32-PM-1024x533.png" alt="">}}


You may be worried about the look and feel like its just a black and white blueprint. Is this the new feature that was awaited for long? No! this is just the simplest output to show the functionality. You can customize rendering and feature styles in order to achieve the look you want. Here is an advanced sample code demonstrating more features in this new release.

{{< gist aspose-com-gists 10f3783b9581d10bc69dbada42705d2c "Examples-CSharp-Rendering-RenderMap-AddMapLayersAndStyles.cs" >}}

Let us see how the styles will change the output using the above sample code:



{{< figure align=center src="images/Screenshot-2019-05-16-at-9.45.54-PM-1024x612.png" alt="">}}


Wow! great. Now you can start working with this feature using your sample maps. Is it?

To understand the details of the code please visit [this][10] article in the documentation section.

## Datum Conversion Due to Incomplete SRS WKT

Aspose.GIS has introduced a new feature of converting between datums when SRS WKT definition is not complete. In order to transform between geographic SRS, TO\_WGS84 parameters are required. If they are present in WKT definition, Aspose.GIS can transform between any geographic SRSs. If they are not present, Aspose.GIS tries to detect TO\_WGS84 parameters by SRS name. If this fails, Aspose.GIS tries to find SRS with the same parameters and similar datum name, in order to take TO\_WGS84 parameters from a similar SRS.

## Other upgradations

The following up gradations are done to make the library more user friendly and error-free.

*   Some extra content at the end of the document was reported while overwriting an existing file. This problem is no more there.
*   There were some issues while specifying paths in the same folder as the executable, however, this issue is resolved now.
*   There were instances where misleading error messages were thrown for a missing file. It was like "Unexpected end of file" which was not indicating the actual issue. This message is corrected now.
*   There was an un-necessary constructor in the GPX driver class which is removed now to avoid any confusion.

I hope you got a fair idea about this new release. Enjoy using this latest version and share your thoughts to enhance it on our support forum.

## API Resources

*   [API Reference Guide][11] – Details the namespaces and classes of the API
*   [GitHub Examples][12] – Provides ready to run API Examples
*   [Support Forum][13] – Write to us if you have any query or inquiry about the API




[1]: https://www.nuget.org/packages/Aspose.GIS/19.4.0
[2]: https://docs.aspose.com/display/gisnet/Aspose.GIS+for+.NET+19.4+Release+Notes
[3]: https://docs.fileformat.com/gis/shp/
[4]: https://docs.fileformat.com/gis/filegdb/
[5]: https://docs.fileformat.com/gis/geojson/
[6]: https://docs.fileformat.com/gis/kml/
[7]: https://docs.aspose.com/display/gisnet/Supported+File+Formats
[8]: https://docs.fileformat.com/page-description-language/svg/
[9]: https://docs.fileformat.com/programming/cs/
[10]: https://docs.aspose.com/display/gisnet/Map+Rendering
[11]: https://apireference.aspose.com/net/gis
[12]: https://github.com/aspose-gis/Aspose.GIS-for-.NET
[13]: https://forum.aspose.com/c/gis




