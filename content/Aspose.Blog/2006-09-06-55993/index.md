---
title: 'AWesome!'
date: Wed, 06 Sep 2006 00:16:00 +0000
draft: false
url: /2006/09/06/55993/
author: DmitryV
summary: ''
tags: ['Dmitry Vorobyev']
---

So we have almost finished another major release of Aspose.Words. We're happy to note how greatly the component evolves and improves despite it's still pretty young by the standards of software industry. It's less than 3 years old but it's already the subject to imitate

Among other cool features, two highly requested formats have been added to the component's arsenal, Rich Text Format (RTF) and WordprocessingML (WordML). One of the areas I'm responsible for is RTF export (will start working on import once we release 4.0 final version) so if you are curious, I will share some interesting facts related to that.

Let me make some numbers public first. RTF 1.8 includes over 1400 keywords (called control words), and Aspose.Words now supports almost all of those required for proper representation of any Microsoft Word documents regardless of their complexity. The only exceptions are:

*   Table styles
*   Formatting revisions
*   Comment ranges

All of these will be supported very soon.

At the moment we process around 95% of the keywords. That wasn't so easy mainly because RTF is a very ambiguous format. That is some keywords or their values just do not obey the rules declared in the format specification (which is also pretty ambiguous, but that's a separate story ). Another difficulty was the inconsistency that was showing itself throughout the format. As a result, the code of the exporter is full of comments specifying that some keyword behaves differently from what is stated in the spec, or may include an undocumented value, or is not mentioned in the spec at all.

Basically, RTF looks like the first attempt of migrating from binary to textual representation of documents. Yes, RTF **is** a textual format but it's hardly supposed to be read by a user  It's impossible to understand what **\\tsbrdrdgr** or **\\lyttblrtgr** mean having no description, isn't it? That wouldn't be a problem, though, if the spec was strict and legible and described each and every keyword Microsoft Word may produce. Unfortunately, I couldn't rely on the format documentation only and had to verify most of the keywords to ensure we produced documents looking exactly similar to the Microsoft Word's output.

Now I'm happy to state that all the problems are solved and the documents we're producing are identical to those created by Microsoft Word. Even their internal representation (I mean RTF stream itself) resembles Microsoft Word; for example, we satisfy old readers as RTF spec dictates (although we didn't test readers older than Microsoft Word 97).

That doesn't mean we blindly mimicked Microsoft Word. For instance, we have a test document containing several ClipArt shapes that when saved as RTF and opened again in Microsoft Word, crashes it. However, Microsoft Word perfectly opens this document when it is exported to RTF by Aspose.Words

Anyway, Microsoft Word is still exemplary for us because we're working with its "native" formats and our goal is getting rid of any differences between the appearances of our documents. I think we've succeeded in it. The accuracy we've achieved is the reason why we call our export High-Fidelity, or Hi-Fi, in case you were wondering. We spend a lot of effort in details. Here's an example. Microsoft Word has no UI elements that allow setting up such line properties as joining style or miter limit. However, these are present among the shape attributes and it's enough to us to be supporting them in RTF and other formats. We just do not ignore minor things even though they are used pretty seldom - who knows, maybe some of your documents will contain those attributes.

If nevertheless you find anything you treat as inaccuracy when exporting to any of the supported formats, welcome to the Support Forums. Many improvements of the product are reaction to your requests, and we are in extreme need of your participation in the development process. We hope recently launched Aspose MVP program shows that well. Together we will make it Hi-End!






