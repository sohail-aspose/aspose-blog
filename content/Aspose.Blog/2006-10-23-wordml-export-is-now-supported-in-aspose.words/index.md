---
title: 'WordML Export is now supported in Aspose.Words'
date: Mon, 23 Oct 2006 15:36:00 +0000
draft: false
url: /2006/10/23/wordml-export-is-now-supported-in-aspose.words/
author: Miklovan
summary: ''
tags: ['Vladimir Averkin']
---

Hello Everybody,  
  

That is my first entry in this blog, so let me introduce myself. My name is Vladimir Averkin, I am a development and support engineer in Aspose Auckland team. Besides providing all kinds of technical support for Aspose.Words users at the forums my primary responsibility is the development of XML-related features of Aspose.Words.  
  

Today I would like to introduce the first major result of my development efforts - brand new Aspose.Words DOC to WordML conversion capability.  
  

Some history first.  
  

WordML is yet another MS Word document format that was introduced first in MS Word 2003 and was intended to be the first truly opened and fully documented format for Word documents. The strive for opened and interchangeable document standards began in late 90s and Microsoft was continuously criticized for closed nature of MS Word formats ever since.  
  

MS already had an opened and decently documented format by this time - RTF. But it had several major drawbacks. It was still proprietary, corporate standard, which means that it was created and maintained inside Microsoft and could be changed or updated by MS anytime without anyone's else approval. Even more serious drawback was that DOC to RTF conversion was not lossless. Some formatting was irreversibly lost when converting to RTF. The third problem was that RTF required implementation of special reader/writer, creating of which required quite large development effort from any implementer. Still it was a very good effort for its time and RTF eventually became quite popular in document processing applications.  
  

So WordML became a second attempt of creating an open document format. Its creation began when the industry inclination toward XML became quite evident and the choice of XML markup for the new format was natural and well-founded. The XML handling was already natively supported on many platforms and XSLT, the technology for XML content processing already became quite popular. Also, from the very beginning WordML was intended to support a lossless conversion from DOC. All features existing in DOC format were to be built in WordML. That was not an easy task at the moment as DOC format had already became very large and complex.  
  

Microsoft was quite successful in the task of creating a new lossless format, based on widely adopted XML and suitable for XSLT processing. The task of creating well-documented and MS-independent format was not fulfilled though. The documentation for WordML is largely incomplete. Document properties, styles, lists, paragraphs and tables are all  described, although very briefly, and the examples and usage recommendations are scarce. Graphics remained absolutely undocumented. Except for the reference to [VML description][1] in MSDN there is no documentation for graphics at all. Even xml schema is incomplete. For example xml elements for charting are entirely missing even from WordML XML schema. Reference to [VML description][2] in MSDN helps but not much as VML in WordML is wildly and heavily different from VML described in this article. Some constructs look similar enough but in no way this could regarded as the reliable documentation source.  
  

There were also large chunks of document data that MS found difficult or unnecessary to translate to XML form and they were included in WordML as is – as a big piles of Base64-encoded data. That included embedded OLE objects, VBA macros, OCX controls, which could probably be left behind during document processing. But that also included all imaging data, which was tightly and sometimes incoherently packed inside ‘w:bindata’ chunks with no documentation or tip on how to extract it from there. All in all that meant that WordML was suitable enough for processing formatted text data using conventional XML+XSLT means but was entirely unsuitable to handle any graphics or OLE information that was stored inside the document.  
  

All of that is contributing to the fact that there are no reliable tools that can render complex WordML files with a decent fidelity or convert them to other formats. The only instrument that did that job good enough was MS Word 2003. But even MS Word 2003 fails to render some of its WordML files correctly. Try for example to convert Microsoft RTF specification document into WordML and then close and open it in MS Word again. You will see some serious table rendering problems there. The good news that these problems seem to be corrected in the new MS Word 2007.  
  

With all of the above said, we are extremely proud to announce that Aspose.Words is now featuring the first full-scale non-Microsoft DOC to WordML conversion. To try it for yourslef you can download new Aspose.Words 4.0 from here, install it and run DocumentExplorer demo source-code project which provides among other features the ability to open DOC files and save them in WordML.  
  

We have thoroughly checked the conversion quality on several hundreds of tests and we have put a major effort to ensure that not only the resulting WordML files are looking in MS Word exactly as the original documents, but also that the inner xml itself matches the one created by MS Word almost exactly.  
  

With this new and exciting capability Aspose.Words can be used in existing WordML-based document processing solutions as a preprocessor for incoming doc files, thus eliminating the need for MS Word automation use.  
  

The conversion is also extremely fast and can crunch about 2-3 megabytes of a complex, mixed-content documents in a second.  
  

I will be extremely happy if you try this new WordML export capability for yourself and let me know what you think. Please be sure to report if you will find any bugs or deficiencies in there. Your feedback on this is highly welcome!




[1]: http://msdn.microsoft.com/library/default.asp?url=/workshop/author/vml/SHAPE/introduction.asp?frame=true
[2]: http://msdn.microsoft.com/library/default.asp?url=/workshop/author/vml/SHAPE/introduction.asp?frame=true



