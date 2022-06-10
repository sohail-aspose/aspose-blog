---
title: 'Rendering is Coming'
date: Tue, 25 Nov 2008 00:18:00 +0000
draft: false
url: /2008/11/25/rendering-is-coming/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

I have earlier mentioned that today, 24th Nov, we will make available an Aspose.Words for .NET release that includes the "final beta" of the new rendering engine. Yes, the one for rendering document pages to images, printing on a server and direct to PDF conversion.

There's been a late minute change to simplify the new public API and it is going to delay the release by 2-3 days.

As a teaser, I can tell you how the new API is going to look like. Most of the new use cases will take only a single line of code to write.

**Easy save with default options to PDF directly (without using Aspose.Pdf):**

document.Save("myFile.pdf");

**Easy save to a multipage TIFF file directly:**

document.Save("myFile.tiff");

**Save to PDF a range of pages, specify options:**

Document.SaveToPdf(int pageIndex, int pageCount, string fileName, SaveToPdfOptions options)

Document.SaveToPdf(int pageIndex, int pageCount, Stream stream, SaveToPdfOptions options)

**Save to PNG, JPEG, EMF, BMP (one page) or TIFF (one or more pages), specify options:**

Document.SaveToImage(int pageIndex, int pageCount, string fileName, SaveToImageOptions options)

Document.SaveToImage(int pageIndex, int pageCount, Stream stream, SaveToImageOptions options)

**Render a page to a .NET Graphics object to a specified zoom factor:**

Document.RenderToScale(int pageIndex, Graphics graphics, float x, float y, float scale)

**Render a page to a .NET Graphics object to a specified size:**

Document.RenderToSize(int pageIndex, Graphics graphics, float x, float y, float widht, float height)

**Easy print:**

Document.Print(string printerName)

Document.Print(PrinterSettings printerSettings)








