---
title: 'Bad Looking Metafiles'
date: Mon, 06 Feb 2006 08:50:00 +0000
draft: false
url: /2006/02/06/41099/
author: DmitryV
summary: ''
tags: ['Dmitry Vorobyev']
---

.NET Framework is surely very powerful but some things are just weird. Goodness knows why Microsoft decided to implement rendering metafiles (such as WMFs and EMFs) and converting them to bitmaps using no smoothing thus eliminating all benefits of vector graphics. They could at least provide some option to choose whether or not to use anti-aliasing but they didn't do that. Applications including MS Word do render metafiles properly but you will get ugly output trying to render them using **System.Drawing.Graphics**, especially if your metafile image contains small details or text.

Now to get applicable quality of metafiles drawing, one needs to implement self-made logic which plays metafile records with anti-aliasing turned on. It's a pretty annoying work since (afaik) EmfPlusRecordType is the largest enumeration in .NET. It appears to be the only solution though.







