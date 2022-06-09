---
title: 'Convert MS Visio Diagrams to PDF, PNG, JPEG, SVG, HTML and XAML in Node.js'
seoTitle: ""
description: ""
date: Wed, 13 May 2020 18:29:48 +0000
draft: false
url: /2020/05/13/convert-ms-visio-vsd-vsdx-to-pdf-png-jpeg-svg-html-xaml-in-node-js/
author: Usman Aziz
summary: ''
tags: ['Node.js Visio Converter API', 'Visio to HTML', 'Visio to JPEG', 'Visio to PDF', 'Visio to PNG', 'Visio to SVG', 'Visio to XML']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/Convert-Visio-to-PDF-PNG-JPEG-SVG-HTML-XAML-in-NodeJs.jpg" alt="Convert Visio to PDF PNG JPEG SVG HTML XAML in Node.Js">}}


In my previous [post][1], I have demonstrated how to create MS Visio diagrams from scratch in Node.js applications. In this article, I'll show you how to use [Aspose.Diagram][2] to export or convert MS Visio diagrams to various popular file formats in Node.js applications.

The conversion of Visio diagrams could be useful in various scenarios. You can convert a diagram to HTML or JPEG/PNG image to display it on a web page or in a Visio document viewer. Similarly, Visio to PDF conversion could be used to remove the dependency of dedicated software for viewing the diagrams. For such scenarios, Aspose.Diagram provides high-quality conversion of Visio diagrams to other formats.

*   [Convert Visio to PDF in Node.js][3]
*   [Convert Visio Diagram to PNG/JPEG/Other Image Formats][4]
*   [Export Visio Diagrams to SVG in Node.js][5]
*   [Convert Visio Diagram to HTML in Node.js][6]
*   [Visio to XAML Conversion in Node.js][7]

## Node.js Visio Converter API - Installation

You can install Aspose.Diagram into your Node.js application using the following npm command.

```
npm install aspose.diagram --save
```

## Convert Visio to PDF in Node.js {#Convert-Visio-to-PDF-in-Node.js}

PDF is a platform-independent document format that keeps the content of a document stable among the heterogeneous environments. Therefore, it is more suitable to convert a Visio diagram to PDF before sharing it among the people without worrying about their environment or installing dedicated software. The following are the steps to convert a Visio diagram to PDF document using Aspose.Diagram.

*   Load the VSD/VSDX Visio diagram using the [Diagram][8] class.
*   Export the diagram to PDF using [Diagram.save(string, SaveFileFormat)][9] method.

The following code sample shows how to convert a Visio VSDX to PDF in Node.js.

{{< gist aspose-com-gists 7ec04b775b208175a41a3c108a6587d1 "convert-visio-vsdx-to-pdf.js" >}}

### VSDX File



{{< figure align=center src="images/Visio-Diagram-JPEG.jpg" alt="VSDX to PDF">}}


### PDF File



{{< figure align=center src="images/Visio-to-PDF.jpg" alt="Visio to PDF in Node.js">}}


## Convert Visio to PNG/JPEG/Other Images in Node.js {#Convert-Visio-Diagram-to-PNG-JPEG-BMP-TIFF}

Conversion of Visio diagrams to image formats is useful for generating thumbnails or displaying the content of the diagrams, i.e. for a Visio viewer. Aspose.Diagram lets you convert Visio diagrams to the following image formats:

*   PNG
*   JPEG
*   TIFF
*   BMP
*   EMF

The following are the steps to convert Visio diagrams to PNG, JPEG or other image formats.

*   Load the MS Visio diagram using [Diagram][10] class.
*   Create an instance of [ImageSaveOptions][11] class and set the desired image format using [SaveFileFormat][12] enumeration.
*   Save the Visio diagram as image using [Diagram.save(string, ImageSaveOptions)][13] method.

The following code sample shows how to convert Visio VSDX to PNG image in Node.js.

{{< gist aspose-com-gists 7ec04b775b208175a41a3c108a6587d1 "convert-visio-vsdx-to-png.js" >}}

## Export Visio Diagrams to SVG in Node.js {#Export-Visio-Diagrams-to-SVG-in-Node.js}

You can also convert a Visio diagram to SVG format in a couple of lines of code. The following are steps to perform this conversion.

