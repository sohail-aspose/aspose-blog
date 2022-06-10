---
title: 'Export Word Document to HTML5 and Optimize Fixed Page Document'
date: Tue, 08 Nov 2016 10:27:02 +0000
draft: false
url: /2016/11/08/support-of-export-document-to-html5-optimization-of-fixed-page-document-and-many-more-with-aspose.words-16.11.0/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

[](http://www.aspose.com/.net/word-component.aspx)Aspose.Words 16.11.0 has been released. This month’s release contains over 74 useful new features, enhancements and bug fixes to the Aspose.Words product.

You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 16.11.0][1]
*   [Aspose.Words for Java 16.11.0][2]

Here is a look at just a few of the biggest features and API changes in this month’s release.

*   Support of Export Document to HTML5
*   Optimization of Fixed Page Document
*   Output PDF now Contains a Valid Document ID Despite the Compliance Settings
*   Support of MS Word 2013 Features from Various DOCX Extension Specifications

## Support export to HTML5

We have added a new feature in Aspose.Wrods v16.11.0 to export document to HTML5. The HtmlSaveOptions.HtmlVersion property can be used to specify version of HTML standard that should be used when saving the document to HTML or MHTML. Default value is Xhtml.

### Added New public Enumeration HtmlVersion```
/// <summary>
/// Indicates the version of HTML is used when saving the document to <see cref="SaveFormat.Html"/> and 
/// <see cref="SaveFormat.Mhtml"/> formats.
/// </summary>
public enum HtmlVersion
{
    /// <summary>
    /// Saves the document in compliance with the XHTML 1.0 Transitional standard. 
    /// </summary>
    /// <remarks>
    /// Aspose.Words aims to output XHTML according to the XHTML 1.0 Transitional standard, 
    /// but the output will not always validate against the DTD. Some structures inside a Microsoft Word 
    /// document are hard or impossible to map to a document that will validate against the XHTML schema. 
    /// For example, XHTML does not allow nested lists (UL cannot be nested inside another UL element), 
    /// but in Microsoft Word document multilevel lists occur quite often.
    /// </remarks>
    Xhtml,
    /// <summary>
    /// Saves the document in compliance with the HTML 5 standard. 
    /// </summary>
    Html5
}
```

### Added New public property in HtmlSaveOptions```
/// <summary>
/// Specifies version of HTML standard that should be used when saving the document to HTML or MHTML.
/// Default value is <see cref="Saving.HtmlVersion.Xhtml"/>.
/// </summary>
public HtmlVersion HtmlVersion
{
     get { return mHtmlVersion; }
     set { mHtmlVersion = value; }
}

```

## Optimization of FixedPage Document

Starting from Aspose.Words v16.11.0, OptimizeOutput option is available for all fixed page formats.

```
/// <summary>
/// Flag indicates whether it is required to optimize output of XPS.
/// If this flag is set redundant nested canvases and empty canvases are removed,
/// also neighbor glyphs with the same formating are concatenated.
/// Note: The accuracy of the content display may be affected if this property is set to true.
///
/// Default is false.
/// </summary>
public virtual bool OptimizeOutput
{
    get { return mOptimizeOutput; }
    set { mOptimizeOutput = value; }
}
```




[1]: http://www.aspose.com/downloads/words-family/net
[2]: http://www.aspose.com/downloads/words-family/java




