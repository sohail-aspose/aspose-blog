---
title: 'Create MS Visio Diagrams in Node.js Applications'
seoTitle: "Create MS Visio (VSDX) Diagrams in Node.Js | Visio API for Node.js"
description: "Create MS Visio diagrams from scratch in Node.js applications. Creare VSDX, VDX, VSX, and other Visio formats in JavaScript. Visio API for Node.js."
date: Tue, 12 May 2020 17:23:22 +0000
draft: false
url: /2020/05/12/create-ms-visio-vsdx-diagrams-from-scratch-in-node.js-applications/
author: Usman Aziz
summary: ''
tags: ['Add master to Visio diagram in Node.js', 'Add pages to Visio diagram in Node.js', 'Add shapes to Visio diagram in Node.js', 'Create MS Visio diagram in Node.js', 'Create Visio VSDX in Node.js', 'Visio API for Node.js']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose_diagram-for-nodejs-1.png" alt="">}}


[Aspose.Diagram for Java][1] is a feature-rich Java API for manipulating Visio diagrams programmatically without requiring **Microsoft Visio**. The API supports working with popular Visio formats including VSD, VSDX, VDX, VSDM, VSSM, and VSSX. Recently, we have leveraged the capabilities of Aspose.Diagram for Java and made it possible to implement MS Visio automation features in **Node.js** applications. These features let you create, manipulate, convert & process MS Visio diagrams within your Node.js application.

[Aspose.Diagram for Node.js via Java][2] provides a complete set of features to automate the creation or manipulation of Visio diagrams. You can create, read, export, print, and protect the diagrams quite easily in a few lines of code. In this article, I'll cover how to create Visio diagrams from scratch within a Node.js application. The rest of the article is divided into the following sections.

*   [Installation of Node.js Visio API][3]
*   [Create MS Visio Diagram from Scratch in Node.js][4]
*   [Add Master to Visio Diagram][5]
*   [Insert Pages in a Visio Diagram][6]
*   [Create a Shape in a Visio Diagram][7]
*   [Add a Text Shape in the Visio Page][8]
*   [Add Hyperlink to a Visio Shape][9]

## Node.js Visio API - Installation {#Installation-of-Node.js-Visio-API}

Use the following command to install Aspose.Diagram package in your Node.js application.

```
npm install aspose.diagram --save
```

## Create MS Visio Diagram in Node.js {#Create-MS-Visio-Diagram-from-Scratch-in-Node.js}

I'll start by creating an empty Visio diagram (VSDX) from scratch. The following are the steps to perform this operation.

*   Create an object of [Diagram][10] class.
*   Save the diagram as a file using [Diagram.save()][11] method.

The following code sample shows how to create a Visio diagram (VSDX) in a Node.js application.

{{< gist aspose-com-gists d4adedf6fd5115e7022c95bacaa806ce "create-visio-diagram.js" >}}

## Add Master to Visio Diagram in Node.js {#Add-Master-to-Visio-Diagram}

The Visio Stencils contain the collection of master shapes that are used to add/copy shapes in the Visio diagrams. You add a master to the Visio diagram using the VSS stencil file. The following are the steps to add a master using Aspose.Diagram.

*   Create a new Visio diagram using the [Diagram][12] class.
*   Add master to the diagram using the stencil file's path and master's name/ID.
*   Add shape to the diagram using the master's name.
*   Save diagram using [Diagram.save()][13] method.

The following code sample shows how to add a master to a Visio diagram in Node.js.

{{< gist aspose-com-gists d4adedf6fd5115e7022c95bacaa806ce "add-master-in-visio-diagram.js" >}}

## Insert Pages in a Visio Diagram in Node.js {#Insert-Pages-in-a-Visio-Diagram}

Before creating the shapes, you need to have at least one page in the Visio diagram. Each page in the Visio diagram has a name and id which is used to uniquely identify that page. The following are the steps to add a page in the Visio diagram.

*   Create an instance of the [Diagram][14] class.
*   Calculate the maximum page ID.
*   Create a new page using [Page][15] class.
*   Set page's name and ID using [Page.setName()][16] and [Page.setID()][17] method respectively.
*   Add page to diagram using [Diagram.getPages().add()][18] method.
*   Save the Visio diagram using [Diagram.save()][19] method.

The following code sample shows how to insert pages into a Visio diagram in Node.js.

{{< gist aspose-com-gists d4adedf6fd5115e7022c95bacaa806ce "add-page-in-visio-diagram.js" >}}

## Create a Shape in a Visio Diagram in Node.js {#Create-a-Shape-in-a-Visio-Diagram}

Once you have created the page in the diagram, you can add a shape to it. The following are the steps to create and insert a shape in the diagram.

*   Create an object of [Diagram][20] class.
*   Add master to the diagram using the stencil file's path.
*   Add a rectangle shape using [Diagram.addShape()][21] method.
*   Set shape's properties such as ID, text, position, fill color, etc.
*   Save the diagram using the [Diagram.save()][22] method.

