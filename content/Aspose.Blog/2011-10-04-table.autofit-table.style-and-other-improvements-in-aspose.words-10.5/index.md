---
title: 'Table.AutoFit, Table.Style and Other Improvements in Aspose.Words 10.5'
date: Tue, 04 Oct 2011 04:04:24 +0000
draft: false
url: /2011/10/04/table.autofit-table.style-and-other-improvements-in-aspose.words-10.5/
author: Romank
summary: ''
tags: ['.NET', 'Apply Style to Table in Word', 'Auto Fit Table in Word Documents', 'Microsoft Word', 'product release', 'tables']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose.words-logo2.jpg" alt="ASpose.Words icon">}}


This post is about our latest Aspose.Words 10.5 release. We regularly produce a new release at the end of each month and each release contains around one hundred improvements and fixes.

As usual, you can download Aspose.Words from:

*   [Aspose.Words for .NET 10.5.0][1]
*   [Aspose.Words for Java 10.5.0][2]

## Improvements in the Public API for Tables

Earlier versions of Aspose.Words had some in the area of formatting tables, rows and cells programmatically. It is sufficient to mention that "table formatting" was not directly available on the Table object, instead you had to apply it to every row using Row.RowFormat object. Also, it was not possible to specify cell width in percent (a.k.a preferred width). These limitations also manifested themselves in behaviors that some customers considered as defects.

I am happy to announce that we've given the table formatting API a significant face lift. New code examples were added to the API Reference and to the Samples projects. The documentation will reflect the new features soon. Here is the list of what's new:

*   **PreferredWidth** class and **PreferredWidthType** enum added that allow to specify cell or table width in points or percent.
*   **CellFormat.PreferredWidth** and **Table.PreferredWidth** properties added.
*   **Table.Style**, **Table.StyleName** and **Table.StyleOptions** properties added that allow you to apply table styles to a table. Also see the new **TableStyleOptions**enum.
*   Table formatting properties such as **Alignment**, **AllowAutoFit**, **Bidi**, **LeftIndent, CellSpacing, Padding** were added to the **Table**object. The same properties were marked obsolete on the **RowFormat** object.
*   The new **Table.AutoFit** method was added to allow you easily format an entire table using one of the "standard Microsoft Word options": Auto Fit to Contents, Auto Fit to Window and Fixed Column Widths.
*   Convenience methods to work shading and borders **Table.SetBorders**, **Table.SetShading** and **Table.ClearBorders**, **Table.ClearShading** have been added.

## Chinese and Japanese Improvements

We have made a number of improvements in Aspose.Words to support these languages. Most notable points are:

*   Line breaking for Chinese and Japanese documents when rendering to PDF, XPS and printing works according to the language rules and also settings stored in the document.
*   Japanese formats for dates are now supported by the field update engine.

## Control how Images and CSS are Loaded

When you load an HTML document into Aspose.Words and the document contains links to images, then by default, Aspose.Words tries to download those images and embed them into the document. We thought this is the "normal" use case because sometimes image dimensions are not known from HTML, but they are requried for a shape in a Word document, but several customers have requested that provide some options to customize this behavior.

Finally Aspose.Words allows you to take control over how images and CSS stylesheets are loaded. You can even completely circumvent where the data comes from. This for example, makes certain "Aspose.Words in the cloud" scenarios easier to implement.

Here is what's been added:

*   **LoadOptions.ResourceLoadingCallback** property
*   **IResourceLoadingCallback** interface, **ResourceLoadingAction**enum, **ResourceLoadingArgs** class.

## Print Word Documents in Java

In the previous blog I hinted this feature is coming. Now I am happy to let you know the family of **Document.Print** methods are available for you. You can now easily print all or only specified pages of a document. Aspose.Words integrates with the Java's printing framework and this means you can customize the print process to your liking. Aspose.Words implements **AsposeWordsPrintDocument** class that provides the "typical" one document page per physical page printing. But it is easy (and we will provide code examples) to print multiple document pages onto a physical page by implementing your own print document class.




[1]: https://downloads.aspose.com/words/net
[2]: https://downloads.aspose.com/words/java




