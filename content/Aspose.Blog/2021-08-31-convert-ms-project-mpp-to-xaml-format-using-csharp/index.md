---
title: 'Convert MS Project MPP to XAML Format using C#'
seoTitle: "Convert MS Project MPP to XAML Format using C#"
description: "Convert MPP files XAML format using C#. Customize the generated XAML output using additional options. Set the presentation format for the generated XAML."
date: Tue, 31 Aug 2021 17:30:51 +0000
draft: false
url: /2021/08/31/convert-ms-project-mpp-to-xaml-format-using-csharp/
author: Muhammad Ahmad
summary: 'Extensible Application Markup Language ([XAML][1] is a simple and declarative language based on [XML][2] that uses the .xaml format for its files. In XAML, you can create, initialize, and set properties of objects with hierarchical relations. It is mainly used to design graphical user interfaces in Xamarin Forms, UWP (Universal Windows Platform), and WPF (Windows Presentation Foundation). In this article, you will learn **how to convert Microsoft Project MPP files to XAML format using C#**.'
tags: ['Convert MPP to XAML C#', 'Convert MPP to XAML with Additional Options C#', 'Set Presentation Format while Convert MPP to XAML C#']
categories: ['Aspose.Tasks Product Family']
---



{{< figure align=center src="images/MPP-to-XAML.jpg" alt="Convert MS Project MPP to XAML Format using C#">}}


