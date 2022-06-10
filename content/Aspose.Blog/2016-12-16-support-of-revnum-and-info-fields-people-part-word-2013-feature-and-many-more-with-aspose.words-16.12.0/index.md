---
title: 'Support of REVNUM and INFO Fields, "people" Part (Word 2013 feature), and many more with Aspose.Words 16.12.0'
date: Fri, 16 Dec 2016 09:06:03 +0000
draft: false
url: /2016/12/16/support-of-revnum-and-info-fields-people-part-word-2013-feature-and-many-more-with-aspose.words-16.12.0/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

[](http://www.aspose.com/.net/word-component.aspx)Aspose.Words 16.12.0 has been released. This month’s release contains over 73 useful new features, enhancements and bug fixes to the Aspose.Words product.

You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 16.12.0][1]
*   [Aspose.Words for Java 16.12.0][2]

Here is a look at just a few of the biggest features and API changes in this month’s release.

*   Save to image formats can be fine-tuned by passing RenderingHints (TextRenderingHint, InterpolationMode etc.) to ImageSaveOptions.GraphicsQualityOptions
*   Support of the "people" part (Word 2013 feature)
*   StructuredDocumentTag extensions supported (Word 2013 feature)
*   REVNUM, INFO fields supported
*   Improved handling of hanging punctuation and hyphens in complex script content
*   Improved handling of "Automatically adjust space between Asian text and numbers" compatibility option
*   Improved paragraph alignment when text contains hidden content
*   Improved reflow of vertically merged cells for complex table grid layout
*   Implemented combining adjacent tables on document loading
*   Path gradient fill support while rendering SVG implemented
*   Leader lines rendering for all DrawingML Chart types (not only for pie-charts) implemented
*   Styles are now properly applied for DrawingML Charts while rendering

## Added feature to support REVNUM and INFO Fields

We have added [FieldInfo][3] and [FieldRevNum][4] classes in Aspose.Wrods v16.12.0 to support [REVNUM][5] and [INFO][6] fields.

## Added new property [ImageSaveOptions.GraphicsQualityOptions][7] to Save fine-tuned Image

We have added ImageSaveOptions.GraphicsQualityOptions property in Aspose.Wrods v16.12.0. This property allows to specify rendering mode and quality for the Graphics object. Use this property to override the Graphics settings provided by Aspose.Words engine by default. It will take effect only when a document is being saved to an image-like format.

## Support of the "people" part (Word 2013 feature)

We have included the roundtrip support of the People part (OOXML format) in Aspose.Words v16.12.0. This part contains contact information about each person who has authored a comment or revision in the current document: identity provider (none, Active Directory or Windows Live ID) and user ID. Using this information MS Word can show additional information about contact.




[1]: http://www.aspose.com/downloads/words-family/net
[2]: http://www.aspose.com/downloads/words-family/java
[3]: http://www.aspose.com/api/net/words/aspose.words.fields/fieldrevnum
[4]: http://www.aspose.com/api/net/words/aspose.words.fields/fieldinfo
[5]: https://support.office.com/en-us/article/Field-codes-RevNum-field-40eb1d97-4b55-4d5c-a5e5-88edf20612da?ui=en-US&rs=en-US&ad=US
[6]: https://support.office.com/en-us/article/Field-codes-Info-field-131e3e52-ded0-4575-b0b5-de50ab7e5b43?ui=en-US&rs=en-US&ad=US
[7]: http://www.aspose.com/api/net/words/aspose.words.saving/imagesaveoptions/properties/graphicsqualityoptions




