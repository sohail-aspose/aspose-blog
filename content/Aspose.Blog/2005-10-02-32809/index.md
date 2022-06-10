---
title: 'About Embedded True Type Fonts in Word Documents'
date: Sun, 02 Oct 2005 04:47:00 +0000
draft: false
url: /2005/10/02/32809/
author: Romank
summary: ''
tags: ['Roman Korchagin']
---

There've been several requests from the customers for Aspose.Word to support processing of Word documents with embedded true type fonts. I've looked into the issue and there are actually two feature requests around embedded fonts:

1.  Be able to embed fonts in Word documents.
2.  Be able to process (open, modify and save) Word documents with embedded fonts already there.

It looks like True Type fonts are embedded in Word files using some Agfa MicroType Express compression technology. Apparently this compression technology must be licensed from Agfa in order to be able to embed True Type font files like MS Word does. I have no idea what and how much it takes to license it and I will investigate, but my guess for now is Aspose is not ready for this yet. Looks like only some big names Microsoft, Samsung, Adobe have licensed this technology so far. An interesting hack I will probably attempt is to embed True Type fonts without using MicroType Express compression, maybe MS Word will still recognize the font file.

Even if Aspose.Word will never be able to embed True Type fonts - not everything is lost. Just making Aspose.Word to preserve existing embedded fonts in the documents (I hope I don't need the license for that) will satisfy many customers. Basically you will design your report in MS Word, request it to embed the fonts in it without subsetting and use Aspose.Word to process the document to populate it with data. The document produced by Aspose.Word will keep the embedded fonts and can be delivered to the end users. This must be the case to satisfy 80% of the needs.

Interesting to note that current WordprocessingML does not support embedding True Type fonts. It looks like in MS Office 12 this XML format will be the default document format with a few optimizations like storing binary data in separate files, so they will probably support embedding True Type fonts then.

RTF supports font embedding, but I was not able to get MS Word to produce and RTF file with an embedded True Type font. I set the options in MS Word to embed fonts and save a document as RTF but it is very small size and does not have any embedded fonts in it. Anyone has an RTF file with an embedded font for me as a sample please?

OpenOffice 1.1 that I play with does not support font embedding, but I've seen they want to add this feature in the future. If they are to produce Word files with embedded fonts, they will face the same issue of licensing the compression technology.







