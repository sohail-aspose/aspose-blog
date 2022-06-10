---
title: 'Changes Related to COM Support in Aspose.Words for .NET 9.1'
date: Sat, 15 May 2010 13:42:00 +0000
draft: false
url: /2010/05/15/changes-related-to-com-support-in-aspose-words-for-net-9-1/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

## Change 1: Manual Registration Now

[Aspose.Words.dll][1] is a .NET class library, but you can use it via .NET COM Interop from many other languages such as ASP, Delphi, JScript, Perl, PHP, Python, C++ etc. In order to use Aspose.Words.dll from a COM client you need to have it registered for COM Interop.

The change is that [Aspose.Words][2] for .NET 9.1 does not register Aspose.Words.dll for COM Interop automatically during install. In earlier versions, Aspose.Words.dll has registered automatically.

While we are still considering pros and cons and deciding whether to return the automatic registration or not, you can easily register Aspose.Words.dll for COM Interop manually, please see http://www.aspose.com/documentation/.net-components/aspose.words-for-.net-and-java/use-aspose-words-for-net-via-com-interop.html

## Change 2: No IDL Anymore

We used to supply Aspose.Words.TLB and Aspose.Words.IDL together with Aspose.Words.DLL in versions earlier than 9.1. Now we decided to try and not supply the .IDL file anymore. Please let us know if you need and cannot generate yourself. If there is a lot of feedback, we might have to put it back in.

The reasons I discussed here [http://stackoverflow.com/questions/2825734/how-to-get-idl-from-a-net-assembly-or-how-to-to-convert-tlb-to-idl-in-a-comman][3]




[1]: https://downloads.aspose.com/words/net
[2]: https://products.aspose.com/words/net
[3]: http://stackoverflow.com/questions/2825734/how-to-get-idl-from-a-net-assembly-or-how-to-to-convert-tlb-to-idl-in-a-comman




