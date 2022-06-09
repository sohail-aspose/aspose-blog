---
title: 'Working with Shapes in PowerPoint presentations using C++'
seoTitle: "Working with Shapes in PowerPoint presentations using C++"
description: "Working with shapes in PowerPoint slides using C++. Add shapes like rectangles, ellipses, lines, etc and connect them using connectors."
date: Tue, 20 Apr 2021 09:33:23 +0000
draft: false
url: /2021/04/20/working-with-shapes-in-powerpoint-presentations-using-cpp/
author: Muhammad Ahmad
summary: 'Microsoft PowerPoint provides you the ability to add shapes to your presentations. Shapes can be helpful in scenarios such as showing the flow of data or showing different phases of a process. You can use shapes such as ellipses, lines, rectangles, etc., and connect them using connectors. You might find yourself in scenarios where you have to add shapes to PowerPoint slides programmatically. To that end, this article will teach you how to **work with shapes in PowerPoint presentations using C++**.'
tags: ['Add Shapes to PowerPoint Slides C++', 'Clone Shapes in PowerPoint Slides C++', 'Connect Shapes in PowerPoint Slides C++', 'Remove Shapes from PowerPoint Slides C++']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Work-with-Shapes-in-Slides-in-C-1024x578.jpg" alt="Working with Shapes in PowerPoint presentations using C++">}}


Microsoft PowerPoint provides you the ability to add shapes to your presentations. Shapes can be helpful in scenarios such as showing the flow of data or showing different phases of a process. You can use shapes such as ellipses, lines, rectangles, etc., and connect them using connectors. You might find yourself in scenarios where you have to add shapes to PowerPoint slides programmatically. To that end, this article will teach you **how to work with shapes in PowerPoint presentations using C++**.

*   [C++ API for Working with Shapes in PowerPoint Presentations][1]
*   [Add a Shape to a PowerPoint Slide][2]
*   [Add Connected Shapes to a PowerPoint Slide][3]
*   [Clone Shapes in PowerPoint Slides][4]
*   [Remove Shapes from PowerPoint Slides using C++][5]
*   [Supported PowerPoint Shapes][6]
*   [Get a Free License][7]

## C++ API for Working with Shapes in PowerPoint Presentations {#CPP-API-for-Working-with-Shapes-in-PowerPoint-Presentations}

[Aspose.Slides for C++][8] is a native C++ library that supports creating, reading, and manipulating PowerPoint files. The API also supports working with shapes in PowerPoint presentations. You can either install the API through [NuGet][9] or download it directly from the [Downloads][10] section.

```
PM> Install-Package Aspose.Slides.Cpp
```

## Add a Shape to a PowerPoint Slide {#Add-a-Shape-to-a-PowerPoint-Slide}

In order to add a shape, use the [ISlide->get\_Shapes()->AddAutoShape()][11] method provided by the API. The following are the steps to add a shape to a PowerPoint slide.

*   Firstly, load the PowerPoint presentation using the [Presentation][12] class.
*   Retrieve the slide where you want to add the shape using the [Presentation->get\_Slides()->idx\_get (int32\_t index)][13] method.
*   Add the shape using the [ISlide->get\_Shapes()->AddAutoShape (ShapeType shapeType, float x, float y, float width, float height)][14] method.
*   Finally, save the presentation using the [Presentation->Save (System::String name, Export::SaveFormat format)][15] method.

The following is the sample code to add a shape to a PowerPoint slide using C++.

{{< gist aspose-com-gists fc1c4560980079d14345c92c5765f0ab "Add-Shape.cpp" >}}



{{< figure align=center src="images/AddShapePowerPointCpp-1024x438.png" alt="Add Shape to PowerPoint Slide">}}


## Add Connected Shapes to a PowerPoint Slide {#Add-Connected-Shapes-to-a-PowerPoint-Slide}

Connectors can be used to connect shapes. In order to create a connector, you can use the [ISlide->get\_Shapes()->AddConnector()][16] method. The following are the steps to add connected shapes to a PowerPoint slide.

*   Firstly, load the PowerPoint presentation using the [Presentation][17] class.
*   Retrieve the slide where you want to add the shapes using the [Presentation->get\_Slides()->idx\_get (int32\_t index)][18] method.
*   Add the shapes using the [ISlide->get\_Shapes()->AddAutoShape (ShapeType shapeType, float x, float y, float width, float height)][19] method.
*   Add the connector using the [ISlide->get\_Shapes()->AddConnector (ShapeType shapeType, float x, float y, float width, float height)][20] method.
*   Connect the shapes to the connector using the [IConnector->set\_StartShapeConnectedTo (System::SharedPtr<IShape> value)][21] and [IConnector->set\_EndShapeConnectedTo (System::SharedPtr<IShape> value)][22] methods.
*   Call the [IConnector->Reroute()][23] method to create the shortest automatic connection path.
*   Finally, save the presentation using the [Presentation->Save (System::String name, Export::SaveFormat format)][24] method.

The following is the sample code to add connected shapes to a PowerPoint slide using C++.

{{< gist aspose-com-gists fc1c4560980079d14345c92c5765f0ab "Add-Connected-Shapes.cpp" >}}



{{< figure align=center src="images/AddConnectedShapesPowerPointCpp-1024x431.png" alt="Add Connected Shapes to PowerPoint Slide">}}


## Clone Shapes in PowerPoint Slides {#Clone-Shapes-in-PowerPoint-Slides}

You can also clone existing shapes using the Aspose.Slides for C++ API. In order to clone a shape, use the [ShapeCollection->InsertClone()][25] method provided by the API. The following are the steps to clone shapes from one slide to another.