Extensible Application Markup Language ([XAML][3] is a simple and declarative language based on [XML][4] that uses the .xaml format for its files. In XAML, you can create, initialize, and set properties of objects with hierarchical relations. It is mainly used to design graphical user interfaces in Xamarin Forms, UWP (Universal Windows Platform), and WPF (Windows Presentation Foundation). In this article, you will learn **how to convert Microsoft Project MPP files to XAML format using C#**.

*   [C# API for Converting MPP Files to XAML Format][5]
*   [Convert MPP Files to XAML Format using C#][6]
*   [Convert MPP Files to XAML Format with Additional Options][7]
*   [Set Presentation Format while Converting MPP Files to XAML Format][8]

## C# API for Converting MPP Files to XAML Format {#CSharp-API-for-Converting-MPP-Files-to-XAML-Format}

[Aspose.Tasks for .NET][9] is an API for working with Microsoft Project (MPP) files. It allows you to read and write MPP/XML files without requiring Microsoft Project to be installed. Furthermore, the API enables you to convert MPP files to XAML format. You can either install the API through [NuGet][10] or download it directly from the [Downloads][11] section.

```
PM> Install-Package Aspose.Tasks
```

## Convert MPP Files to XAML Format using C# {#Convert-MPP-Files-to-XAML-Format-using-CSharp}

You can convert MPP files to XAML format in just a few lines of code. To achieve that, please follow the steps given below.

*   Load the MPP file using the [Project][12] class.
*   Save the XAML file using the [Project.Save(string filename,SaveFileFormat format)][13] method.

The following sample code shows how to convert MPP files to XAML format using C#.

{{< gist aspose-com-gists 6268d176bd53cc58f9e210d92e250476 "Convert_MPP_To_XAML.cs" >}}

## Convert MPP Files to XAML Format with Additional Options {#Convert-MPP-Files-to-XAML-Format-with-Additional-Options}

In order to customize the generated XAML file, you can use the [XamlOptions][14] class. To use the [XamlOptions][15], follow the steps given below.

*   Load the MPP file using the [Project][16] class.
*   Create an instance of the [XamlOptions][17] class.
*   Set the desired options.
*   Save the XAML file using the [Project.Save(string filename, SaveOptions options)][18] method.

The following sample code shows how to convert an MPP file to XAML format using additional options with C#.

{{< gist aspose-com-gists 6268d176bd53cc58f9e210d92e250476 "Convert_MPP_To_XAML_With_Options.cs" >}}

## Set Presentation Format while Converting MPP Files to XAML Format {#Set-Presentation-Format-while-Converting-MPP-Files-to-XAML-Format}

While converting MPP files to XAML format, you can use different presentation formats. To specify the presentation format, you will use the [PresentationFormat][19] enumeration. The [PresentationFormat][20] enumeration provides the following options.

*   PresentationFormat.GanttChart
*   PresentationFormat.TaskUsage
*   PresentationFormat.ResourceUsage
*   PresentationFormat.ResourceSheet
*   PresentationFormat.TaskSheet

The following are the steps to set the presentation format while converting MPP files to XAML format.

*   Load the MPP file using the [Project][21] class.
*   Create an instance of the [XamlOptions][22] class.
*   Set the presentation format by setting the [XamlOptions.PresentationFormat][23] property value using the [PresentationFormat][24] enumeration.
*   Save the XAML file using the [Project.Save(string filename, SaveOptions options)][25] method.

The following sample code shows how to set the presentation format while converting MPP files to XAML format using C#.

{{< gist aspose-com-gists 6268d176bd53cc58f9e210d92e250476 "Set_Presentation_Format_While_Converting_MPP_To_XAML.cs" >}}

## Get a Free License

In order to try the API without evaluation limitations, you can request [a free temporary license][26].

## Conclusion

In this article, you have learned how to convert MPP files to XAML format using C#. You have also learned how to customize the generated XAML output using additional options. Furthermore, you have seen how to set the presentation format for the generated XAML files using Aspose.Tasks for .NET API. The API provides many additional features for working with MPP files that you can explore in detail by visiting the [official documentation][27]. In case of any questions, please feel free to reach us at our [free support forum][28].

## See Also

*   [Convert XML to MPP or MPP to XML Programmatically using C#][29]
*   [Convert MS Project MPP to Images (PNG, JPEG, BMP, TIFF) using C#][30]




[1]: https://docs.fileformat.com/web/xaml/)
[2]: https://docs.fileformat.com/web/xml/
[3]: https://docs.fileformat.com/web/xaml/)
[4]: https://docs.fileformat.com/web/xml/
[5]: #CSharp-API-for-Converting-MPP-Files-to-XAML-Format
[6]: #Convert-MPP-Files-to-XAML-Format-using-CSharp
[7]: #Convert-MPP-Files-to-XAML-Format-with-Additional-Options
[8]: #Set-Presentation-Format-while-Converting-MPP-Files-to-XAML-Format
[9]: https://products.aspose.com/tasks/net/
[10]: https://www.nuget.org/packages/Aspose.Tasks
[11]: https://downloads.aspose.com/tasks/net
[12]: https://apireference.aspose.com/tasks/net/aspose.tasks/project
[13]: https://apireference.aspose.com/tasks/net/aspose.tasks.project/save/methods/5
[14]: https://apireference.aspose.com/tasks/net/aspose.tasks.saving/xamloptions
[15]: https://apireference.aspose.com/tasks/net/aspose.tasks.saving/xamloptions
[16]: https://apireference.aspose.com/tasks/net/aspose.tasks/project
[17]: https://apireference.aspose.com/tasks/net/aspose.tasks.saving/xamloptions
[18]: https://apireference.aspose.com/tasks/net/aspose.tasks.project/save/methods/6
[19]: https://apireference.aspose.com/tasks/net/aspose.tasks.visualization/presentationformat
[20]: https://apireference.aspose.com/tasks/net/aspose.tasks.visualization/presentationformat
[21]: https://apireference.aspose.com/tasks/net/aspose.tasks/project
[22]: https://apireference.aspose.com/tasks/net/aspose.tasks.saving/xamloptions
[23]: https://apireference.aspose.com/tasks/net/aspose.tasks.saving/saveoptions/properties/presentationformat
[24]: https://apireference.aspose.com/tasks/net/aspose.tasks.visualization/presentationformat
[25]: https://apireference.aspose.com/tasks/net/aspose.tasks.project/save/methods/6
[26]: https://purchase.aspose.com/temporary-license
[27]: https://docs.aspose.com/tasks/net/
[28]: https://forum.aspose.com/c/tasks/15
[29]: https://blog.aspose.com/2021/08/25/convert-xml-to-mpp-or-mpp-to-xml-programmatically-using-csharp/
[30]: https://blog.aspose.com/2021/08/12/convert-ms-project-mpp-to-images-png-jpeg-bmp-tiff-using-csharp/