*   Load the Visio diagram using [Diagram][14] class.
*   Export the diagram to SVG format using [Diagram.save(string, SaveFileFormat)][15] method.

The following code sample shows how to convert Visio VSDX to SVG format in Node.js.

{{< gist aspose-com-gists 7ec04b775b208175a41a3c108a6587d1 "convert-visio-vsdx-to-svg.js" >}}

## Convert Visio Diagram to HTML in Node.js {#Convert-Visio-Diagram-to-HTML-in-Node.js}

Aspose.Diagram also allows you to convert the Visio diagram into an HTML document. In Visio to HTML conversion, the API also generates a sidebar to navigate between the pages of the diagram. The following are the steps to perform this conversion.

*   Create an instance of the [Diagram][16] class and initialize it with the Visio file's path.
*   Save the diagram as HTML using [Diagram.save(string, SaveFileFormat)][17] method.

The following code sample shows how to convert Visio VSDX to HTML in Node.js.

{{< gist aspose-com-gists 7ec04b775b208175a41a3c108a6587d1 "convert-visio-vsdx-to-html.js" >}}

### Visio to HTML



{{< figure align=center src="images/Visio-to-HTML.jpg" alt="Visio to HTML Node.js">}}


## Convert Visio to XAML in Node.js {#Visio-to-XAML-Conversion-in-Node.js}

You can also convert a Visio diagram to XAML format created using Microsoft's markup language which is named the same, XAML (Extensible Application Markup Language). The following are the steps to convert a Visio diagram to XAML format.

*   Load Visio VSDX file using the [Diagram][18] class.
*   Save VSDX as XAML using [Diagram.save(string, SaveFileFormat)][19] method.

The following code sample shows how to convert Visio VSDX to XAML in Node.js.

{{< gist aspose-com-gists 7ec04b775b208175a41a3c108a6587d1 "convert-visio-vsdx-to-xaml.js" >}}

## Conclusion

In this article, we have seen how to convert MS Visio diagrams to various popular formats in Node.js applications. The conversion scenarios we have covered in this article include Visio to PDF, Visio to images (PNG, JPEG, etc.), Visio to SVG, Visio to HTML, and Visio to XAML. You can learn more about the Node.js Visio API from the [documentation][20].

## Related Article

*   [Create MS Visio Diagrams in Node.js Applications][21]




[1]: https://blog.aspose.com/2020/05/12/create-ms-visio-vsdx-diagrams-from-scratch-in-node.js-applications/
[2]: https://products.aspose.com/diagram/nodejs-java
[3]: #Convert-Visio-to-PDF-in-Node.js
[4]: #Convert-Visio-Diagram-to-PNG-JPEG-BMP-TIFF
[5]: #Export-Visio-Diagrams-to-SVG-in-Node.js
[6]: #Convert-Visio-Diagram-to-HTML-in-Node.js
[7]: #Visio-to-XAML-Conversion-in-Node.js
[8]: https://apireference.aspose.com/diagram/net/aspose.diagram/diagram
[9]: https://apireference.aspose.com/diagram/net/aspose.diagram.diagram/save/methods/2
[10]: https://apireference.aspose.com/diagram/net/aspose.diagram/diagram
[11]: https://apireference.aspose.com/diagram/net/aspose.diagram.saving/imagesaveoptions
[12]: https://apireference.aspose.com/diagram/net/aspose.diagram/savefileformat
[13]: https://apireference.aspose.com/diagram/net/aspose.diagram.diagram/save/methods/3
[14]: https://apireference.aspose.com/diagram/net/aspose.diagram/diagram
[15]: https://apireference.aspose.com/diagram/net/aspose.diagram.diagram/save/methods/2
[16]: https://apireference.aspose.com/diagram/net/aspose.diagram/diagram
[17]: https://apireference.aspose.com/diagram/net/aspose.diagram.diagram/save/methods/2
[18]: https://apireference.aspose.com/diagram/net/aspose.diagram/diagram
[19]: https://apireference.aspose.com/diagram/net/aspose.diagram.diagram/save/methods/2
[20]: https://docs.aspose.com/display/diagramjava/Product+Overview
[21]: https://blog.aspose.com/2020/05/12/create-ms-visio-vsdx-diagrams-from-scratch-in-node.js-applications/





