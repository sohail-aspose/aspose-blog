---
title: 'Instance field vs local variable and parameter'
date: Tue, 06 Sep 2005 21:30:00 +0000
draft: false
url: /2005/09/06/31782/
author: Romank
summary: ''
tags: ['Roman Korchagin']
---

After about 15 years of programming I begin to stumble on some basic object-oriented concepts and I can't sleep well because I can't find a reasonable answer.

Here is the question I'm dealing with now:

**When to use an instance field versus a local variable (and pass it as a parameter) if two or more methods in a class need to share that data?**

For example, MyClass has a public method called ReadTheThing and “the thing“ has a header and a body. I would normally make two private methods ReadHeader and ReadBody and call them from the ReadTheThing method. When ReadHeader is called, it reads some data that is later used in ReadBody. What is the best way to pass that data from ReadHeader to ReadBody?

_//First approach - use the instance field(s) to share the common data between methods.  
_public class MyClass  
{  
    public void ReadTheThing()  
    {  
        ReadHeader();  
        ReadBody();  
        OutputBody();  
    }

    private void ReadHeader()  
    {  
        mHeader = ... some complex algorithm to read the header  
    }

    private void ReadBody()  
    {  
        mBody = ... some complex algorithm to read the body, **uses mHeader, read earlier**.  
    }

    private void OutputBody()  
    {  
        ... some complex algorithm to **process mBody read earlier.  
**    }  
  
    private Header mHeader;  
    private Body mBody;  
}

_//Second approach - use local variables and pass them as parameters between methods.  
_public class MyClass  
{  
    public void ReadTheThing()  
    {  
        Header header = ReadHeader();  
        Body body = ReadBody(header);  
        OutputBody(body)  
    }

    private Header ReadHeader()  
    {  
        ... some complex algorithm to read the header  
        return header;  
    }

    private Body ReadBody(Header header)  
    {  
        ... some complex algorithm to read the body, **uses the header parameter**  
        return body;  
    }

    private void OutputBody(Body body)  
    {  
        ... some complex algorithm to **process body  
**    }  
}

\-----------------

It is easy to come up with a dozen or more of pros and cons for each approach. For example, if too many methods need that data, make it an instance field. If need to return several objects, it might be easier to make them instance fields (probably better split the method actually). Too many parameters passed around and long parameter lists are not nice to deal with. But many instance fields some of which are not initialized during various stages are not nice either. Parameter-less and return-less methods make it harder to understand their scope and effect on potentially many instance fields. etc etc.

So far looks like there is no hard and fast rule here. If you have some ideas, let me know.

For the time being I'm just doing it on a case-by-case basis often combining both approaches in a single class. I cannot say it turns out bad, it turns out okay, but I'm wondering if one can do better. Just don't want to spend too much time thinking about each variable should it be an instance field or passed around as a parameter. I catch myself doing way too many back and forth refactorings here, want to work out a simple guideline to decide when the good is good enough.







