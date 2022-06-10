---
title: 'Automatically Update Styles, Sign XPS & Register Hyphenation Dictionary in Aspose.Words 14.2.0'
date: Mon, 24 Mar 2014 00:20:10 +0000
draft: false
url: /2014/03/24/automatically-update-styles-sign-xps-register-hyphenation-dictionary-in-aspose.words-14.2.0/
author: Muhammad Ijaz
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

[![Aspose.Words logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2014/01/aspose.words_logo.png)Aspose.Words 14.2.0 has been released with this month’s release containing over 115 useful new features, enhancements and bug fixes to the Aspose.Words products.

You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 14.2.0][2]
*   [Aspose.Words for Java 14.2.0][3]
*   [Aspose.Words for Android 1.7][4]

Here is a look at just a few of the biggest features in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the links above.

## Automatically Update Styles

When the document (with this option set) is opened, changes to the styles in the attached template will automatically appear in this document. In Microsoft Word, this option is called **Automatically update document styles** and can be set through **Templates and Add-ins** dialogue as you can see in the following image.

[![][5]](https://blog.aspose.com/wp-content/uploads/sites/2/2014/03/AutoUpdateStyles.jpg)

Set the Document.AutomaticallyUpdateStyles option to **true** to let the styles update when document is opened in Microsoft Word.

```
Document doc
= new Document();
doc.AttachedTemplate = "MyTemplate.dot"; 

doc.AutomaticallyUpdateSyles
= true; 

doc.Save("out.docx"); 
```

## Register Hyphenation Dictionary

Aspose.Words now supports hyphenation. Prior to this release, the default hyphenation used by Aspose.Words was not suitable for some documents with hyphenation and was affecting the number of pages or position of words. A new class has been introduced to specify a hyphenation dictionary for required language. Use the Hyphenation.RegisterDictionary method to specify hyphenation dictionaries as you can see in the following code.

```
Hyphenation.RegisterDictionary("en-US", "C:/HyphDic/hyph_en_US.dic");

Hyphenation.RegisterDictionary("de-CH", "C:/HyphDic/hyph_de_CH.dic"); 
```

## Digitally Sign XPS Documents

Aspose.Words supports exporting Word documents to XPS and digitally sign output XPS documents. A new public method, LoadSignatures, has been introduced in DigitalSignatureUtil class. This method can be used to load signatures from DOC, DOCX, ODT and XPS documents.

```
DigitalSignatureCollection signatures = DigitalSignatureUtil.LoadSignatures(@"X:\test.xps");

MemoryStream stream = new MemoryStream(MiscUtil.CopyFileToByteArray(@"X:\test.docx")); 

DigitalSignatureCollection signaturesFromStream = DigitalSignatureUtil.LoadSignatures(stream); 
```




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/01/aspose.words_logo.png "Aspose.Words logo"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.words-for-.net/category1188.aspx
[3]: http://www.aspose.com/community/files/72/java-components/aspose.words-for-java/category1378.aspx
[4]: http://www.aspose.com/community/files/74/android-components/aspose.words-for-android/category1430.aspx
[5]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/03/AutoUpdateStyles.jpg "AutoUpdateStyles"




