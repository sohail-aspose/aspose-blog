---
title: 'Aspose.Pdf.Kit for Java Release 1.8.0.0 Published!'
date: Wed, 09 May 2007 22:14:00 +0000
draft: false
url: /2007/05/09/75843/
author: Forever
summary: ''
tags: []
categories: ['Aspose.PDF Product Family']
---

Features added or improved:

1\. Filling XFA fields in PDF templates created by Adobe 7 and 8 is fully supported without losing any action or script information.

 1) User can fill XFA fields in PDF templates by Adobe 7 and 8 without losing any action or scripts.

 2) Form.allFlatten() and Form.partialFlatten() are both enabled for XFA forms.

 3) Form.FillImageField() can be applied to Image Field to support image pasting in both Adobe 7 and 8.

 4) Support for XFA in FormEditor.SetSubmitUrl() is provided.

 5) Form.exportXml()/Form.importXml() have been upgraded for XFA supporting. Data in PDF documents by Adobe Designer 7 & 8 can be fully exported to a leveled XML file.

2\. Editing the content of PDF file is improved:

 1) Extracting bookmark information is provided by Class PdfContentEditor. You can extract bookmark information such as title, level, destination page number or action destination.

 2) Bookmark’s title has been modified according to specified title by Class PdfContentEditor.

 3) Creating Polygon, PolyLine and curve is provided by Class PdfContentEditor. You can draw polygon in existing pdf documents.

 4) Extracting the information of all links in the pdf document is provided by Class PdfContentEditor, you can extract the link information such as source page number，destination page number，link action type，destination file name，destination page View Type，link visibility，link color，link rectangle，link URI.

Bugs fixed:

1) Reading PDF files error when the startref tag at the end of PDF file. Please refer to: http://www.aspose.com/Community/forums/thread/66822.aspx

2) Some operations such as makeNUp and changePageSize cause 'a file was broken' error when setting license. Please refer to: http://www.aspose.com/Community/forums/thread/72235.aspx








