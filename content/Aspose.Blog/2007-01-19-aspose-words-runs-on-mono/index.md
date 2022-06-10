---
title: 'Aspose.Words runs on Mono!'
date: Fri, 19 Jan 2007 08:21:00 +0000
draft: false
url: /2007/01/19/aspose-words-runs-on-mono/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

We've been asked several times by our customers whether [Aspose.Words][1] is supported on [Mono][2]. Now we've done some preliminary tests running Aspose.Words on Mono 1.2 and I'm happy to tell we have not encountered any problems so far! It seems to work great.

This makes Aspose.Words the only library avaialble in the world that deals with Microsoft Word documents on Mono because as far as I can tell none of the other competing components work on Mono.

I've downloaded Mono 1.2, compiled and run the following simple program against a big 5mb Microsoft Word document with lots of complex formatting, tables, and images:

```
using System;
using Aspose.Words;

class Hello
{

static void Main()
{
 try
 {

 License l = new License();
 l.SetLicense(@”Aspose.Words.lic”);

 Console.WriteLine(“Loading.”);
 Document doc = new Document(@”C:\X\Aspose\Aspose.Words\Doc\Word2003RTFSpec.doc”);

 Console.WriteLine(“Saving DOC.”);
 doc.Save(@”C:\mono out.doc”, SaveFormat.Doc);

 Console.WriteLine(“Saving RTF.”);
 doc.Save(@”C:\mono out.rtf”, SaveFormat.Rtf);

 Console.WriteLine(“Saving WordML.”);
 doc.Save(@”C:\mono out.wml”, SaveFormat.WordML);

 Console.WriteLine(“Saving HTML.”);
 doc.Save(@”C:\mono out.html”, SaveFormat.Html);

 Console.WriteLine(“Saving TXT.”);
 doc.Save(@”C:\mono out.txt”, SaveFormat.Text);

 Console.WriteLine(“Saving XML for Aspose.Pdf.”);
 doc.Save(@”C:\mono out.xml”, SaveFormat.AsposePdf);

 }
 catch (Exception e)
 {
  Console.WriteLine(e.Message);
 }

 Console.WriteLine(“Done. Press any key.”);
 Console.ReadLine();
}
}
```

This seemingly simple example actually tests quite a lot. Apparently the guys at Mono did some great work because it worked like magic. It worked fast and produced exactly the same results as running with the .NET Framework.  

We tried running Aspose.Words on Mono a year or more ago, but it produced so many exceptions that we did not even bother sorting it out. I'm happy to see that Mono has evolved so much.

If you are planning on using Aspose.Words on Mono, I would like to define some policies:

1.  We have not tested all of Aspose.Words functionality on Mono yet, but we will do more tests. For example, we have not tested whether mail merge with ADO.NET data sources works.
2.  We will provide free technical support for Aspose.Words as usual, but there could be issues that we will not be able to resolve, say because some functionality required by Aspose.Words and available on .NET is missing in Mono.
3.  The main idea to gather is that if you use Aspose.Words on Mono you might not be able to do all what's available when running Aspose.Words on .NET and we don't know what it is yet.




[1]: https://products.aspose.com/words
[2]: http://www.mono-project.com/Main_Page




