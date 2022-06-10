---
title: 'Is it Unit Testing or What?'
date: Sun, 26 Feb 2006 01:51:00 +0000
draft: false
url: /2006/02/26/42630/
author: Romank
summary: ''
tags: ['Roman Korchagin']
---

It's not a secret we've been using unit testing and test-driven development for Aspose.Words from the beginning. I've also studied, used and taught unit testing and many XP practices in the "early days", for example, my [Practical Unit Testing][1] articles in MSDN from 2000. It long ago became a part of nature, yet here is something new I noticed that grabbed me.

Most of the unit tests I wrote before, conformed to the "commonly accepted understanding" of what a unit test looks and feels like. It would be a test that basically exercises the methods and properties of one class or tests an interaction between a few classes. If I was writing an algorithm to break formatted text into lines, the tests would create fragments of text, feed them into the line breaking engine and check the line objects created on the output are as expected. There will be of course tests for all the smaller subtasks of the algorithm, such as finding a suitable break position in the line, calculating the height of the line, calculating widths of tab stops and so on. Correct me if this is not what the "normal" unit tests are about.

Here is an example of what I think is a "normal" unit test.

```
/// 
/// Test the fast method of appending children.
/// 
[Test]
public void TestAppendChildForLoad()
{
   Document doc = new Document(false);
   //Appends when there are no children
   Node sect1 = doc.AppendChildForLoad(new Section(doc));
   //Appends when there are some children
   Node sect2 = doc.AppendChildForLoad(new Section(doc));
   //Check document knows children
   Assert.AreEqual(sect1, doc.FirstChild);
   Assert.AreEqual(sect2, doc.LastChild);
   //Check sections know the document
   Assert.AreEqual(doc, sect1.ParentNode);
   Assert.AreEqual(doc, sect1.Document);
   //Check sections know each other
   Assert.AreEqual(null, sect1.PreviousSibling);
   Assert.AreEqual(sect2, sect1.NextSibling);
   Assert.AreEqual(sect1, sect2.PreviousSibling);
   Assert.AreEqual(null, sect2.NextSibling);
}
```

When working on a new code we always rewrite, change classes, methods, interfaces a number of times before we get it right. Since it is TTD, when you want to rework your code, there are usually heaps of unit tests already exist and need updating too. We find it becomes really hard to maintain. You end up rewriting not only code several times but also all the tests for it. The progress really slows very quickly. This is a problem we have not solved yet. How do you achieve TTD yet allow yourself to change the code easily, especially in the early stages? Give up TTD?

These days, however, we are working on a viewer control to render Microsoft Word documents as images of pages. In addition to the "normal" unit testing, we tried a technique of comparing the generated bitmaps against a gold standard pixel by pixel. The technique was first used for Aspose.Chart and then applied to Aspose.Words. The "new unit tests" now look like this:

```
 /// 
/// Test decimal tab alignment.
/// 
\[Test\]
public void TestCustomTabDecimal()
{
TestViewerUtil.VerifyPara(@”Viewer\\LineBuilderTab\\TestCustomTabDecimal”, 0);
} 
```

The approach to compare bitmaps clicked well for a number of reasons and we love it so much that I'm afraid we almost don't write the "normal" unit tests anymore.

The advantages I can see are:

*   True, 100% test first development is easily achieved. Just create a test document in Microsoft Word first. Easy.
*   Unit testing code is easy to maintain - no changes to the unit test if the algorithm changes.

Something that can be considered disadvantages:

*   You don't have tests for the inner workings of the algorithms. It is possible something could go wrong or inefficient deep inside the code yet the output will appear fine and you will not notice the problem.
*   If a test fails, it might be harder to find the actual place in the code that causes the problem since the pixelized output is too far away from the code that performed the job.

So here are two very different beasts both presented and executed as unit tests. I hope you found something useful in the article. Let me know if you have any good thoughts to add.




[1]: https://docs.microsoft.com/en-us/



