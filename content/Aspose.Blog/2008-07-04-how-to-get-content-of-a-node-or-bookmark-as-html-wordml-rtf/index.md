---
title: 'How to get content of a node or bookmark as HTML, WordML, RTF?'
date: Fri, 04 Jul 2008 14:47:00 +0000
draft: false
url: /2008/07/04/how-to-get-content-of-a-node-or-bookmark-as-html-wordml-rtf/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

**How to get content of a node or bookmark as HTML, WordML, RTF?**  

Many customers of Aspose.Words ask this question, but so far there was no simple one-line-of-code way of doing that in Aspose.Words.  

The general solution we recommended so far was to "extract" the document fragment you are interested in into a separate Document object and then use Document.Save to save it in the desired format. Extracting the fragment might be done either by deleting all content from the document except the fragment you are interested in, or by copying the fragment into an empty Document instance. Because the Document is a tree of nodes, extracting a fragment is not always straightforward and requires a bit of coding with traversing nodes.  

We would like to change that and make it easy for you. The reason we have not yet done this is "complex consequences" that are not immediately apparent to the users who ask for this feature, but are very apparent to us when we try to think of implementing this feature.  

This post is to let you, the user who asks for this feature see the "consequences" of this feature and seek your feedback. Once we decide how to proceed, we will quickly implement extracting HTML, WordML, RTF and any other format from nodes, bookmarks and any other document fragments.  
  

**Where Should the Images Go?**  

You want to obtain contents of a node or bookmark as an HTML string. All you want to do is:  

string htmlString = doc.Range.Bookmarks\["MyBookmark"\].ToHtml();  

It is often forgotten that the fragment could contain images. When a complete document is saved to HTML, the images are written as separate files and the output HTML file references them.  

However, what to do with images when extracting only a fragment of a document as HTML? Should we just ignore the images in this case?  
  

**What's an RTF Fragment?**  

It is easy to say "I want RTF of that paragraph", but the problem is that any RTF fragment (or WordML or OOXML for that matter) is only valid within the context of a particular document.  

There are several document-wide structures that every fragment will often refer to. For example, an RTF fragment will use \\f0 etc keywords to refer to entries in the font table. That is if you don't carry an RTF font table along with that RTF paragraph then the "references" to fonts will be dangling and you will never find out what font is used by text of the RTF fragment.  

This situation is not limited to fonts and RTF, it is much more widespread. Other document-wide structures that are often referenced are styles and list (numbering) and this affects not only RTF, but WordML and OOXML.  

In WordML there is a thing called "context free chunk" that could be used to solve the problem.  A context free chunk is basically a "mini document" that includes all the document-wide-structures that are referenced by that particular document fragment. Brian Jones gives a bit of info about context free chunks here : [http://blogs.msdn.com/brian\_jones/archive/2005/07/20/441167.aspx][1]  

What do you think if we make Node.ToWordML() to return XML in the context free chunk format? I am not so sure about RTF and OOXML though. For RTF we will probably have to return a complete "mini document". For OOXML... no ideas so far.  
  

**Jagged Fragments**  

A bookmark in a Word document can start in a paragraph outside of a table, but end inside a table. The document is a tree of nodes and the situation looks something like this:  

<bmkStart name="MyBookmark/>  

<table>  
<tr>  
<tc><bmkEnd name="MyBookmark"/></tc>  
</tr>  
</table>  

If you want to get content of MyBookmark as HTML or WordML you are looking at several "jagged" nodes. That is start of table, row and cell elements are inside the bookmark, but they end outside of it. How do you want that exported?  

A possible solution is to "snap" up or down until the jagged fragment is closed. It could be possible to snap so the whole table is included in the bookmark or excluded. What do you think?




[1]: http://blogs.msdn.com/brian_jones/archive/2005/07/20/441167.aspx




