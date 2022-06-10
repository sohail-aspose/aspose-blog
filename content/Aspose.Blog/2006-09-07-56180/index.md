---
title: 'A Bit More About Nemerle and Functions'
date: Thu, 07 Sep 2006 20:00:00 +0000
draft: false
url: /2006/09/07/56180/
author: DmitryV
summary: ''
tags: ['Dmitry Vorobyev']
---

After posting my first impression about Nemerle I noticed that I had been criticized by some community members for my superficial knowledge of the language and related concepts. I like constructive criticism and I do accept it; so I'm thankful to those guys for pointing me to that.

However, I'd like to note I didn't try to pose as an expert. I only expressed my current understanding of the language and I advisedly highlighted that in the post. So I think next time I will write a separate large disclaimer to show that the subsequent text will not pretend to be an expert's voice

What was mostly derided by the critics was the part about local functions. They disliked my sentence "I guess this would be useful to not overburden classes with specific small methods such as printing a formatted string". Yet I'm still persuaded this is true (as a particular case), I must admit functions are **much** more important in Nemerle than just a nice but utility feature.

The real power of functions I guess (critics may relax! no more than my personal opinion ) is that they can be passed as parameters and return values. This resembles the behaviour of C# delegates but doesn't require them (although Nemerle does support delegates – probably to satisfy the cases when Nemerle assemblies should be referenced from other .NET languages). Also, unlike delegates, functions are much more flexible. So in this sense functions are similar to other data types.

Here's how a method accepting a function looks like in Nemerle:

Compute(f : int \* int -> int, x : int, y : int) { ... }

Among other parameters this method accepts a function which, in turn, accepts two integer values and returns an integer value.

Nemerle also supports anonymous functions (similar to anonymous delegates in C# 2.0, but no need in delegates again). Anonymous functions might be useful when you need to pass some function to the iterator or filtering method so there's no need to refer it by its name.

You can see how to create an anonymous function inline:

Compute(fun(x, y) { x + y }, 3, 4) { ... }

Nemerle supports different types of lambda expressions – which are basically a syntactic sugar for anonymous functions:

Compute((x, y) => x + y, 3, 4) { ... }

Thus Nemerle provides an exhaustive support for functional programming. I didn't mention here such features as partial application or function decomposition – just because I haven't made them out yet and don't want to mislead you. Although Nemerle doesn't force a developer to use this approach, it offers the mixing of two programming styles: the top-level program structure is object oriented, while in the body of methods functional style can be (and probably should be) used. Therefore – I concluded that, as opposed to my first impression, **functions are a core part of the language**.

Now let me share what I think of it. Although I really admire Nemerle, I do not feel myself "ready" to it yet, at least to use the mentioned "mixed" programming approach. I guess functional programming requires some special cast of mind. I'm not sure whether I will ever "grow" to it and whether I really need that at all. That's why the function use case I proposed might sound dumb for functional programming experts  I'm personally a staunch supporter of the object oriented programming paradigm, and at the moment I do not feel to be in urgent need of using local functions in my code, neither do my colleagues. Time will show if we should change our minds. After all, C# 3.0 will support lambda expressions – is it just a tribute to fashion?







