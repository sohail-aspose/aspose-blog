---
title: 'Performance Test of Large File'
date: Sat, 16 Sep 2006 12:15:00 +0000
draft: false
url: /2006/09/16/56872/
author: Romank
summary: ''
tags: ['Roman Korchagin']
---

Just wanted to share results of one of the performance tests we do right now before finalizing Aspose.Words 4.0. We think the results are very good, hence we want to share them. The test is for a quite LARGE file, so it is pretty much a stress test if you like. Most of the files you will process with Aspose.Words are likely to be smaller and process much faster.

**Test Setup**

*   Test file: Word2003RTFSpec.doc, **size 4.78mb**, **212 pages**, 390,000 characters, 12,860 paragraphs.
*   Test machine: P4 3.0Ghz, 2Gb RAM, SATA RAID0.

**Test Results**

*   Open test document (load into Aspose.Words.Document object): **1.4 seconds**.
*   Save test document in DOC format: **1.2 seconds**.
*   Save test document in WordML format: **1.7 seconds**.
*   Save test document in RTF format: **3.0 seconds**.

The time shown is the minimal time taken over several runs. All other software I tested takes 5 seconds or more for the same operations.







