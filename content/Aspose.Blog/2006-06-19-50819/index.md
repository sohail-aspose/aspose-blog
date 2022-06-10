---
title: 'How to Make Your Teammates Happy'
date: Mon, 19 Jun 2006 22:02:00 +0000
draft: false
url: /2006/06/19/50819/
author: DmitryV
summary: ''
tags: ['Dmitry Vorobyev']
---

I'm sure there are a number of funny "guides" for programmers over the Web – collections of derisive rules that should NEVER be followed. At least I've seen a pretty comprehensive guide that shows [how to write unmaintainable code][1] in Java. Anyway, this inspired me to design a list of helpful hints intended for .NET (and not only .NET) developers who desire to obtain recognition in their teams  It's far from being that comprehensive (after all, it's just a blog post), yet I would expand this list with great pleasure.

Few of the hints are based on my own past experience  I'm thankful to Roman mentoring me on such things personally as well as other pros like Martin Fowler mentoring us all through his books and articles.

**30 helpful hints for successful collaboration in a team**

1\. Refactoring is evil. It was developed by those who wanted you to waste your time by moving code fragments from one place to another without improving functionality. If the result doesn't get better, why to make such efforts?  
2\. Make methods as long as possible. Methods occupying over 500 lines are welcome. Who needs lots of small methods each of which performs one tiny action? Also, the lesser calls are made, the better.  
3\. Don't use comments or use it to store things not related to programming. Comments are little oases in code where we can record our thoughts and reflections and communicate with our colleagues in a natural language. So take a rest from coding when writing comments, just express yourself there!

 // Joe is a moron :)  
 a = b;

4\. Name your classes, methods, fields, variables, and other language units in such a way that you were the only person able to understand their real purpose. You can use any abbreviations you want. You can even mislead your teammates so that the purpose of your method or variable would be opposite to what its name means. Why should someone else be familiar with what you've been toiling at for a long time?!  
5\. Unit testing is another devilish thing invented by those who probably had plenty of time. Can you afford to spend extra hours creating non-production code only intended to check if your main code is okay? No, you can't! First of all, you must trust that your code is ideal and contains no bugs – and you will attain to that very soon, you'll see. Second, if however several minor errors occur in your code, you can always catch them all using a debugger. Modern debuggers are so advanced that you will find and eliminate all probable errors very quickly.  
6\. Never separate logical blocks of code with blank lines. Do you want your source files to grow? So make sure that each line is effectively filled with code.  
7\. Cause a scandal if conflicts occur after you update your code from repository. It can damage your original idea if you merge their code with yours manually.  
8\. Naming conventions are rubbish. Do you need all those "pascal", "camel" etc? Identifiers should not follow any unified style because it limits your creativity. Just take a glance how nice letter case mixing looks:

 int mY1nteGeRvAr1Able;  
 float FL0At;

9\. It's okay to use many temporary variables in your methods. They are stored on the stack so don't worry about memory impact. If you give them abstract names like _temp1_, _temp2_, _temp3_ etc, you can reuse them for different purposes throughout the method.  
10\. Enums are just surrogates of regular numbers. To declare an enumeration, you need to implement its body and figure out a name for each value member and probably assign numeric values. What a stupid idea of giving names to numbers! Just forget it. Magic numbers are much easier to implement. Remember, your time is priceless.  
11\. Avoid using named constants. Again, magic numbers and inline string literals look much better.  
12\. Do not follow any coding standards or guidelines. No one instructs a painter how to paint; programming is also a creative process so don't let them limit your potential. If your code is hard to read and understand, no worries: take a look at Picasso's canvases – they seem tangled too, but they are considered masterpieces though!  
13\. Missing global variables? Static fields are an excellent replacement! You can make them internal or public for easy access from any point. Feel free to read and write values; if your code is supposed to be used in a multithreading environment, it's the headache of the user, not yours.  
14\. Burn your extreme programming books if you have any. If you don't, pretend you have never heard this term. If you really haven't, you're a saint!  
15\. No need to check if parameter values passed to a method are valid (not null, not empty string, within a range of possible values etc). You cannot anticipate all possible scenarios. And you shouldn't care of that.  
16\. Comments are also useful to exclude various code pieces without removing them so that they can be easily brought back in the future. Comment out such pieces regardless of whether you are the author or someone else is. Don't bother leaving descriptions of why you excluded a particular code block. It should be clear from surrounding code.  
17\. Make your code compact. Tabs, spaces, and line breaks are normally ignored by compiler so there's no need in them. Don't indent code blocks. Your code is not a newspaper article or official document so formatting it is redundant.

using System;public class helloWorldclass{public static void metHOd1(){Console.WriteLine("Hello world!");}}  
  
18\. Duplications are a good way to show your productivity to your team leader. Numerous similar fragments of code only differing by value or values they work with make an impression of hard work. Try to disguise your duplications by complicating the code, though, because some team leaders don't like them for some weird reason.  
19\. Never check if your code compiles before committing it into repository. You'll be notified if something goes wrong. You can then say that you've checked the whole thing as usual and somebody probably gonna soil your reputation.  
20\. Use long conditional statements without unnecessary parentheses intended just to make it more readable. Compiler is smart enough to determine the right order of evaluation.  
21\. Large nested **switch/case** blocks might characterize you as an experienced developer.  
22\. The **goto** statement is not bad, moreover, it's a hidden potential of the language, rarely used due to the stupid and wrong common opinion. Why can't you jump to a certain place in your code if the language does allow it? So use gotos frequently to skip code blocks and jump out of loops and your colleagues will consider you programming guru very soon.  
23\. Be frank with your teammates. If you don't like their code, let them know. Show them the right way by replacing their code with yours. After a couple of lessons they will surely accept your coding style and you will gain prestige in the team.  
24\. Organize your source files and folders in such a way that it would take a while to find something. Place several big classes into one file. This prevents curious persons from quick comprehension of your smart and tricky code.  
25\. Create your own implementation of different fundamental things such as collections, sorting algorithms etc. Leave ready solutions to dilettantes. It's cool to create those things from scratch each time you start working on a new project. Maybe you will succeed in inventing some brand new method of storing data or enumerating arrays.  
26\. Your teammates will be thankful if you help them to pinpoint and eliminate their errors. So don't hesitate to modify their code. Accommodate it to your coding style for convenience. Rename variables as you like. Delete excessive code fragments (for example unit tests). Remember, you're the one team!  
27\. Never use properties in your internal (probably public too) classes. They do not add any functionality, just access your fields so don't bother writing them. Use internal or public fields instead. Encapsulation was invented by paranoids.  
28\. Methods accepting 1-2 parameters look not considerable. Try to develop methods whose parameter list consists of minimum 5-6 parameters. Name them _a_, _b_, _c_ and so forth, even if their types are totally different. You will lose your time contriving a nice name for each parameter.  
29\. Don't dispose objects that deal with unmanaged stuff. Garbage collector will kill them automatically. Modern computers are pretty powerful thus releasing some resources earlier doesn't make sense.  
30\. Please forget all these hints unless you want to be violently kicked by your teammates




[1]: http://www.mindprod.com/jgloss/unmain.html



