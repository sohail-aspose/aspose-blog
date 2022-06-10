---
title: 'RTF and Culture'
date: Mon, 16 Jul 2007 01:26:00 +0000
draft: false
url: /2007/07/16/rtf-and-culture/
author: Romank
summary: ''
tags: ['Roman Korchagin']
---

From what I can tell RTF and Culture do not mix.

If you have English culture selected in your regional settings, create a document in Microsoft Word and save as RTF, then double values (in custom document properties) will be written as 123.45. When you open this document in Microsoft Word it seems to use the current culture. So if you culture is English, the document will load okay.

If you happen to have Russian culture and save the document as RTF, the numbers will be written as 123,45. This is because the Russian culture usues comma as a decimal separator. Again, if you open this document in Microsoft Word while using Russian culture, there will be no problems.

However, if you try to open an RTF document with 123.45 in Microsoft Word on a computer with Russian culture, or try to open a document with 123,45 in Microsoft Word on a computer with English culture - the value will be imported incorrectly. In one case I got it as 12345.

Note that there is no indication inside the RTF file as to which culture was used when writing the file.

My conclusion - there is no way out in this case. This bug seems to have survived in RTF and in Microsoft Word for over 20 years?







