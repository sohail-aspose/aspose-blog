---
title: 'Password Protect ODT OTT Files Support in Aspose.Words for Android via Java'
date: Tue, 17 Apr 2018 10:58:59 +0000
draft: false
url: /2018/04/17/password-protect-odt-ott/
author: Awais Hafeez
summary: ''
tags: ['Password protect ODT', 'Password protect OTT', 'encrypt ODT', 'encrypt OTT']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose_words-for-android-128x128.png" alt="Password ODT and OTT file">}}


We are pleased to announce the new monthly release of **Aspose.Words for Android via Java 18.4**. Aspose.Words for Android via Java has full functionality of Aspose.Words for Java with [few limitations, minor API changes and additional requirements][1]. This version also includes all bug fixes and public API changes made in Aspose.Words for Java 18.4, see following release notes for more information.

[Aspose.Words for Java 18.4 release notes][2]  
[Aspose.Words for Android via Java 18.4 release notes  
](https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Android+via+Java+18.4+Release+Notes)  
[Aspose.Words for Android via Java 18.4][3] now allows you to perform following tasks:

*   [Open and Save Encrypted OpenDocument][4][](https://docs.aspose.com/display/wordsjava/Rendering#Rendering-EscapetheURIinOutputPDF)
*   [How to Add a Watermark in Table Cell][5]
*   [Verify Encrypted Document][6]

## Public Ref Class for out-ref Emulation Added in API

Related issue: WORDSJAVA-1756  
On .NET baseline, some public API methods contain out/ref params in signatures. Service classes Ref, RefInt, RefBoolean, etc. are added to emulate out/ref in Java. Now, the code like:

```
void SomeMethod(ref Document doc, out int i)

```

is autoported to Aspose.Words for Java as:

```
void someMethod(Ref doc, RefInt i)

```

The Ref\* classes contain get() and set() methods to get and set the value.

Here is a look at just a few of the biggest features and API changes in this month’s release.

*   Added public Ref<T> class for out/ref emulation in public API.
*   Provide an ability to work with password-protected ODT and OTT file formats
*   Preserve PaperTray information in PCL
*   Added ShapeBase.IsLayoutInCell property 
*   Implemented optimization of metafile rendering vector output. Optimization includes applying intermediate transformations directly to the graphics and removing redundant canvases. Such optimization is also performed by MW when saving metafiles as vector graphics to PDF, XPS, etc.
*   PaperTray information is now saved in PCL output
*   “DrawingML shapes are not fully supported” warning is not thrown anymore, more specific warnings are used instead while rendering
*   DrawingML shapes with auto-size and empty textboxes don’t throw exception while rendering now
*   WordArt objects with empty fill now cast only outline shadows while rendering. Previously the whole shape cast a shadow
*   Improved rendering of MathAccentElement. The accent symbol is rendered in accordance with the letter’s height
*   Improved rendering of PieChart, if data labels have a manual layout
*   Improved rendering of the text boxes with OleObjects (e.g. Math equation)
*   Improved rendering of WordArt objects with gradient fill
*   Fixed a bug causing the corruption of radial gradient fill for rotated shapes while rendering
*   Fixed rendering of “Monotype Hadassah” font with legacy encoding
*   Fixed a problem with META\_SETPIXEL WMF record while rendering meta-files
*   Improved frame width calculation when paragraph has right indent
*   Improved computation of widths of ideographic space when combined with document grid, space inside footnotes
*   Improved floating table positioning for RTL tables in 2013 compatibility mode
*   Improved layout of 2013 compatible documents when page break overlaps footer
*   Improved positioning of wrapped lines in 2013 compatibility mode, and lines with large inline images
*   Fixed issue with character compressing when Kinsoku rule is ignored by document
*   Fixed incorrect glyph selection for Zero Width No-Break Space when font does not have this glyph
*   Fixed comment range highlighting issue when comment spans multiple pages inside a repeated header row of a table
*   Fixed rendering of text in merged cells when row contains hidemark attribute on the cell break and all remaining cells are merged

'Aspose.Words for Android via Java' is an advanced Word document processing API to perform a wide range of document processing tasks directly within your native Android applications. Aspose.Words for Android via Java API supports DOC, OOXML, RTF, HTML, OpenDocument, PDF, XPS, EPUB and other formats. You can generate, modify, convert and render documents.  
[Learn more about Aspose.Words for Android via Java][7]

## Aspose.Words for Android via Java API Resources

Following are the links to some useful resources you may need to accomplish your tasks.

*   [Aspose.Words for Android via Java Online Documentation][8] ('Aspose.Words for Android via Java' is very similar to 'Aspose.Words for Java'. So, you can use the same documentation)
*   [Features][9]
*   [Limitations and API Differences][10]
*   [Product Page][11][](http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-words/)
*   [Install Aspose.Words for Android via Java from Maven][12]
*   [API Reference Guide][13] (Aspose.Words for Android via Java is very similar to Aspose.Words for Java. So, you can use the same API Reference Guide)
*   [Free Support Forum][14]
*   [Paid Support Helpdesk][15]
*   [GitHub Examples][16]

## Start a Free Trial Today

Start a free trial today – all you need is to [sign up with Aspose][17]. Once you have signed up, you are ready to try all the powerful file processing features offered by Aspose.

You can easily download 'Aspose.Words for Android via Java' API for evaluation. The evaluation download is the same as the purchased download. The evaluation version simply becomes licensed when you add a few lines of code to [apply the license][18].

The evaluation version of Aspose.Words for Android via Java (without a license specified) provides full product functionality, but it inserts an evaluation watermark at the top of the document on open and save, and limits the maximum document size to several hundred paragraphs.

If you want to test 'Aspose.Words for Android via Java' API without the evaluation version limitations, you can also request a 30-day Temporary License. Please refer to [How to get a Temporary License][19]?




[1]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Android+via+Java+API+Differences+and+Limitations
[2]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+18.4+Release+Notes
[3]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-words/18.4
[4]: https://docs.aspose.com/display/wordsjava/Saving+a+Document#SavingaDocument-OpenandSaveEncryptedOpenDocument
[5]: https://docs.aspose.com/display/wordsjava/Working+with+Watermark#WorkingwithWatermark-HowtoAddaWatermarkinTableCell
[6]: https://docs.aspose.com/display/wordsjava/Creating+or+Loading+a+Document#CreatingorLoadingaDocument-VerifyEncryptedDocument
[7]: https://products.aspose.com/words/android-java
[8]: https://docs.aspose.com/display/wordsjava/Home
[9]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Android+via+Java+Features
[10]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Android+via+Java+API+Differences+and+Limitations
[11]: https://products.aspose.com/words/android-java
[12]: https://docs.aspose.com/display/wordsjava/Installation#Installation-InstallAspose.WordsforAndroidviaJavafromMavenRepository
[13]: https://apireference.aspose.com/java/words
[14]: https://forum.aspose.com/c/words
[15]: https://helpdesk.aspose.com/
[16]: https://github.com/aspose-words/Aspose.Words-for-Java
[17]: https://www.aspose.com/
[18]: https://docs.aspose.com/display/wordsjava/Licensing
[19]: https://purchase.aspose.com/temporary-license




