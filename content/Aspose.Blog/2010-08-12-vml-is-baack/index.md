---
title: 'VML is baack...'
date: Thu, 12 Aug 2010 02:36:00 +0000
draft: false
url: /2010/08/12/vml-is-baack/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

There were plenty of heated debates when OOXML was driven to acceptance as an ISO standard. Although we have a lot of experience with OOXML on the Aspose.Words team - we did not participate much in those debates. Today's topic is not about the reasons why we stayed away from those debates. This post is just about one thing I found interesting/funny we came across recently.

As you might know ISO/IEC-29500:2008 specifies two levels of OOXML compliance - Transitional and Strict.

The Transitional compliance level is pretty much the old ECMA-376 plus some new features.

The Strict compliance level disallows some of the really _MS Word early versions_\-flavoured features. For example, the Strict compliance level specifies that all drawings in an OOXML document are specified as DrawingML shapes, not as VML (Vector Markup Language).

But the interesting thing that we came across is that ISO 29500 allows extensions and Microsoft did not waste any time by implementing something that is known as _\[MS-ODRAWXML\]: Office Drawing Extensions to Office Open XML Structure Specification_. This document basically puts VML back into ISO 29500 Strict documents via the standard extension mechanism.

So it turns out that if you thought an OOXML document that complies to ISO 29500 Strict cannot contain VML - you were wrong, it can - via the extension mechanism provided by the same ISO 29500 standard.








