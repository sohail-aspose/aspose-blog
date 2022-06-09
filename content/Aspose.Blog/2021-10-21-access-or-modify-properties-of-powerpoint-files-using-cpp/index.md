---
title: 'Access or Modify Properties of PowerPoint Files using C++'
seoTitle: "Access or Modify Properties of PowerPoint Files using C++"
description: "Use the C++ PowerPoint API to add, access and modify built-in and custom document properties in PowerPoint presentations using C++."
date: Thu, 21 Oct 2021 15:31:20 +0000
draft: false
url: /2021/10/21/access-or-modify-properties-of-powerpoint-files-using-cpp/
author: Muhammad Ahmad
summary: 'PowerPoint files contain metadata or document properties that provide additional information about the presentation. These include information such as the title, date, author, etc., of the presentation. In this article, you will learn **how to access and modify the properties in PowerPoint presentations using C++**.'
tags: ['Access Built-in Properties in PowerPoint C++', 'Access Custom Properties in PowerPoint C++', 'Add Custom Properties in PowerPoint C++', 'Modify Built-in Properties in PowerPoint C++', 'Modify Custom Properties in PowerPoint C++']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Document-Properties-in-PowerPoint.jpg" alt="Access or Modify Properties of PowerPoint Files using C++">}}


PowerPoint files contain metadata or document properties that provide additional information about the presentation. These include information such as the title, date, author, etc., of the presentation. In this article, you will learn **how to access and modify the properties in PowerPoint presentations using C++**.

*   [C++ API for Accessing and Modifying Properties of PowerPoint Presentations][1]
*   [Types of Properties in PowerPoint Presentations][2]
*   [Access Built-in Properties in PowerPoint Presentations][3]
*   [Modify Built-in Properties in PowerPoint Presentations][4]
*   [Add Custom Properties in PowerPoint Presentations][5]
*   [Access and Modify Custom Properties in PowerPoint Presentations][6]

## C++ API for Accessing and Modifying Properties of PowerPoint Presentations {#CPP-API-for-Accessing-and-Modifying-Properties-of-PowerPoint-Presentations}

[Aspose.Slides for C++][7] is a C++ API for working with PowerPoint files. It enables you to create, read and update PowerPoint files without needing additional software. Furthermore, the API allows you to access and modify the properties of PowerPoint presentations. You can either install the API through [NuGet][8] or download it directly from the [Downloads][9] section.

```
PM> Install-Package Aspose.Slides.Cpp
```

## Types of Properties in PowerPoint Presentations {#Types-of-Properties-in-PowerPoint-Presentations}

There are two types of properties in PowerPoint presentations: built-in and custom. The built-in properties store general information about the presentations like the title, date, etc. On the other hand, custom properties store custom information in key/value pairs. The following sections cover how to add, access, and modify built-in and custom properties of PowerPoint presentations.

## Access Built-in Properties in PowerPoint Presentations using C++ {#Access-Built-in-Properties-in-PowerPoint-Presentations-using-CPP}

The following are the steps to access built-in properties in PowerPoint presentations.

*   Firstly, load the PowerPoint file using the [Presentation][10] class.
*   Access the properties using the [Presentation->get\_DocumentProperties()][11] method.
*   Read the individual properties using the [IDocumentProperties][12] object with methods like [IDocumentProperties->get\_Category()][13], [IDocumentProperties->get\_Author()][14], etc.

The following sample code shows how to access built-in properties in PowerPoint presentations using C++.

{{< gist aspose-com-gists e41095433eb735742b5dfdf2f202561d "Access_Builtin_Properties.cpp" >}}

## Modify Built-in Properties in PowerPoint Presentations using C++ {#Modify-Built-in-Properties-in-PowerPoint-Presentations-using-CPP}

The following are the steps to modify built-in properties in PowerPoint presentations.

*   Firstly, load the PowerPoint file using the [Presentation][15] class.
*   Retrieve the properties in the [IDocumentProperties][16] object using the [Presentation->get\_DocumentProperties()][17] method.
*   Modify the properties using the [IDocumentProperties][18] object with methods like [IDocumentProperties->set\_Author(System::String value)][19], [IDocumentProperties->set\_Title(System::String value)][20], etc.
*   Finally, save the presentation using the [Presentation->Save(System::String fname, Export::SaveFormat format)][21] method.

The following sample code shows how to modify built-in PowerPoint properties using C++.

{{< gist aspose-com-gists e41095433eb735742b5dfdf2f202561d "Modify_Builtin_Properties.cpp" >}}

## Add Custom Properties in PowerPoint Presentations using C++ {#Add-Custom-Properties-in-PowerPoint-Presentations-using-CPP}

