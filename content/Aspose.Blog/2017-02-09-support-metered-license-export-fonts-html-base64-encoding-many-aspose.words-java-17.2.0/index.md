---
title: 'Export Fonts to HTML in Base64 Encoding with Aspose.Words for Java 17.2.0'
date: Thu, 09 Feb 2017 10:49:03 +0000
draft: false
url: /2017/02/09/support-metered-license-export-fonts-html-base64-encoding-many-aspose.words-java-17.2.0/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

We are pleased to announce our next version of [Aspose.Words for Java 17.2.0][1]. This month’s release contains over 51 useful new features, enhancements and bug fixes. Please see the [release notes][2] for more detail. If you are planning to upgrade from old version of Aspose.Words to the current version, we would strongly suggest you to check the [Public API and Backward Incompatible Changes][3] section to know what APIs are changed so far.

Here is a look at just a few of the biggest features and API changes in this month’s release.

*   Support of Metered License
*   Export fonts to HTML in Base64 encoding
*   Added HtmlSaveOptions.ResourceFolder and HtmlSaveOptions.ResourceFolderAlias public Properties
*   Exposed access to Height/Width of Text Frames
*   Improved control over BiDi text direction elements
*   Non-bidi fields that contain hided bidi whitespaces are properly resolved

## Introduced Metered Licensing

Starting from 17.2.0 version, Aspose.Words for Java provides the functionality to use metered licensing mechanism. Aspose.Words allows developers to apply metered key. It is a new licensing mechanism. The new licensing mechanism will be used along with existing licensing method. Those customers who want to be billed based on the usage of the API features can use the metered licensing. Following code example shows how to set metered public and private keys.

```
// set metered public and private keys
Metered metered = new Metered();
// Access the setMeteredKey property and pass public and private keys as parameters
metered.setMeteredKey("*****", "*****");
//Load the document
Document doc = new Document(MyDir + "in.docx");
//Get the page count of document
System.out.println(doc.getPageCount());
```

## Added Public Property HtmlSaveOptions.ExportFontsAsBase64

We have introduced new property HtmlSaveOptions.ExportFontsAsBase64 in Aspose.Words 17.2.0. This property allows user to embed fonts resources to HTML in Base64 encoding. Please review the following article for more detail.  
[Export fonts to HTML in Base64 encoding][4]

```
/// <summary>
/// Specifies whether fonts resources should be embedded to HTML in Base64 encoding.
/// Default is <c>false</c>.
/// </summary>
/// <remarks>
/// By default, fonts are written to separate files. If this option is set to <c>true</c>, fonts will be embedded
/// into the document's CSS in Base64 encoding.
/// </remarks>
public bool ExportFontsAsBase64 {
    get { return mExportFontsAsBase64; }
    set { mExportFontsAsBase64 = value; }
} 
```

Use Case:

```
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
saveOptions.setExportFontResources(true);
saveOptions.ExportFontsAsBase64(true);
doc.save(fileName, saveOptions);
```

## Added Public Property HtmlSaveOptions.ResourceFolder

We have introduced new property HtmlSaveOptions.ResourceFolder in Aspose.Words 17.2.0. This property is used to Specify a physical folder where all resources like images, fonts, and external CSS are saved when a document is exported to HTML. The default value of this property is an empty string. Please review the following article for more detail.  
Working with HtmlSaveOptions properties

```
/// <summary>
/// Specifies a physical folder where all resources like images, fonts, and external CSS are saved when a document
/// is exported to HTML. Default is an empty string.
/// </summary>
/// <remarks>
/// <see cref="ResourceFolder"/> is the simplest way to specify a folder where all resources should be written.
/// Another way is to use individual properties <see cref="FontsFolder"/>, <see cref="ImagesFolder"/>,
/// and <see cref="CssStyleSheetFileName"/>.
///
/// <see cref="ResourceFolder"/> has a lower priority than folders specified via <see cref="FontsFolder"/>,
/// <see cref="ImagesFolder"/>, and <see cref="CssStyleSheetFileName"/>. For example, if both <see cref="ResourceFolder"/>
/// and <see cref="FontsFolder"/> are specified, fonts will be saved to <see cref="FontsFolder"/>, while images and CSS
/// will be saved to <see cref="ResourceFolder"/>.
///
/// If the folder specified by <see cref="ResourceFolder"/> doesn't exist, it will be created automatically.
///
/// <seealso cref="FontsFolder"/>
/// <seealso cref="ImagesFolder"/>
/// <seealso cref="CssStyleSheetFileName"/>
/// </remarks>
public string ResourceFolder
{
    get { return mResourceFolder; }
    set
    {
        ArgumentUtil.CheckNotNull(value, "ResourceFolder");
        mResourceFolder = value;
    }
}
```

