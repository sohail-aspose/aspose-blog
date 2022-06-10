---
title: 'The Rendering Fidelity of Footnotes'
date: Thu, 08 Apr 2010 21:43:00 +0000
draft: false
url: /2010/04/08/the-rendering-fidelity-of-footnotes/
author: Mf
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

_This article is a technical blurb mostly about why it is taking so long for us to support footnotes and endnotes in Aspose.Words when rendering documents to PDF, XPS or printing. This post looks at how Microsoft Word handles some tricky layouts and even reveals some obscure flaws. It might be interesting to Aspose.Words customers who are waiting for footnotes to be supported or to any other developer whomever pondered about document layout._

As you might know one of the goals of the Aspose.Words layout engine is to produce result as close to Microsoft Word as possible. Being in charge of this piece of Aspose.Words I personally spend a lot of time figuring out how Microsoft Word formats a document into pages. Footnotes are hot for us because many customers are waiting for this feature, so I’ve decided to share some thoughts in this post. Hopefully if there are curious readers out there I’ll post regularly.

# What We’ve Done so Far

Aspose.Words for .NET 9.0 supports rendering of footnotes to some extent. Some simple documents might render acceptable. We decided it is better to release now because some footnotes is better than no footnotes at all.

Some of the limitations are:

· Only footnotes are rendered. Endnotes are not rendered.

· Footnotes are rendered immediately below text (not at the bottom of the page)

· Wrapping of long footnotes to next page is not supported. The text of the footnote could be truncated.

· Occassionally the text of the footnote will not appear.

More complete support is coming in the next version, estimated May 2010.

# Magic footnotes

I believe everybody knows what footnotes and endnotes are in Microsoft Word documents so I’ll not disscuss it here, however there are a few things I need to mention:

· Footnote or endnote consists of two parts. One part is a reference mark in the main text story of the document. The other part is the content of the footnote or endnote which is typically rendered at the bottom of the page or at the end of the document.

· References are continuously numbered, but can use custom marks or skip numbers.

· There are also three types of delimeters used to separate main text from the footnote/endnote text. They are separator, continuation separator and continuation notice.

· Footnote/endnote text can wrap from one column to another and can occupy one or more pages at the end of a section.

· There are two types of locations for footnote text and two types for endnote text.

· Footnote/endnote numbering and location can be specified per section in a document.

When I was starting to analyze this feature I knew that implementation challenge wouldn’t be technical but rather logical. The layout model of the document (it was adapted from Aspose.Editor before it was discontinued) already provides more functionality than required by Aspose.Words rendering. It already keeps track of all stories in the document but until recently footnotes story was ignored.

With this kind of attitude I was hoping to prototype Aspose.Words code in a few hours. I started to create small, but tricky test documents in Microsoft Word and tried to push its layout engine into a corner and that’s where the “magic” begun.

# Magic 1: Non-trivial ordering of footnotes

As you can see on the first screenshot, while table fits into one page footnotes flow according to the logical order of the references in the main text story, from 1 to 9. The second screenshot has same numbers for references but content is now ordered differently. There is no error and “yes” there are two “5” footnotes. This is how Word 2007 renders this case (I’m not surprised though). Let’s ignore the bug for now but focus on the ordering issue.

Technically, a footnote story can be represented as a linked list of runs, that is “1 One¶2 Two¶…9 Nine¶”. In Microsoft Word you can move caret from one footnote to another and using VBA you can query current position in the story which returns increasing integer. Word’s layout engine uses this order to pick a next portion of content to be flowed into a geometrical container. However, as we’ve seen this no longer works for footnotes since “seven” is rendered after “nine”.

# Magic 2: Column Balancing with Footnotes

The second thing is balancing of text columns. If a section ends with a “section break continuous” break and it has two or more columns then the content will be balanced between last group of columns of this section to minimize height of this group. Microsoft Word will include the height of the footnotes/endnotes into the column and balancing shall account for it.

Right, a bug again. Endnote “C” is overlapped by content of a second section on the page. Ignore the bug for now, but still the issue is that the column was designed to aggregate main text story content, however, as we’ve seen content of footnote/endnote stories is also flowed into it and balancing must handle this properly.

# Magic 3: Wrapping to Next Page

Third and last for this post is picking the right positions to wrap footnote and main text content. My initial thoughts were that Microsoft Word flows main text story content and footnotes in parallel. I thought that it attempts to flow footnote content as soon as a reference is flowed into the column. However the next example made me anxious.

If my idea was correct, then Microsoft Word would flow both 1st and 2nd footnotes right after first two lines of the main text story are flowed into the column, which means that 2nd footnote would fit on the first page completely and last two lines of the paragraph would be wrapped to the next column. However this doesn’t happen. Do you know why? Now I do.

You need to take paragraph rules into account. They are working in both main text and footnote text. There are also rules which try to keep the reference and content on the same page, rules about sharing of page by footnotes and endnotes, separator overflows, and hopefully you’ll get an idea of why it takes so long to implement layout of footnotes/endnotes the way Microsoft Word does it.

If you have something to say I’d be more than glad to hear it.

\- Michael