The following are the steps to add custom properties in PowerPoint presentations.

*   Firstly, load the PowerPoint file using the [Presentation][22] class.
*   Retrieve the properties in the [IDocumentProperties][23] object using the [Presentation->get\_DocumentProperties()][24] method.
*   Add the custom properties using the [IDocumentProperties->idx\_set(System::String name, System::SharedPtr<System::Object> value)][25] method.
*   Finally, save the presentation using the [Presentation->Save(System::String fname, Export::SaveFormat format)][26] method.

The following sample code shows how to add custom properties in PowerPoint presentations.

{{< gist aspose-com-gists e41095433eb735742b5dfdf2f202561d "Add_Custom_Properties.cpp" >}}

## Access and Modify Custom Properties in PowerPoint Presentations {#Access-and-Modify-Custom-Properties-in-PowerPoint-Presentations}

The following are the steps to access and modify custom properties in PowerPoint presentations.

*   Firstly, load the PowerPoint file using the [Presentation][27] class.
*   Retrieve the properties in the [IDocumentProperties][28] object using the [Presentation->get\_DocumentProperties()][29] method.
*   Loop through the properties and access each property's name and value using the [IDocumentProperties->GetCustomPropertyName(int32\_t index)][30] and [IDocumentProperties->idx\_get(System::String name)][31] methods respectively.
*   Modify the required custom properties using the [IDocumentProperties->SetCustomPropertyValue()][32] method based on the type of the value you want to store.
*   Finally, save the presentation using the [Presentation->Save(System::String fname, Export::SaveFormat format)][33] method.

The following sample code shows how to access and modify custom properties in PowerPoint presentations using C++.

{{< gist aspose-com-gists e41095433eb735742b5dfdf2f202561d "Access_And_Modify_Custom_Properties.cpp" >}}

## Get a Free License

In order to try the API without evaluation limitations, you can request [a free temporary license][34].

## Conclusion

In this article, you have learned how to access and modify built-in properties in PowerPoint presentations. Furthermore, you have seen how to add, access, and modify custom PowerPoint properties using Aspose.Slides for C++ API. It is a robust API with lots of additional features for automating your PowerPoint-related tasks. You can explore the API in detail by visiting the [official documentation][35]. In case of any queries, please feel free to reach us at our [free support forum][36].

## See Also

*   [Embed Video in PowerPoint Presentations using C++][37]
*   [Add Slide Transitions in PowerPoint Presentations using C++][38]




[1]: #CPP-API-for-Accessing-and-Modifying-Properties-of-PowerPoint-Presentations
[2]: #Types-of-Properties-in-PowerPoint-Presentations
[3]: #Access-Built-in-Properties-in-PowerPoint-Presentations-using-CPP
[4]: #Modify-Built-in-Properties-in-PowerPoint-Presentations-using-CPP
[5]: #Add-Custom-Properties-in-PowerPoint-Presentations-using-CPP
[6]: #Access-and-Modify-Custom-Properties-in-PowerPoint-Presentations
[7]: https://products.aspose.com/slides/cpp
[8]: https://www.nuget.org/packages/Aspose.Slides.Cpp
[9]: https://downloads.aspose.com/slides/cpp
[10]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[11]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#a40a03eb17a9904ff80063f6df714c402
[12]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_document_properties
[13]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_document_properties#acea84e0d96a3fa4dd5c18e4c39baf63f
[14]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_document_properties#a9060ad8ff6fdf44a6bf7c2f86a1551bd
[15]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[16]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_document_properties
[17]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#a40a03eb17a9904ff80063f6df714c402
[18]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_document_properties
[19]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_document_properties#a5196195772184dfab679defe42e30d74
[20]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_document_properties#aaa50a12098b437503992a76916d0c7c5
[21]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[22]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[23]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_document_properties
[24]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#a40a03eb17a9904ff80063f6df714c402
[25]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_document_properties#ab4a1ea577aed49917841e170b29fe971
[26]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[27]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[28]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_document_properties
[29]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#a40a03eb17a9904ff80063f6df714c402
[30]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_document_properties#a71d28c68406a23b9542a93626d579456
[31]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_document_properties#a56c14fe8ac59a9e8678b9f61dd16cfc5
[32]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_document_properties#a7e0d0bb0c76e18da43f5e171c304649a
[33]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[34]: https://purchase.aspose.com/temporary-license
[35]: https://docs.aspose.com/slides/cpp/
[36]: https://forum.aspose.com/c/slides/11
[37]: https://blog.aspose.com/2021/10/15/embed-video-in-powerpoint-presentations-using-cpp/
[38]: https://blog.aspose.com/2021/10/14/add-slide-transitions-in-powerpoint-presentations-using-cpp/




