---
title: 'Aspose.Word Exceptions'
date: Wed, 02 Nov 2005 17:54:00 +0000
draft: false
url: /2005/11/02/35002/
author: Romank
summary: ''
tags: ['Roman Korchagin']
---

I recently read this article in MSDN blogs [Design Guidelines Update: Exception Throwing][1] and this prompted me to finally review how Aspose.Word throws exceptions.  

I must say I agree with everything what Krzysztof says in that article and I was actually doing exactly that for ages in my C++ and Delphi projects long before .NET. Of course that was raising some eyebrows from many developers whom I used to work with, but I knew it would come out right in the end.  

So the review of Aspose.Word exception handling revealed that there is really not much to change. Aspose.Word always used to consistently throw exceptions mostly using the appropriate exception classes already defined in the .NET framework. I just tidied up in a few places and I now can document it as a policy, effective from Aspose.Word 3.3 due to be released soon.  

1\. Aspose.Word throws an exception when a method cannot complete the operation it is designed to do.  

2\. When an invalid argument is passed to Aspose.Word, an exception derived from ArgumentException is thrown. In some cases (for example when a string cannot be null and cannot be an empty string) an instance of ArgumentException itself is thrown. Ideally, argument exceptions should only be thrown if you pass an invalid argument into one of the public methods so the message makes it clear you are trying to do something wrong. However, there are many more internal classes in Aspose.Word than public and the internal classes also throw argument exceptions and in theory there could be a situation when you get an ArgumentException, but you did not pass that argument into a public method. This should not normally happen, it would be a bug in our code if it happens.  

3\. When you call a method of Aspose.Word and the operation cannot be completed in that particular current state, an InvalidOperationException will be thrown. For example, trying to insert a cell while table and row were not created in DocumentBuilder.  

4\. The NotSupportedException is thrown when you try to engage one of the features not supported by Aspose.Word. For example, import from HTML some constructs that are not yet supported (for example many CSS features) or try to open a document in pre-Word97 format.  

5\. Aspose.Word defines one exception class PleaseReportException. This is a specific of the way we work with the binary DOC format. Big chunks of the DOC format are not documented and we sometimes cannot be sure if a particular condition or situation can occur in a document in real life or not. Whenever we detect such a condition in code and think it is safer to stop processing and make the situation vivid instead of silently ignoring it and potentially creating problems, we do that. The idea is that when you see a PleaseReportException, you post the error message in the Aspose.Word Support Forums and attach the problem file. This will help us to quickly learn a new undocumented thing about the DOC format and release a hotfix that processes that file okay.  

6\. Some other standard exceptions defined in .NET are also thrown by some methods, for example FileNotFoundException, CryptographyException when failed to find or decrypt a license file etc.  

7\. All exceptions that can be thrown by the public methods will gradually be fully documented in the API reference.  

8\. We will provide more "tester" methods in the public API so you can do things with a check as opposed to throwing an exception. These methods will only be added where really needed. For example at the moment DocumentBuilder.MoveToMergeField throws if a field is not found in the document. We will provide a way to first detect if there is such a merge field in the document before moving to it. Please feel free to submit suggestions about what operations do you think should be possible without throwing.




[1]: http://blogs.msdn.com/kcwalina/archive/2005/03/16/396787.aspx



