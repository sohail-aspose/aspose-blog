---
title: 'Word Cleaner developed DOC Converter Pro offering Batch Conversion of Microsoft Word Files to HTML'
date: Tue, 08 Mar 2011 19:52:18 +0000
draft: false
url: /2011/03/08/batch-conversion-of-microsoft-word-files-to-html-within-the-software-using-apis/
author: Brian O Neill
summary: ''
tags: ['Aspose.Words', 'Aspose.Words supports DOC to HTML conversion', 'DOC to HTML conversion', 'Flawless MS Word to HTML conversion feature', 'Insert Table Of Contents inside Word file', 'Manipulate Footnotes and Endnotes in Word file', 'Success Stories']
categories: ['Aspose.Words Product Family']
---

## About Word Cleaner



{{< figure align=center src="images/Docconvert-logo-1.png" alt="">}}


[Word Cleaner][1] (_now Doc Converter_) is a shareware program that batch converts Microsoft Word files to HTML and during conversion, it cleans up the code. In previous versions, we relied on linking into Word to do the conversion, and then we used to execute a special clean up routines on the code. Then we started looking to use [Aspose.Words for Java][2] in a subsequent version of Word Cleaner, specifically to use the conversion from Word files to HTML format.

## Problem

It is very common for users to write content for web pages in Microsoft Word, but the problems occur when users try to convert these files to HTML. We encountered follow two major issues:

*   Word has a "save as HTML" function, but the HTML produced contains a massive amount of unnecessary Word-specific code. This makes the code very messy, and dramatically increases the size of the HTML files.
*   Users try to copy and paste from Word into a CMS. The problem here is that very often the Word-specific HTML is also pasted. It causes unnecessary complex code and increased storage space in the CMS.

Another problem with Word Automation that we faced was that the users need to have Word installed on their machines. Even if they had MS Word, there were sometimes issues regarding its linking.

As an example, if you open up a new Word file and enter sample text like "This is a test", then go to File and Save as HTML you will find that the HTML file contains 436 lines of code, and the file size is 21kb. However when the same file is converted using [Aspose.Words for Java][3], the HTML file has only 14 lines of code and the file size is less than 1k. This is over a 95% reduction in size!

You may clearly notice that [Aspose.Words for Java][4] dramatically reduces the size of converted HTML and also the HTML is better formatted and structured.

## Solution

We evaluated [Aspose.Words for Java][5] for several reasons:

*   It is a standalone product that does not require the user to have Microsoft Word installed.
*   It produces very [clean HTML when converted from Word files][6]. It also supports advanced features like tables of contents, [footnotes][7], etc.
*   It works really well on servers
*   It can work on Mac OSX, and we are looking into using it with the Mono framework. A Mac version is one of our top user requests so we planned to use [Aspose.Words for Java][8], so that we can create a Mac version.



{{< figure align=center src="images/word-cleaner-case-study-aspose-words.png" alt="Word Cleaner main screen preview" caption="Image 1:- The word cleaner main screen">}}




{{< figure align=center src="images/word-cleaner-case-study-aspose-words-1.png" alt="Word to HTML conversion preview" caption="Image 2:- Built-in editors let you view the converted HTML.">}}


## Experience

We liked the fact that you could download a fully functional [free trial][9] of [Aspose.Words for Java][10] and it enabled us to create a demo app to test its capabilities.

We also liked the [support forum][11] and found a massive amount of information there. We posted a few requests in the [forum][12] and found that we got very prompt and helpful replies from the support staff.

## Implementation

Switching to [Aspose.Words for Java][13] took about a week to change over the code, and so far we have been very happy with the results and have had no real issues reported.

## Outcome

To date, we have been extremely satisfied with the results. We are due to go live with the new version of our software next month and anticipate that while using [Aspose.Words for Java][14], our customers will clearly see the benefits of the new version.

## Next Steps

We are interested in looking at other [Aspose products][15] like [Aspose.Cells][16]. We are very impressed with the flexibility of the [Aspose][17] range, particularly the ability to run them on server environments and the ability to run them with the mono framework.

## Conclusion

Generally, we are very happy working with [Aspose.Words for Java][18] and were impressed by the way the product is continually updated with regular new releases. We found the [documentation][19] clear, the [support][20] very helpful and we have no hesitation at all in recommending [Aspose.Words for Java][21] to other developers.




[1]: https://wordcleaner.com/
[2]: https://products.aspose.com/words/java
[3]: https://products.aspose.com/words/java
[4]: https://products.aspose.com/words/java
[5]: https://products.aspose.com/words/java
[6]: https://docs.aspose.com/display/wordsjava/Saving+a+Document#SavingaDocument-SpecifyingHTMLSaveOptions
[7]: https://docs.aspose.com/display/wordsjava/Working+with+Document#WorkingwithDocument-WorkingwithFootnoteandEndnote
[8]: https://products.aspose.com/words/java
[9]: https://downloads.aspose.com/words/java
[10]: https://products.aspose.com/words/java
[11]: https://forum.aspose.com/c/words
[12]: https://forum.aspose.com/c/words
[13]: https://products.aspose.com/words/java
[14]: https://products.aspose.com/words/java
[15]: https://products.aspose.com/
[16]: https://products.aspose.com/cells
[17]: https://www.aspose.com/
[18]: https://products.aspose.com/words/java
[19]: https://docs.aspose.com/display/wordsjava/Getting+Started
[20]: https://forum.aspose.com/c/words
[21]: https://products.aspose.com/words/java




