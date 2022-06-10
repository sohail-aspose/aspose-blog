---
title: 'Nemerle: The Mage''s Language'
date: Tue, 22 Aug 2006 23:25:00 +0000
draft: false
url: /2006/08/22/nemerle-the-mages-language-aspose/
author: DmitryV
summary: ''
tags: ['Dmitry Vorobyev']
---

Nemmerle is the name of a mage from Ursula K. Le Guin's book "A Wizard of Earthsea". I don't know whether it's a fairy trick of his but Nemerle now seems to be one of the most popular among the family of "alternative" .NET languages and its popularity is growing. I haven't had a chance to explore it in-depth but from what I've learnt so far I can confidently state I like it!  

Nemerle resembles C# but is much more complex and flexible. Whereas C# looks like a hybrid of C++ and Java, Nemerle is a thermonuclear mixture of C#, Java, VB .NET, Pascal, and even Lisp And that's not bad. That's great!  

Nemerle offers functional, object-oriented and imperative features. Actually, there are _tons_ of great features offered by Nemerle and it's impossible (and not reasonable) to list all of them here. I will just highlight the most distinctive of them.  

**Meta-programming.** This is what really makes this language POWERFUL. Imagine you could create your own programming constructs using special macros. You could extend the language as you like. Roughly speaking, you could sculpture almost new programming language fully adjusted to your needs! That's what is possible in Nemerle.  

Even not running to an extreme, meta-programming is not yet another developer's toy, it **is** useful. The process of development is full of various programming patterns we are forced to repeat more and more. We use many techniques and tools intended to make this easier. The examples are VS snippets or ReSharper Live Templates. C# also includes few built-in structures which simplify certain areas of programming (**lock** instead the use of monitors, **using** instead of calling **Dispose** inside a **finally** block, and so on), but their number is low and, what is more important, they are hardcoded into the syntax of the language and you cannot introduce your own.  

Let's take an example. Very often we create classes with several fields initialized in the constructor. There's nothing else to do within constructor body, just assign parameter values to a couple of fields. So we have a pattern here, and it would be nice to automatize the process of creating such constructors. We can use a tool to achieve that, and we can not declare the constructor at all if we use Nemerle, but apply a special macro instead  

Take a look how easy it is (notice Nemerle uses Pascal style for declaring fields and parameters):  

\[Record\]  
class Person {  
  public name: string;  
  public age: int;  
  public sex: bool;  
}  

This is equivalent to  

class Person {  
  public name: string;  
  public age: int;  
  public sex: bool;  

  public this (name: string, age: int, sex: bool) {  
    this.name = name;  
    this.age = age;  
    this.sex = sex;  
  }  
}  

**Record** is a macro which checks what fields are defined inside the class and generates constructor to initialize them. It is a built-in macro and it looks like a C# custom attribute but you are free to develop your own that define custom language constructs such as new loop types or anything else!  

**Type inference.** Another great feature that allows you not to specify types of variables you declare. The compiler is smart enough to infer the types itself from variable assignments and similar things. That is, you don't need to write such long statements as:  

Dictionary<string, int> d = new Dictionary<string, int>();  
d.Add ("Ala", 7);  
foreach (string s in args) {  
  ...  
}  

but you can write instead:  

def d = Dictionary ();  
d.Add ("Ala", 7);  
foreach (s in args) {  
  ...  
}  

This feature will also be supported in C# 3.0 but Nemerle offers it now and it's still obscure what compiler will be smarter to infer types. At least Nemerle compiler already shows great results in this area!  

**Functions.** You can define functions inside methods. I guess this would be useful to not overburden classes with specific small methods such as printing a formatted string. Here is an example which says hello to all persons in list:  

public Greet (people: list\[string\]): void {  
  def say\_hello (s) {  
    System.Console.WriteLine ($"Hello $s");  
  }  

 foreach (person in people)  
    say\_hello (person);  
}  

The example shows more peculiarities of Nemerle: lists are special built-in elements of the language, and $ is used to mark a special active region within a string represented by an expression (and a simple identifier is also considered an expression) which gets evaluated and replaced with the result (nice and easy, compare it with C# string formatting).  

**New language constructs.** Although C-based languages allow to implement everything a developer needs using their basic constructs, those constructs might sometimes be a bit too common to nicely put developer's intentions into code. For example, the **for** loop is used very often to just repeat a block of code a certain number of times without any special loop conditions and without the use of the control variable. So isn't writing **for (int i = 0; i < 100; i++)** a little redundant for such cases? That's what we must write however. Nemerle includes a number of "more specialized" language constructs to ease developer's life. So you can simply write **repeat (100)** before a block to repeat and that's it. I presume this construct is also defined by means of macros and this is COOL  

I have actually mentioned here just a minuscule part of staggering Nemerle capabilities. To learn them all, visit the homepage of the language [www.nemerle.org][1].  

I'm personally fond of C# but Nemerle just looks like the next step of evolution




[1]: http://www.nemerle.org/