*   Firstly, load the PowerPoint presentation using the [Presentation][26] class.
*   Retrieve the source slide using the [Presentation->get\_Slides()->idx\_get (int32\_t index)][27] method.
*   Access the shapes of the source slide using the [ISlide->get\_Shapes()][28] method.
*   Access the shapes of the destination slide using the [ISlide->get\_Shapes()][29] method.
*   Clone the shape using the [IShapeCollection->InsertClone (int32\_t index, System::SharedPtr<IShape> sourceShape, float x, float y)][30] method.
*   Finally, save the presentation using the [Presentation->Save (System::String name, Export::SaveFormat format)][31] method.

The following is the sample code to clone shapes in PowerPoint slides using C++.

{{< gist aspose-com-gists fc1c4560980079d14345c92c5765f0ab "Clone-Shape.cpp" >}}



{{< figure align=center src="images/CloneShapePowerPointCpp-1024x438.png" alt="Clone Shapes in PowerPoint Slides">}}


## Remove Shapes from PowerPoint Slides using C++ {#Remove-Shapes-from-PowerPoint-Slides-using-CPP}

The following are the steps to remove shapes from PowerPoint slides.

*   Firstly, load the PowerPoint presentation using the [Presentation][32] class.
*   Retrieve the slide from where you want to remove the shape using the [Presentation->get\_Slides()->idx\_get (int32\_t index)][33] method.
*   Find the required shape by matching the alternative text using the [IShape->get\_AlternativeText()][34] method.
*   Remove the shape using the [ISlide->get\_Shapes()->Remove (System::SharedPtr<IShape> shape)][35] method.
*   Finally, save the presentation using the [Presentation->Save (System::String name, Export::SaveFormat format)][36] method.

The following is the sample code to remove shapes from PowerPoint slides using C++.

{{< gist aspose-com-gists fc1c4560980079d14345c92c5765f0ab "Remove-Shape.cpp" >}}

## Supported PowerPoint Shapes {#Supported-PowerPoint-Shapes}

Aspose.Slides for C++ supports many shapes for you to work with. The following is a list of some of the supported shapes.

*   [Ellipse][37]
*   [Line][38]
*   [Rectangle][39]
*   [Connector][40]

You can view the complete list of supported shapes by viewing the [ShapeType][41] enum values.

## Get a Free License {#Get-a-Free-License}

You can request [a free temporary license][42] to try the API without evaluation limitations.

## Conclusion

In this article, you have learned how to work with shapes in PowerPoint presentations using C++. Specifically, you have learned how to add, clone, and remove shapes from PowerPoint slides. Furthermore, you have seen how to connect shapes using a connector. In addition to working with shapes, Aspose.Slides for C++ provides many additional features for enhancing your PowerPoint presentations. You can explore the API in detail by visiting the [official documentation][43]. In case of any questions, please feel free to reach us on our [free support forum][44].

## See Also

*   [Extract Text from PowerPoint Files using C++][45]




[1]: #CPP-API-for-Working-with-Shapes-in-PowerPoint-Presentations
[2]: #Add-a-Shape-to-a-PowerPoint-Slide
[3]: #Add-Connected-Shapes-to-a-PowerPoint-Slide
[4]: #Clone-Shapes-in-PowerPoint-Slides
[5]: #Remove-Shapes-from-PowerPoint-Slides-using-CPP
[6]: #Supported-PowerPoint-Shapes
[7]: #Get-a-Free-License
[8]: https://products.aspose.com/slides/cpp
[9]: https://www.nuget.org/packages/Aspose.Slides.Cpp
[10]: https://downloads.aspose.com/slides/cpp
[11]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_shape_collection#a22cd6252336905ea935496b4b5799ae2
[12]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[13]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_slide_collection#a640042758d7f73745c4e6a0eceb5524e
[14]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_shape_collection#a22cd6252336905ea935496b4b5799ae2
[15]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[16]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_shape_collection#a9441bdd5610d5277e7e57d3ff0bc6d94
[17]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[18]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_slide_collection#a640042758d7f73745c4e6a0eceb5524e
[19]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_shape_collection#a22cd6252336905ea935496b4b5799ae2
[20]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_shape_collection#a9441bdd5610d5277e7e57d3ff0bc6d94
[21]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_connector#a09179f3f5f66bf9e594c4f4065c8196a
[22]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_connector#a0d26c504c8557f626a49e1c9474b8e5d
[23]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_connector#a450b0d683a7bce41cc17bef08f95f492
[24]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[25]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_shape_collection#ae5a4f29ccd34398ad86e587917234860
[26]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[27]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_slide_collection#a640042758d7f73745c4e6a0eceb5524e
[28]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_base_slide#aa6b93a3863b7516d4a1a751a0ca885c7
[29]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_base_slide#aa6b93a3863b7516d4a1a751a0ca885c7
[30]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_shape_collection#ae5a4f29ccd34398ad86e587917234860
[31]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[32]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[33]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_slide_collection#a640042758d7f73745c4e6a0eceb5524e
[34]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_shape#a4d2254f43168cd342909f38a93df8b95
[35]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_shape_collection#a0fbbe99a14c1b2d7634f1e7881360f0c
[36]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[37]: https://docs.aspose.com/slides/cpp/ellipse/
[38]: https://docs.aspose.com/slides/cpp/line/
[39]: https://docs.aspose.com/slides/cpp/rectangle/
[40]: https://docs.aspose.com/slides/cpp/connector/
[41]: https://apireference.aspose.com/slides/cpp/namespace/aspose.slides#abe1c0baea327186bde49ad44636bb8c5
[42]: https://purchase.aspose.com/temporary-license
[43]: https://docs.aspose.com/slides/cpp/
[44]: https://forum.aspose.com/c/slides/11
[45]: https://blog.aspose.com/2021/04/10/extract-text-from-powerpoint-files-using-cpp/





