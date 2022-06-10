---
title: 'PDF Rendering of WordArt MathAccentElement PieChart Ole Objects in SharePoint'
date: Wed, 02 May 2018 06:32:04 +0000
draft: false
url: /2018/05/02/aspose.words-for-sharepoint-18.4-released/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose-Words-for-SharePoint-e1399452535590.png" alt="PDF rendering in SharePoint">}}


We are really delighted to announce the release of version 18.4 of the Aspose.Words for SharePoint API. This release comes with some very exciting features to enhance the usability of the API. This version also sees the codebase better tweaked and the core functionality closer to Aspose.Words for .NET 18.4, which is the base product that **Aspose.Words for SharePoint 18.4** is ported from.  
We recommend you to download the latest release and check out all the features introduced in the base Aspose.Words for .NET API. You can download the latest release of Aspose.Words for SharePoint from the following link:

*   [Download Aspose.Words for SharePoint 18.4 now][1]

## Bug Fixes and Changes

Aspose.Words for SharePoint 18.4 release includes the latest improvements and fixes made up to date in Aspose.Words for .NET (18.4). The most notable are:

*   Preserve PaperTray information in PCL    
*   Implemented optimization of metafile rendering vector output. Optimization includes applying intermediate transformations directly to the graphics and removing redundant canvases. Such optimization is also performed by MS Word when saving metafiles as vector graphics to PDF, XPS, etc.
*   PaperTray information is now saved in PCL output
*   DrawingML shapes with auto-size and empty textboxes don't throw exception while rendering now
*   WordArt objects with empty fill now cast only outline shadows while rendering. Previously the whole shape cast a shadow
*   Improved rendering of MathAccentElement. The accent symbol is rendered in accordance with the letter's height
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

## Aspose.Words for SharePoint API Resources:

Following are the links to some useful resources you may need to accomplish your tasks.

*   [Aspose.Words for SharePoint 18.4 release notes][2]
*   [Aspose.Words for .NET release notes][3]
*   [Aspose.Words for SharePoint Online Documentation][4][](https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Android+via+Java+API+Differences+and+Limitations)
*   [Aspose.Words for SharePoint Product Page][5]
*   [Download Aspose.Words for SharePoint][6][](https://docs.aspose.com/display/wordsjava/Installation#Installation-InstallAspose.WordsforAndroidviaJavafromMavenRepository)
*   [Aspose.Words Forum][7][](https://github.com/aspose-words/Aspose.Words-for-Java)

## Start a Free Trial Today

Start a free trial today – all you need is to [sign up with Aspose][8]. Once you have signed up, you are ready to try all the powerful file processing features offered by Aspose.

You can easily download 'Aspose.Words for SharePoint' API for evaluation. The evaluation download is the same as the purchased download. Please check [How to License Aspose.Words for SharePoint][9].

The evaluation version of Aspose.Words for SharePoint (without a license specified) provides full product functionality, but it inserts an [evaluation watermark][10] at the top of the document on open and save, and limits the maximum document size to several hundred paragraphs.

If you want to test 'Aspose.Words for SharePoint' API without the evaluation version limitations, you can also request a 30-day Temporary License. Please refer to [How to get a Temporary License][11]?




[1]: https://downloads.aspose.com/words/sharepoint/new-releases/aspose.words-for-sharepoint-18.4/
[2]: https://docs.aspose.com/display/wordssharepoint/Aspose.Words+for+SharePoint+18.4+Release+Notes
[3]: https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET
[4]: https://docs.aspose.com/display/wordssharepoint
[5]: https://products.aspose.com/words/sharepoint
[6]: https://downloads.aspose.com/words/sharepoint
[7]: https://forum.aspose.com/c/words
[8]: https://www.aspose.com/
[9]: https://docs.aspose.com/display/wordssharepoint/License+Aspose.Words+for+SharePoint
[10]: https://docs.aspose.com/display/wordssharepoint/Evaluate+Aspose.Words+for+SharePoint
[11]: https://purchase.aspose.com/temporary-license




