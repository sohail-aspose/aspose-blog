---
title: 'Bind Content Control to Custom XML Parts in Word Documents'
date: Tue, 23 May 2017 06:53:56 +0000
draft: false
url: /2017/05/23/improved-toa-includetext-fields-bind-content-control-custom-xml-parts-many-aspose.words-17.5/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

We are pleased to announce our next version of Aspose.Words 17.5. This month’s release contains over 84 useful new features, enhancements and bug fixes. You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 17.5][1]
*   [Aspose.Words for Java 17.5][2]

Please see the [release notes][3] for more detail. If you are planning to upgrade from older version of Aspose.Words to the current version, we would strongly suggest you to check the [Public API and Backward Incompatible Changes][4] section to know what APIs are changed so far.

Here is a look at just a few of the biggest features and API changes in this month’s release.

*   MailMerge and Metafile Rendering Performance are Improved.
*   Support TOA, IMPORT, INCLUDE, SHAPE Fields.
*   API to bind SDT to CustomXML Properties is Provided.
*   Implemented Support for ShapeLayoutLikeWW8 Compatibility Option.
*   Improved Calculation of Width of Spaces in Asian Text.
*   Improved Text Wrapping for Lines Consisting of Many Tabs.
*   Improved Layout of Multi-Column Sections When Column Ends with Page Break Followed by Paragraph Break.
*   Alow Resolution Text Rendering to Images Improved.
*   Underlined Text in EMF+ Images are now Rendered into Fixed Page Formats.
*   HtmlFixed Output File Rendering Improved.
*   Image Crop is now Taken into Account While Rendering HtmlFixed.
*   Shaded DrawingML Images Rendering Fixed.
*   DrawingML Charts rendering improved (axis label placement).

## Added Feature to Set left/top/right/bottom Padding of Table's Cell

We have added new method CellFormat.SetPaddings in Aspose.Words 17.5. The method is used to set the amount of space (in points) to add to the left/top/right/bottom of the contents of cell. Please read the following article for more detail:

[Applying Formatting on the Cell Level][5]

## Implemented API to Bind StructuredDocumentTag to Node of Custom XML Part

We have added new feature in Aspose.Words 17.5 to  bind content controls with XML data (custom XML part) in Word documents. The XmlMapping class is used to specify the information that is used to establish a mapping between the parent structured document tag and an XML element stored within a custom XML data part in the document. 

```
/// <summary>
/// Gets an object that represents the mapping of this structured document tag to XML data
/// in a custom XML part of the current document.
/// </summary>
/// <remarks>
/// You can use the <see cref="Markup.XmlMapping.SetMapping"/> method of this object to map
/// a structured document tag to XML data.
/// </remarks>
public XmlMapping XmlMapping { get; }
```
```
/// <summary>
/// Specifies the information that is used to establish a mapping between the parent
/// structured document tag and an XML element stored within a custom XML data part in the document.
/// </summary>
public class XmlMapping
{
    /// <summary>
    /// Sets a mapping between the parent structured document tag and an XML node of a custom XML data part.
    /// </summary>
    /// <param name="customXmlPart">A custom XML data part to map to.</param>
    /// <param name="xPath">An XPath expression to find the XML node.</param>
    /// <param name="prefixMapping">XML namespace prefix mappings to evaluate the XPath.</param>
    /// <returns>A flag indicating whether the parent structured document tag is successfully mapped to
    /// the XML node.</returns>
    public bool SetMapping(CustomXmlPart customXmlPart, string xPath, string prefixMapping);
 
    /// <summary>
    /// Deletes mapping of the parent structured document to XML data.
    /// </summary>
    public void Delete();
 
    /// <summary>
    /// Returns the custom XML data part to which the parent structured document tag is mapped.
    /// </summary>
    public CustomXmlPart CustomXmlPart { get; }
 
    /// <summary>
    /// Returns the XPath expression, which is evaluated to find the custom XML node
    /// that is mapped to the parent structured document tag.
    /// </summary>
    public string XPath { get; }
 
    /// <summary>
    /// Returns XML namespace prefix mappings to evaluate the <see cref="XPath"/>.
    /// </summary>
    /// <remarks>
    /// Specifies the set of prefix mappings, which shall be used to interpret the XPath expression
    /// when the XPath expression is evaluated against the custom XML data parts in the document.
    /// </remarks>
    public string PrefixMappings { get; }
 
    /// <summary>
    /// Returns <b>true</b> if the parent structured document tag is successfully mapped to XML data.
    /// </summary>
    public bool IsMapped { get; }
}
```

## Added Public Method CustomXmlPartCollection.Add(string id, string xml)

We have added CustomXmlPartCollection.Add method in Aspose.Words 17.5. This method creates a new XML part with the specified XML and adds it to the collection.   

```
/// <summary>
/// Creates a new XML part with the specified XML and adds it to the collection.
/// </summary>
/// <param name="id">Identifier of a new custom XML part.</param>
/// <param name="xml">XML data of the part.</param>
/// <returns>Created custom XML part.</returns>
public CustomXmlPart Add(string id, string xml)
```

## Aspose.Words for .NET Resources

The following resources will help you work with Aspose.Words for .NET:

*   [Home of Aspose.Words for .NET API][6].
*   [Aspose.Words for .NET Download Section][7].
*   [Aspose.Words for .NET Documentation][8] – up-to-date documentation containing Programmer’s Guide, Knowledge Base and much more.
*   [Aspose.Words for .NET API Reference Guide][9] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   Aspose.Words Product Family Forum – post your technical questions and queries, or any other problem you are facing while working with Aspose.Words APIs.
    *   [Free Support Forum][10]
    *   [Paid Support Forum][11]
*   [Enable Blog Subscription][12] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
*   [Aspose.Words for .NET Examples][13] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/words/net
[2]: https://downloads.aspose.com/words/java
[3]: https://docs.aspose.com/words/net/aspose-words-for-net-17-5-release-notes/
[4]: https://docs.aspose.com/words/net/aspose-words-for-net-17-5-release-notes/
[5]: https://docs.aspose.com/words/net/applying-formatting/#ApplyingFormatting-ApplyingFormattingontheCellLevel
[6]: https://www.aspose.com/products/words/net
[7]: https://downloads.aspose.com/words/net
[8]: https://docs.aspose.com/words/net/
[9]: https://apireference.aspose.com/net/words
[10]: https://forum.aspose.com/c/words
[11]: https://helpdesk.aspose.com/
[12]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[13]: https://github.com/aspose-words/Aspose.Words-for-.NET




