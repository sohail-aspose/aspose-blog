---
title: 'Table Of Contents (TOC) Improvements in Aspose.Words 10.1'
date: Mon, 30 May 2011 09:37:20 +0000
draft: false
url: /2011/05/30/table-of-contents-toc-improvements-in-aspose.words-10.1/
author: DmitryV
summary: ''
tags: ['Work with Table of Content in Word', 'Work with ToC in Word']
categories: ['Aspose.Total Product Family']
---

Just wanted to supplement the [Aspose.Words for .NET and Java 10.1 announcement][1] with some details about Table of Contents (TOC) update. The announcement states the release includes about 20 TOC fixes, let me tell you what the most noticeable categories are:

*   **Performance fixes.** There was a performance decrease since version 9.6 reported by our users. It is no longer there, yet there is a field for further improvements.
*   **Appearance fixes.** Aspose.Words used to construct some complex TOCs with certain issues, which particularly had to do with TOC entry labels and following text appeared too close to each other. It is fixed now.
*   **Behavior fixes.** Some field switches caused TOC to behave differently than MS Word did. Most of such issues are now resolved.
*   **Crash fixes.** We have eliminated all reported exceptions used to occur when updating a TOC.
*   **Miscellaneous fixes.** There was a bunch of user-specific fixes related to rare or minor issues. Fixed now.

We keep working on the TOC update feature extensively because it is probably the most sophisticated MS Word field and there are more fixes to resolve as well as features to implement. Stay tuned! Oh, nearly forgot: if you call **Document.UpdatePageLayout()** after **Document.UpdateFields()** just to update TOC (that was a must in first versions of TOC update) – get rid of the **Document.UpdatePageLayout()** call. All the work is done in **Document.UpdateFields()** including the update of layout.



{{< figure align=center src="images/TOC.png" alt="Table Of Contents by Aspose.Words">}}


Here are the Aspose.Words for .NET and Java 10.1 download links:

*   [https://downloads.aspose.com/words/net][2]
*   [https://downloads.aspose.com/words/java][3]




[1]: https://blog.aspose.com/2011/05/29/aspose.words-10.1-delivers-101-issues-resolved-2/
[2]: https://downloads.aspose.com/words/net
[3]: https://downloads.aspose.com/words/java




