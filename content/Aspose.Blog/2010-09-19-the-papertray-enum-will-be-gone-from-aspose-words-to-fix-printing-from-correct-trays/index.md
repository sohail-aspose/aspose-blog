---
title: 'The PaperTray enum will be gone from Aspose.Words.'
date: Sun, 19 Sep 2010 15:56:00 +0000
draft: false
url: /2010/09/19/the-papertray-enum-will-be-gone-from-aspose-words-to-fix-printing-from-correct-trays/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Microsoft Word allows specifying different paper trays in a document for each section, for the first and all further pages of each section.

We have corresponding Aspose.Words.PaperTray enum, which is used by the Section.PageSetup.FirstPageTray and OtherPagesTray properties. The PaperTray enum has values like AutomaticSheetFeed, LargeFormatBin, ManualFeed and so on.

We thought we had it working! We thought we tested printing a document using Aspose.Words will take paper from the correct trays as specified in the document. Our AsposeWordsPrintDocument class that performs printing converted our PaperTray enum into System.Drawing.Printing.PaperSource class.

But several customers reported that Aspose.Words does not seem to obey the paper tray specified in the document.

We have studied MS Word's behavior and reviewed (the now more up-to-date) document format specifications and found that... the paper tray value stored in Word documents is completely **implementation specific**. The value seems to be completely **printer specific**.

If you create a document in Microsoft Word and set paper tray values, the values stored in the document will be for the currently selected (or default maybe) printer. For example, the value of 292 will be stored inside the Word document.

Then, when you take this document to another computer that has a different printer installed and try to print it (or just check in Page Setup to see what paper tray is selected), you will observe that the paper tray is not preserved! It is reset to a default value.

What this all means is that you can only expect the paper tray to be correctly handled by Microsoft Word when printing on the same printer model as the one that was selected when the paper trays were selected.

There are no "universal" or "well known" values for paper trays stored in Word documents and hence we cannot have a meaningful PaperTray enumeration in Aspose.Words.

To fix the problem and print to the correct paper trays we have removed the PaperTray enum from Aspose.Words and changed PageSetup.FirstPageTray and OtherPagesTray to simple integers.

So in the next version of Aspose.Words, if you print your document on the same printer model which was selected when the document was created, it will print using the correct trays. If you print on another printer - a wrong (the default) tray for the printer might be selected. Unfortunately this behavior is by Microsoft Word's design and we cannot improve it.