The following code sample shows how to add a shape to the Visio diagram in Node.js.

{{< gist aspose-com-gists d4adedf6fd5115e7022c95bacaa806ce "add-shape-in-visio-diagram.js" >}}

## Add a Text Shape to a Visio Diagram in Node.js {#Add-a-Text-Shape-in-the-Visio-Page}

Aspose.Diagram also lets you add text to the Visio diagrams. In this case, the text is added as a shape. The following are the steps to add text to a Visio diagram.

*   Create a new Visio diagram using the [Diagram][23] class.
*   Add text shape to diagram using _Diagram.getPages().getPage(0).addText()_ method.
*   Save the diagram using [Diagram.save()][24] method.

The following code sample shows how to add text shape to the Visio diagram in Node.js.

{{< gist aspose-com-gists d4adedf6fd5115e7022c95bacaa806ce "add-text-in-visio-diagram.js" >}}

## Add Hyperlink to a Visio Shape in Node.js {#Add-Hyperlink-to-a-Visio-Shape}

Hyperlinks in Visio diagrams can be used to navigate from one page to another or to link a file or a web page to the drawing. The following are the steps to add a hyperlink to a Visio diagram.

*   Create a new Visio diagram.
*   Select the desired page from the diagram.
*   Select the desired [Shape][25] from the selected page.
*   Create a new hyperlink using the Hyperlink class and set its properties.
*   Add the hyperlink to the shape using [Shape.getHyperlinks().add()][26] method.
*   Save the diagram.

The following code sample shows how to add a hyperlink to a Visio diagram in Node.js.

{{< gist aspose-com-gists d4adedf6fd5115e7022c95bacaa806ce "add-hyperlink-in-visio-diagram.js" >}}

## Conclusion

In this article, you have learned how to create Visio diagrams/drawings from scratch in Node.js applications. The step by step tutorial and code samples showed how to add master, pages, shapes, text, and hyperlinks in the Visio diagram with a few lines of code. You can explore more about the Visio API for Node.js using the [documentation][27].

## Related Article(s)

*   [Draw Shapes in Visio Diagrams using C#][28]




[1]: https://www.aspose.com/products/diagram/java
[2]: https://products.aspose.com/diagram/nodejs-java
[3]: #Installation-of-Node.js-Visio-API
[4]: #Create-MS-Visio-Diagram-from-Scratch-in-Node.js
[5]: #Add-Master-to-Visio-Diagram
[6]: #Insert-Pages-in-a-Visio-Diagram
[7]: #Create-a-Shape-in-a-Visio-Diagram
[8]: #Add-a-Text-Shape-in-the-Visio-Page
[9]: #Add-Hyperlink-to-a-Visio-Shape
[10]: https://apireference.aspose.com/diagram/java/com.aspose.diagram/Diagram
[11]: https://apireference.aspose.com/diagram/java/com.aspose.diagram/diagram#save(java.lang.String,%20int)
[12]: https://apireference.aspose.com/diagram/java/com.aspose.diagram/Diagram
[13]: https://apireference.aspose.com/diagram/java/com.aspose.diagram/diagram#save(java.lang.String,%20int)
[14]: https://apireference.aspose.com/diagram/java/com.aspose.diagram/Diagram
[15]: https://apireference.aspose.com/diagram/java/com.aspose.diagram/Page
[16]: https://apireference.aspose.com/diagram/java/com.aspose.diagram/page#Name
[17]: https://apireference.aspose.com/diagram/java/com.aspose.diagram/page#ID
[18]: https://apireference.aspose.com/diagram/java/com.aspose.diagram/diagram#Pages
[19]: https://apireference.aspose.com/diagram/java/com.aspose.diagram/diagram#save(java.lang.String,%20int)
[20]: https://apireference.aspose.com/diagram/java/com.aspose.diagram/Diagram
[21]: https://apireference.aspose.com/diagram/java/com.aspose.diagram/diagram#addShape(double,%20double,%20double,%20double,%20java.lang.String,%20int)
[22]: https://apireference.aspose.com/diagram/java/com.aspose.diagram/diagram#save(java.lang.String,%20int)
[23]: https://apireference.aspose.com/diagram/java/com.aspose.diagram/Diagram
[24]: https://apireference.aspose.com/diagram/java/com.aspose.diagram/diagram#save(java.lang.String,%20int)
[25]: https://apireference.aspose.com/diagram/java/com.aspose.diagram/Shape
[26]: https://apireference.aspose.com/diagram/java/com.aspose.diagram/shape#Hyperlinks
[27]: https://docs.aspose.com/display/diagramjava/Product+Overview
[28]: https://blog.aspose.com/2019/09/05/draw-shapes-in-page-using-aspose.diagram-for-.net/





