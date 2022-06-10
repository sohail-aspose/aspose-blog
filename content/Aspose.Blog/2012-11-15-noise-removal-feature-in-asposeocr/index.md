---
title: 'Noise Removal Filters and Second Guess a Symbol in OCR using C#'
date: Thu, 15 Nov 2012 07:09:29 +0000
draft: false
url: /2012/11/15/noise-removal-feature-in-asposeocr/
author: Tilal Ahmad
summary: ''
tags: ['.NET', 'Aspose.OCR', 'Noise Removal Filters', 'OCR', 'Second guess of recognized symbol', 'product release']
categories: ['Aspose.OCR Product Family']
---



{{< figure align=center src="images/aspose-OCR-for-net_100.png" alt="">}}


We are pleased to announce the release of [Aspose.OCR for .NET][1] 1.3.0. In this release, we have introduced two new features. Firstly,  noise removal filters are included in the public API. Now you can process images with these filters before running recognition.  This helps improve text recognition accuracy.

Secondly, we've added a feature for exposing a second possible guess for a symbol. The following code snippet shows how the second guess properties work.

```
OcrEngine ocr = new OcrEngine();
//ocr.Config.
ocr.Config.UseDefaultDictionaries = true;
/**
int ocrEngine.Config.ProbabilityRow - defines how to return text with symbols, e.g.
if it set to 1 - we will return second possible guess,
if it is 2 - we will return third possible guess and so on. Default value is 0.
**/
ocr.Config.ProbabilityRow = 1;
….
….
//string ocrEngine.ProbabilitySymbols contains these results. By default it is empty.
Console.WriteLine("Text ProbabilitySymbols: " + ocr.ProbabilitySymbols);
```

Please visit the following link for further details on what’s new in [Aspose.OCR for .NET 1.3.0][2].




[1]: https://products.aspose.com/ocr/net
[2]: https://products.aspose.com/ocr/net




