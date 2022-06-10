---
title: 'Improved SVG Images Rendering and Adjust Space between Asian and Latin Text/Numbers in Aspose.Words for .NET 17.6'
date: Mon, 12 Jun 2017 08:59:01 +0000
draft: false
url: /2017/06/12/support-automatically-adjust-space-asian-latin-text-numbers-many-aspose.words-17.6/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

[](http://www.aspose.com/.net/word-component.aspx)We are pleased to announce our next version [Aspose.Words for .NET 17.6][1]. This month’s release contains over 82 useful new features, enhancements and bug fixes. Please see the [release notes][2] for more detail. If you are planning to upgrade from older version of Aspose.Words to the current version, we would strongly suggest you to check the [Public API and Backward Incompatible Changes][3] section to know what APIs are changed so far.

  
Here is a look at just a few of the biggest features and API changes in this month’s release.

*   Added feature to Automatically adjust space between Asian and Latin text, numbers.
*   Throw warnings when an external resource in HTML could not be loaded.
*   Track changes view settings in LibreOffice.
*   Added ability to reference to data from parent region in child regions.
*   Implemented support for distributed paragraph alignment.
*   Improved handling of justified alignment in Asian text.
*   Improved line height calculation for inline images in Asian text
*   Improved handling of hidden paragraph breaks around text frames
*   Improved text wrapping of sections breaks around floating objects
*   Improved Aps logical structure generation for repeated header rows
*   SVG graphics are now rendered via internal EMF rendering engine (without GDI+).
*   Improved rendering of PDF logical structure of Table headers.
*   Character offsets in META\_EXTTEXTOUT records are now taken into account while rendering multi-byte encoding meta-files.

## Improved SVG Images Rendering

We have improved SVG image rendering technique in this version. Earlier, upon inserting SVG image into the document, it is converted to meta-file (EMF) using GDI+. We have noticed that GDI+ is not working as expected in multi-threading approach, exception occurs in GDI+. To prevent problems with multi-threading, we have switched to our own EMF rendering engine instead of GDI+.

## Added Public Properties ParagraphFormat.AddSpaceBetweenFarEastAndAlpha and ParagraphFormat.AddSpaceBetweenFarEastAndDigit

We have added support of automatically adjust space between Asian and Latin text, Asian text and numbers in Aspose.Words for .NET 17.6. We have added two public properties in ParagraphFormat class AddSpaceBetweenFarEastAndAlpha and AddSpaceBetweenFarEastAndDigit to achieve this. Please read the following article for more detail:  
[Automatically Adjust Space between Asian and Latin text, Numbers][4]

```
/// <summary>
/// Gets or sets a flag indicating whether inter-character spacing is automatically adjusted between regions
/// of Latin text and regions of East Asian text in the current paragraph.
/// </summary>
public bool AddSpaceBetweenFarEastAndAlpha { get; set; }
 
/// <summary>
/// Gets or sets a flag indicating whether inter-character spacing is automatically adjusted between regions
/// of numbers and regions of East Asian text in the current paragraph.
/// </summary>
public bool AddSpaceBetweenFarEastAndDigit { get; set; }
```

## Added Public Property HtmlLoadOptions.PreferredControlType

We have added new feature in Aspose.Words for .NET 17.6 to import <input> and <select> elements as content control (SDT) during HTML to DOCX conversion.  Please refer to the following article for more detail:  
[Save HTML tags Input and Select as Content Control][5]

```
/// <summary>
/// Type of document nodes that represent <input> and <select> elements imported from HTML.
/// </summary>
public enum HtmlControlType
{
    FormField,
    StructuredDocumentTag
}
 
 
/// <summary>
/// Gets or sets preffered type of document nodes that will represent imported <input> and <select> elements.
/// Default value is <see cref="HtmlControlType.FormField"/>.
/// </summary>
/// <remarks>
/// Please note that setting this property does not guarantee that all imported controls will be of the specified type.
/// If an HTML control is not representable with document nodes of the preferred type, Aspose.Words will use
/// a compatible <see cref="HtmlControlType"/> for that control.
/// </remarks>
public HtmlControlType PreferredControlType
{
    get { return mPreferedControlType; }
    set { mPreferedControlType = value; }
} 
```

Use case:

```
 HtmlLoadOptions lo = new HtmlLoadOptions();
lo.PreferredControlType = HtmlControlType.StructuredDocumentTag;
Document doc = new Document(@"input.html", lo); 
```

## Aspose.Words for .NET Resources

The following resources will help you work with Aspose.Words for .NET:

*   [Home of Aspose.Words for .NET API][6].
*   [Aspose.Words for .NET Download Section][7].
*   [Install Aspose.Words for .NET NuGet Package][8]
*   [Aspose.Words for .NET Documentation][9] – up-to-date documentation containing Programmer’s Guide, Knowledge Base and much more.
*   [Aspose.Words for .NET API Reference Guide][10] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   Aspose.Words Product Family Forum – post your technical questions and queries, or any other problem you are facing while working with Aspose.Words APIs.
    *   [Free Support Forum][11]
    *   [Paid Support Forum][12]
*   [Enable Blog Subscription][13] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
*   [Aspose.Words for .NET Examples][14] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/words/net/new-releases/aspose.words-for-.net-17.6/
[2]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+17.6+Release+Notes
[3]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET
[4]: https://docs.aspose.com/display/wordsnet/Using+DocumentBuilder+to+Modify+a+Document+Easily#UsingDocumentBuildertoModifyaDocumentEasily-AutomaticallyAdjustSpacebetweenAsianandLatintext,Numbers
[5]: https://docs.aspose.com/display/wordsnet/Saving+a+Document#SavingaDocument-SaveHTMLtagsInputandSelectasContentControl
[6]: https://www.aspose.com/products/words/net
[7]: https://downloads.aspose.com/words/net
[8]: https://www.nuget.org/packages/Aspose.Words/
[9]: https://docs.aspose.com/display/wordsnet
[10]: https://apireference.aspose.com/net/words
[11]: https://forum.aspose.com/c/words
[12]: https://helpdesk.aspose.com/
[13]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[14]: https://github.com/aspose-words/Aspose.Words-for-.NET




