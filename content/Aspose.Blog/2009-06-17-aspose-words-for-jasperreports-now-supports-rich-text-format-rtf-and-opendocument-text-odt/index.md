---
title: 'Aspose.Words for JasperReports Now Supports Rich Text Format (RTF) and OpenDocument Text (ODT)!'
date: Wed, 17 Jun 2009 01:05:00 +0000
draft: false
url: /2009/06/17/aspose-words-for-jasperreports-now-supports-rich-text-format-rtf-and-opendocument-text-odt/
author: DmitryV
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

We proudly announce a new release of Aspose.Words for JasperReports. In this release, you will find that a number of exciting features have been added.

First off, apart from DOC, DOCX, TXT and HTML, the product now supports two additional formats - Rich Text Format (RTF) and OpenDocument Text (ODT)!

Secondly, lines and rectangles are now exported along with other report elements. Note however that they are disabled by default because the way some JasperReports are currently designed may lead to corrupted document layout. Consider enabling this feature by setting the _EXPORT\_LINES_ and _EXPORT\_RECTANGLES_ parameters to true. Switch them back to false (one of them or both) if the document layout becomes corrupted - this basically means that you should redesign the report or accept the document without lines or rectangles exported.

Thirdly, this release introduces the _SPACING\_FACTOR_ parameter. This parameters allows you to decrease spacing between report elements when being set to a value less than 1.0 (which is default). If you notice that page breaks in your document are being pushed to subsequent pages, thus leading to excessive blank pages to appear, try setting the parameter to a smaller value, say 0.9 or 0.75. This will "shrink" spacing and make page contents more compact. Keep on until the report looks as expected.

To download, please visit [http://www.aspose.com/community/files/67/jasperreports-exporters/aspose.words-for-jasperreports/default.aspx][1]




[1]: http://www.aspose.com/community/files/67/jasperreports-exporters/aspose.words-for-jasperreports/default.aspx