Use Case:

```
Document doc = new Document("C:\Test.docx");
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
saveOptions.setCssStyleSheetType(CssStyleSheetType.External);
saveOptions.setExportFontResources(true);
saveOptions.setResourceFolder("C:\Resources");
doc.save("C:\Test.html", saveOptions);
```

## Added Public Property HtmlSaveOptions.ResourceFolderAlias

We have introduced new property HtmlSaveOptions.ResourceFolderAlias in Aspose.Words 17.2.0. This property is used to specify the name of the folder used to construct URIs of all resources written into an HTML document. The default value of this property is an empty string. Please review the following article for more detail.  
Working with HtmlSaveOptions properties

```
/// <summary>
/// Specifies the name of the folder used to construct URIs of all resources written into an HTML document.
/// Default is an empty string.
/// </summary>
/// <remarks>
/// <see cref="ResourceFolderAlias"/> is the simplest way to specify how URIs for all resource files should be
/// constructed. Same information can be specified for images and fonts separately via <see cref="ImagesFolderAlias"/>
/// and <see cref="FontsFolderAlias"/> properties, respectively. However, there is no individual property for CSS.
///
/// <see cref="ResourceFolderAlias"/> has lower priority than <see cref="FontsFolderAlias"/>
/// and <see cref="ImagesFolderAlias"/>. For example, if both <see cref="ResourceFolderAlias"/>
/// and <see cref="FontsFolderAlias"/> are specified, fonts' URIs will be constructed using <see cref="FontsFolderAlias"/>,
/// while URIs of images and CSS will be constructed using <see cref="ResourceFolderAlias"/>.
///
/// If <see cref="ResourceFolderAlias"/> is empty, the <see cref="ResourceFolder"/> property value will be used
/// to construct resource URIs.
///
/// If <see cref="ResourceFolderAlias"/> is set to '.' (dot), resource URIs will contain file names only, without
/// any path.
///
/// <seealso cref="ResourceFolder"/>
/// <seealso cref="FontsFolderAlias"/>
/// <seealso cref="ImagesFolderAlias"/>
/// </remarks>
public string ResourceFolderAlias
{
    get { return mResourceFolderAlias; }
    set
    {
        ArgumentUtil.CheckNotNull(value, "ResourceFolderAlias");
        mResourceFolderAlias = value;
    }
} 
```

Use Case:

```
Document doc = new Document("C:\Test.docx");
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
saveOptions.setCssStyleSheetType(CssStyleSheetType.External);
saveOptions.setExportFontResources(true);
saveOptions.setResourceFolder("C:\Resources");
saveOptions.setResourceFolderAlias("http://example.com/resources");
doc.save("C:\Test.html", saveOptions);
```

## Aspose.Words for Java Resources

The following resources will help you work with Aspose.Words for Java:

*   [Home of Aspose.Words for Java API][5].
*   [Aspose.Words for Java Download Section][6].
*   [Aspose.Words for Java Documentation][7] – up-to-date documentation containing Programmer’s Guide, Knowledge Base and much more.
*   [Aspose.Words for Java API Reference Guide][8] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Words Product Family Forum][9] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Words APIs.
*   [Enable Blog Subscription][10] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
*   [Aspose.Words for Java Examples][11] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: http://downloads.aspose.com/words/java
[2]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+17.2.0+Release+Notes
[3]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+17.2.0+Release+Notes
[4]: https://docs.aspose.com/display/wordsjava/Converting+a+Microsoft+Word+document+using+save+Method#ConvertingaMicrosoftWorddocumentusingsaveMethod-ExportFontstoHTMLinBase64Encoding
[5]: https://www.aspose.com/products/words/java
[6]: http://downloads.aspose.com/words/java
[7]: https://docs.aspose.com/display/wordsjava/Home
[8]: https://www.aspose.com/api/java/words
[9]: https://www.aspose.com/community/forums/aspose.words-product-family/75/showforum.aspx
[10]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[11]: https://github.com/aspose-words/Aspose.Words-for-Java




