---
title: 'When conversion to PDF in Aspose.Words for Java will be fully available?'
date: Thu, 12 Aug 2010 22:59:00 +0000
draft: false
url: /2010/08/12/when-conversion-to-pdf-in-aspose-words-for-java-will-be-fully-available/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

**Current Situation**

Rendering Word documents to PDF is available in Aspose.Words for Java since version 4.0 released on 30th November 2009.

We call that functionality "BETA" because of several limitations: images are only saved as JPEG to PDF, not all bitmap types are rendered correctly, image cropping is ignored, WordArt is not rendered and a few others.

Aspose.Words for Java 4.0 was followed by a couple of hotfixes, latest 4.0.2 released on 5th March 2010. More details on the releases page [http://www.aspose.com/community/files/72/java-components/aspose.words-for-java/category1378.aspx][1]

In addition to the limitations mentioned above - Aspose.Words for Java conversion to PDF does not have features that were added to Aspose.Words for .NET conversion to PDF in the recent times. Most noticeably, Aspose.Words for Java conversion to PDF does not yet support footnotes, endnotes and update of the TOC (Table Of Contents) field.

**A bit of Background**

Aspose.Words started as .NET project, written in C#. Aspose.Words for Java was only conceived and released several years after Aspose.Words for .NET.

From the start, we wanted Aspose.Words for .NET and Java to be sister-products and have as much of the same API and functionality as possible. We started to develop Aspose.Words for Java by manually porting C# code of Aspose.Words for .NET to the Java programming language. We always tried to port that code almost line-to-line, developing our own .NET-like library classes where needed. The result was two successful products for different platforms with essentially only one code base to maintain.

However, the manual process of porting from C# to Java was very time consuming. We had to carefully select all the changes that were made in C# and make exactly the same changes in Java. We had to repeat that over and over. In addition to time consuming, this was boring.

**CsPorter - Automatic C# to Java Porting Tool**

While practicing manual porting for several years we have accumulated a lot of experience and know-how. We became confident that we can develop and automatic C#-to-Java conversion tool for Aspose.Words and for all other Aspose products.

We did not have ambitions to support automatic porting of WinForms, WebForms, WPF, ADO.NET and other cool .NET stuff. We only had Aspose.Words to worry about - it is a server-side component that just relies on .NET collections, streams and a bit on graphics.

So after several prototypes we choose a suitable technology and begun to work on a project called CsPorter - a tool to automatically port  Aspose.Words C# code to Java.

**Reason for Delays in Aspose.Words for Java**

The vision that we have is to completely regenerate Aspose.Words for Java code from the original Aspose.Words for .NET code in a matter of seconds. Compile and unit test both products and release them with the same set of features, same version number on the same day!

The work on CsPorter has been progressing so well that we shifted resources from maintaining the manually ported Aspose.Words for Java to working on ensuring the speediest delivery of the Aspose.Words for Java automatically ported version.

Basically, we no longer manually port C# to Java code. This is the reason we are not getting TOC, footnotes and endnotes in the Aspose.Words for Java conversion to PDF - we are simply not working on these features directly.

Although the work on automatic porting is progressing well, it is taking longer than expected.

**What we are doing now**

CsPorter as a tool has reached a level where it can port all of the Aspose.Words C# code no "porting problems". But the resulting Java code does not yet compile because the original C# code uses very .NET platform specific classes in a few places. For example CultureInfo, Bitmap, Metafile and so on.

What we are doing now is modifying our C# code to make it automatically portable and compilable on Java. We are making platform abstractions and shifting things around and rerunning CsPorter often to check how many more "compile problems" are out there.

For example, we have recently made Aspose.Words for .NET to measure text widths without relying on .NET Graphics classes. This resolved some autoporting problems.

**Current Autoporting Status**

We have an internal indicator that shows exact progress on making our Aspose.Words C# code autoportable into compilable Java code. This indicator just shows how many generated Java files compile and how many have compile errors.

I can share the current indicator status here:

Compiles okay = 70%

Does not compile = 29.6%

This roughly means that we are 70% done with the full conversion to PDF (and many other features that so far have been missing) in Aspose.Words for Java. It is roughly because after we get 100% code compiles we will surely have some work to do to get all the tests pass.

**What's Next, Estimates etc**

Aspose.Words 10.0, the first version of our .NET and Java autoported product equal in functionality and released on the same day, was planned to go out end of August 2010.

It does no longer seem that AW 10.0 will be ready by end of August. The Java code is only 70% compilable. But the finish line is in sight and the progress is measurable. So just bear with us for a little longer - **a few more weeks**.

I will be happy to publish the AW 10.0 completeness indicator every week from now on in this blog.




[1]: http://www.aspose.com/community/files/72/java-components/aspose.words-for-java/category1378.aspx




