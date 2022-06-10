---
title: 'Process Multiple OneNote Files in Parallel Threads in C#'
date: Mon, 06 May 2019 15:51:52 +0000
draft: false
url: /2019/05/06/process-onenote-file-in-para%e2%80%8blle%e2%80%8bl-threads-with-aspose.note-19.3/
author: Ahsaniqbal
summary: ''
tags: []
categories: ['Aspose.Note Product Family']
---



{{< figure align=center src="images/Aspose.Note-for-.NET_1.png" alt="">}}


It will please all of you to know that new updated version of [Aspose.Note for .NET 19.3][1] is available now. This release contains enhancements and improvements which will provide you a quality product and performance rich version. A common programming paradigm i.e. parallel processing is targetted this time and improvements are made to get error free functionality in this environment. Please visit the [release][2] [notes][3] section of API documentation for details about this new release.  

## Process Multiple Files in Parallel using C#

You may require to use this library in a multi-document processing environment like opening multiple documents in separate threads and say searching hyperlinks along with making replacements in parallel for all the documents. Sometimes you may get an exception like "Object is currently in use elsewhere" while saving a document and getting the process terminated. This was causing hindrance in some cases and there was a desire to investigate this issue thoroughly. It was identified that as System.Drawing.Graphics class is used by Aspose.Note, this was causing the problem because it was was not threadsafe somehow and was verified by disabling it for successful operations. Be calm! This issue is resolved now and you can use Aspose.Note without any error while processing multiple documents in parallel.

## Other Improvements

*   Exception "Aspose.Note.UnsupportedFileFormatException-Unknown binary data compression in OneNote Online file format" was raised while loading some OneNote files. This issue is resolved now.
*   Another exception "System.ArgumentOutOfRangeException-Index was out of range. Must be non-negative and less than the size of the collection occurred in mscorlib.dll" is also resolved in this release.




[1]: https://www.nuget.org/packages/Aspose.Note/19.3.0
[2]: https://docs.aspose.com/display/notenet/Aspose.Note+for+.NET+19.3+Release+Notes
[3]: https://docs.aspose.com/display/notenet/Aspose.Note+for+.NET+19.1+Release+Notes




