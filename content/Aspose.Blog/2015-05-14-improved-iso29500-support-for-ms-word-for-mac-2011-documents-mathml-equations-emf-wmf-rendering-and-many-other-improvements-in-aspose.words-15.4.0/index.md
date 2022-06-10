---
title: 'Improved Iso29500 Support for MS Word for Mac 2011 documents, MathML Equations, EMF, WMF rendering and many other Improvements in Aspose.Words 15.4.0'
date: Thu, 14 May 2015 15:54:20 +0000
draft: false
url: /2015/05/14/improved-iso29500-support-for-ms-word-for-mac-2011-documents-mathml-equations-emf-wmf-rendering-and-many-other-improvements-in-aspose.words-15.4.0/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

[](http://www.aspose.com/.net/word-component.aspx)Aspose.Words 15.4.0 has been released. This month’s release contains over 110 useful new features, enhancements and bug fixes to the Aspose.Words products.

You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 15.4.0][1]
*   [Aspose.Words for Java 15.4.0][2]

Here is a look at just a few of the biggest features and API changes in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the links above.

*   MathML equations rendering inside shapes implemented
*   MathML equations vertical positioning improved when rendering
*   Improved Iso29500 support for MS Word for Mac 2011 documents
*   Improved page number calculation, footnote balancing, nested floating tables and text wrapping around floating objects
*   EMF and WMF rendering improvements
*   Added some new public members to HTML save options and shapes/drawing
*   Over 30 improvements to DocumentBuilder, TXT, ODT and Microsoft Word document formats

## HtmlFixedSaveOptions.CssClassNamesPrefix Public Property Added

We have added new public property to HtmlFixedSaveOptions class:

```
 /// <summary>
/// Specifies prefix which is added to all class names in style.css file.
/// Default value is <c>"aw"</c>.
/// </summary>
public string CssClassNamesPrefix
{
    get { return mCssClassNamesPrefix; }
    set { mCssClassNamesPrefix = value; }
} 
```

This property behaves similar way as HtmlSaveOptions.CssClassNamesPrefix property for Aspose.Pdf. Please check the following article:

PDF to HTML - Prefix CSS Class Names in style.css

This is how simple style.css looked in previous Aspose.Words releases:

```
 div {
    position:absolute;
}
span {
    position:absolute;
    white-space:nowrap;
    color:#000000;
    font-size:12pt;
}
img {
    position:absolute;
}
svg {
    position:absolute;
}
page {
    position:relative;
    border:solid 1pt black;
    margin:10pt auto 10pt auto;
    overflow:hidden;
}
.text1 {
    font-family:'Calibri';
    font-style:normal;
    font-weight:normal;
} 
```

Both element and class selectors are used. In order to provide Aspose.Pdf's HtmlSaveOptions.CssClassNamesPrefix behavior now style.css looks like this:

```
 .awdiv {
    position:absolute;
}
.awspan {
    position:absolute;
    white-space:nowrap;
    color:#000000;
    font-size:12pt;
}
.awimg {
    position:absolute;
}
.awsvg {
    position:absolute;
}
.awpage {
    position:relative;
    border:solid 1pt black;
    margin:10pt auto 10pt auto;
    overflow:hidden;
}
.awtext1 {
    font-family:'Calibri';
    font-style:normal;
    font-weight:normal;
} 
```

Only class selectors are used which allows to prefix all class names.

## HtmlSaveOptions.ExportOriginalUrlForLinkedImages Public Property Added

We have added new public property to HtmlSaveOptions class:

```
 /// <summary>
/// Specifies whether original URL should be used as the URL of the linked images.
/// Default value is <c>false</c>.
/// </summary>
/// <remarks>
/// <para>If value is set to <c>true</c> <see cref="ImageData.SourceFullName"/> value is used as the URL of linked images
/// and linked images are not loaded into document's folder or <see cref="HtmlSaveOptions.ImagesFolder"/>.</para>
/// <para>If value is set to <c>false</c> linked images are loaded into document's folder or <see cref="HtmlSaveOptions.ImagesFolder"/>
/// and URL of each linked image is constructed depending on document's folder, <see cref="HtmlSaveOptions.ImagesFolder"/>
/// and <see cref="HtmlSaveOptions.ImagesFolderAlias"/> properties.</para>
/// </remarks>
public bool ExportOriginalUrlForLinkedImages
{
    get { return mExportOriginalUrlForLinkedImages; }
    set { mExportOriginalUrlForLinkedImages = value; }
} 
```

## ShapeBase.IsSignatureLine Public Property Added

Previously, the API didn't provide any clues to whether a shape is a signature line or not, except for a hint under Alternative Text. This property provides a way to distinguish signature line shapes.

## Unknown Fields now Merged during Mail Merge like in MS Word

While analyzing WORDSNET-11716, we have discovered that Word merges unknown fields like ﻿{ City } which normally serve as bookmark references. The fields are merged even though there are corresponding bookmarks in the document. We've decided to implement similar behavior due to the "do like Word" policy. However, this is a noticeable behavioral change to be published to our customers.




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.words-for-.net/default.aspx
[2]: http://www.aspose.com/community/files/72/java-components/aspose.words-for-java/default.aspx




