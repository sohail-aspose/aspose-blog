---
title: 'Set Locale and Create Reviewer using Aspose.Diagram for .NET and Java'
date: Sun, 02 Sep 2018 11:40:27 +0000
draft: false
url: /2018/09/02/support-for-setting-locale-and-creating-reviewer-in-aspose.diagram/
author: Asad Ali
summary: ''
tags: []
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose-Diagram-for-net_100.png" alt="">}}


We are pleased to announce the August release of Aspose.Diagram API with version 18.8 which is available for download and to be used in both .NET and Java Platforms. Various enhancements and bug fixes have been made to the library to improve its usability and performance. If you are planning to upgrade to latest version of the API, we strongly recommend you to go through the release notes section of both .NET and Java APIs in public API documentation. Release notes of the mentioned version of the API can be checked over following links:

*   [Aspose.Diagram for .NET 18.8 Release Notes][1]
*   [Aspose.Diagram for Java 18.8 Release Notes][2]

In order to download Aspose.Diagram 18.8 for .NET/Java, please visit the following links:

*   [Aspose.Diagram for .NET 18.8][3]
*   [Aspose.Diagram for Java 18.8][4]

## Set Locale with Aspose.Diagram for Java

As per general behavior in Java Applications when an unrecognized locale is encountered, they fall to the parts of locale settings which is recognized. In the earlier version(s) of the API, API was unable to demonstrate such behavior in Java Applications. Setting different locales support has been added in the latest release of the API and you can set locale as per your requirements using following code snippet:

```
LoadOptions loadOptions = new LoadOptions(LoadFileFormat.VDX);
loadOptions.setLocale(Locale.US);
Diagram diagram = new Diagram("test.vdx", loadOptions);
```

## Support to Create New Reviewer

While creating comments in a Diagram, sometime you have a requirement to specify reviewer for comments. In order to specify different reviewers for different comments, new support has been added in Aspose.Diagram API. You can use following code snippet to implement this new feature:

```
Reviewer viewer = new Reviewer();
viewer.Name.Value ="test";
viewer.ReviwerID.Value = 3;
```

## Miscellaneous Fixes

Along with the features and enhancements mentioned above, following are various fixes which have been made in latest version of the API:

*   Improved Image Rendering
*   VSD to other file formats conversion has been further improved
*   Diagram saving has been improved to work effeciently
*   Improved Shapes Processing in a VDX file

## Aspose.Diagram for .NET and Java Resources

The following resources will help you work with Aspose.Diagram for .NET and Java APIs:

*   [Home page for Aspose.Diagram API][5].
*   [Aspose.Diagram API wiki docs][6]– Help documentation and API reference documents.
*   [Aspose.Diagram product family forum][7]– Post your technical questions, queries and any other problem you faced while running Aspose.Diagram APIs.
*   [Enable email subscription][8]– Do not limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
*   [Aspose.Diagram for .NET Examples][9]– We have published our code examples on the social coding website GitHub.com. Anyone can explore the code examples for learning purposes.
*   [Aspose.Diagram for Java Examples][10] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
*   Release Notes ([.NET][11] and [Java][12] – For details on API fixes, please check Release Notes having a complete list of the new features.




[1]: https://docs.aspose.com/display/diagramnet/Aspose.Diagram+for+.NET+18.8+Release+Notes
[2]: https://docs.aspose.com/display/diagramjava/Aspose.Diagram+for+Java+18.8+Release+Notes
[3]: https://www.nuget.org/packages/Aspose.Diagram/18.8.0
[4]: https://artifact.aspose.com/repo/com/aspose/aspose-diagram/18.8/
[5]: http://www.aspose.com/products/diagram
[6]: https://docs.aspose.com/display/diagramproductfamily/Home
[7]: https://forum.aspose.com/c/diagram
[8]: https://blog.aspose.com/category/aspose-products/aspose-diagram-product-family/
[9]: https://github.com/asposediagram/Aspose_diagram_NET
[10]: https://github.com/asposediagram/Aspose_Diagram_Java
[11]: https://docs.aspose.com/display/diagramnet/Aspose.Diagram+for+.NET+18.8+Release+Notes
[12]: https://docs.aspose.com/display/diagramjava/Aspose.Diagram+for+Java+18.8+Release+Notes)




