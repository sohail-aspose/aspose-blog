---
title: 'Convert 3D Model to PDF and Import 3D Content from PDF using C#'
date: Thu, 06 Oct 2016 05:08:00 +0000
draft: false
url: /2016/10/06/save-a-3d-model-in-pdf-generate-tangent-and-binormal-data-for-all-meshes-and-import-3d-content-from-pdf-using-aspose.3d-for-.net-16.9.0/
author: Imran Rafique
summary: ''
tags: ['Convert Polygons to Triangles', 'Import 3D Contents', 'Import 3D Scenes', 'Save 3D Model in PDF', 'Tangent and Binormal Data']
categories: ['Aspose.3D Product Family']
---



{{< figure align=center src="images/Aspose.3d-for-net-100x100.png" alt="Aspose.3D for NET APIs">}}


We are pleased to announce the availability of [new version 16.9.0 of Aspose.3D for .NET API][1]. The new version extends this API with new key features. Developers can import any supported type of 3D model, and then export it to PDF. They can also import 3D scenes and contents from an existing 3D PDF as well as convert all polygons to triangles of a 3D model, and may also generate tangent and binormal data for all meshes in 3D models. The list of supported 3D formats is constantly growing as demands change and technologies evolve. Developers can install Aspose.3D Nuget package in their .NET applications because we publish each version as [a NuGet package on the NuGet gallery][2]. We recommend our clients upgrade old version of the Aspose.3D API to this latest one. For details on API fixes, please check Release Notes having a complete list of the features, enhancements and bug fixes.

## Convert 3D Models to PDF using C#

Using Aspose.3D API, developers may create a 3D model from scratch or import from an existing 3D file, they can save it to the PDF. It was a demanded feature because PDF files are compatible across multiple platforms. This article shows how developers can save a 3D scene in the PDF file format: Save a 3D Scene in the PDF Format

{{< gist aspose-3d 631532eeb21c3374f2ed "Examples-CSharp-Loading-and-Saving-Save3DInPdf-Save3DInPdf.cs" >}}

## Import 3D Scenes and Contents from a PDF

A PDF can store 3D scenes and contents to display 3D models interactively. Aspose.3D API allows to extract 3D scenes and contents from 3D PDFs. Developers may iterate through all 3D scenes and contents to save them in separate files. This article shows how developers can extract 3D scenes and contents from a PDF, and then save in the separate files: Import 3D Scenes and Contents from a PDF

{{< gist aspose-3d 631532eeb21c3374f2ed "Examples-CSharp-Loading-and-Saving-OpenSceneFromProtectedPdf-OpenSceneFromProtectedPdf.cs" >}}

### Extract All Raw 3D Content from PDF

{{< gist aspose-3d 631532eeb21c3374f2ed "Examples-CSharp-Loading-and-Saving-OpenSceneFromProtectedPdf-OpenSceneFromProtectedPdf.cs" >}}

### Extract All 3D Scenes From PDF into 3D Format

{{< gist aspose-3d 631532eeb21c3374f2ed "Examples-CSharp-Loading-and-Saving-OpenSceneFromProtectedPdf-OpenSceneFromProtectedPdf.cs" >}}

## Convert All Polygons to Triangles in a 3D Scene

Using Aspose.3D API, developers can now convert all polygons to triangles of a 3D scene. This way, they can ensure proper rendering of the non-planar faces. This article shows how developers can convert all polygons to triangles in 3D file: Convert All Polygons to Triangles in 3D Files

## Generate Tangent and Binormal Data for All Meshes

All meshes don't contain tangent and binormal (bitangent) data in various 3D file types. Using Aspose.3D API, developers can generate and store tangent and binormal data for all meshes. The tangent and bitangent are orthogonal vectors with the Normal and instruct about the rate of change of the texture coordinates over the mesh surface. This article shows how to generate tangent and binormal data for all meshes of a 3D scene: Build Tangent and Binormal Data for All Meshes in 3D Files

## Public API Changes

The following API changes in the new version are also worth noting:

*   PdfLoadOptions, PdfSaveOptions and PdfFormat classes have been added.
*   A PDF format entry has been added in the FileFormat class for loading and saving purposes.
*   PdfLightingScheme and PdfRenderMode enums are added to set a rendering mode and lighting scheme before saving a 3D scene in the PDF.
*   A Triangulate method is added in the PolygonModifier class to convert all polygons to triangles in a 3D scene.
*   The two BuildTangentBinormal methods are added in the PolygonModifier class to generate tangent and binormal data for all meshes.

## Aspose.3D for .NET Resources

The following resources will help you work with Aspose.3D for .NET:

*   [Home page for Aspose.3D for .NET API][3]
*   [Download Aspose.3D for .NET][4]
*   [Aspose.3D product family forum][5] - Post your technical questions, queries and any other problem you faced while running Aspose.3D APIs.
*   Aspose.3D for .NET online documentation – help documentation and API reference documents.
*   [Enable Blog Subscription][6] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.3D APIs, new features, fixes and other API related topics by subscribing to Aspose.3D blog.
*   [Aspose.3D for .NET Examples][7] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
*   Migrate from Earlier Versions of Aspose.3D API – We keep track of Aspose.3D API change version by version. So we recommend to get help from this section while upgrading to the latest API version or if Aspose.3D API code is broken at some stage.

We hope you’ll enjoy this new release that save time and efforts. The API is quite simple and developers can use it in application easily.




[1]: http://downloads.aspose.com/3d/net/new-releases/aspose.3d-for-.net-16.9.0/
[2]: https://www.nuget.org/packages/Aspose.3d
[3]: http://www.aspose.com/products/3d/net
[4]: http://downloads.aspose.com/3d/net
[5]: http://www.aspose.com/community/forums/aspose.3d-product-family/535/showforum.aspx
[6]: https://blog.aspose.com/category/aspose-products/aspose-3d-product-family
[7]: https://github.com/aspose3D/Aspose_3d_NET




