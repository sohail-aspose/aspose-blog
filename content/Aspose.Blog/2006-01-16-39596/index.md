---
title: 'Unit Tests – The Secret of Quality'
date: Mon, 16 Jan 2006 13:21:00 +0000
draft: false
url: /2006/01/16/39596/
author: DmitryV
summary: ''
tags: ['Dmitry Vorobyev']
---

Before I joined the Aspose Auckland team, I didn’t consider unit testing to be somewhat important or, furthermore, necessary for development. Indeed, the usefulness of unit tests is not too obvious at first glance, especially if the project is not so big. We have to write significant amounts of extra code thus expending extra time and efforts… are there any benefits actually?

Well, unit testing proved to be **very** important when developing projects consisting of more than several simple classes. Moreover, now I’m completely sure that the development of such complex projects as Aspose.Word is simply impossible without it. Rather, it’s still possible – but you should then forget about something called quality and get ready to the fact that adding some feature, even pretty small, may break existing code and you won’t notice it until customers start to complain. Also, get ready to lots of extra hours of working with the debugger, placing breakpoints here and there and watching variable values. And even after you seem to have fixed all reported bugs, no one still can guarantee that there is no real-world situation that would cause your code to fail. Definitely, such a product just cannot be proudly named _the high-quality product_.

Aspose.Word is a pretty complex project which contains numerous classes (its **public** API consists of over 100 classes – guess how many internal ones are inside?). All of them are related with each other in some way – so changing behaviour of one might implicitly affect others. That’s the main reason why unit tests are essential for Aspose.Word development. At the moment Aspose.Word includes about **1000** unit tests and their number grows permanently because **we must write a test (or even a couple of tests, contained in a separate class) when we are going to add some new feature**. That’s the Aspose Auckland Team’s rule. Yes, we should try to create a test before implementing a feature itself; we try to use test-first design approach whenever possible. This approach proved to be very useful since we make getting some results our aim – and only then, keeping in mind what exactly we want to get, we start writing code in order to reach the goals. We could even treat writing “main” code as process of tuning the project so that all the tests get passed – but we don’t do it since we are still programmers, not tuners :)

Another strict rule we must follow is that **we never check in our code until make sure all the tests (both existing and just added) are passed**. Do you see the advantage? This guarantees that: 1) the newly added feature works 2) it hasn’t damaged existing code. Pretty easy, but very effective quality assurance. Breaking this rule may make Roman angry :)

**One of the numerous Aspose.Word unit tests**

```
///
/// Tests cells CSS attributes.
///
[Test]
public void TestCellCss()
{
   mDoc = Open(“TestCellCss.html”);
   Save(“TestCellCss Out.doc”);

   NodeList rows = mDoc.SelectNodes(“//Row”);

   Cells cells = ((Row)rows[0]).Cells;

   Assert.AreEqual(Color.Red, cells[0].CellFormat.Borders[BorderType.Left].Color);
   Assert.AreEqual(Color.Yellow, cells[0].CellFormat.Borders[BorderType.Right].Color);
   Assert.AreEqual(Color.Green, cells[0].CellFormat.Borders[BorderType.Top].Color);
   Assert.AreEqual(Color.Black, cells[0].CellFormat.Borders[BorderType.Bottom].Color);

   Assert.AreEqual(LineStyle.Emboss3D, cells[0].CellFormat.Borders[BorderType.Left].LineStyle);
   Assert.AreEqual(LineStyle.Single, cells[0].CellFormat.Borders[BorderType.Right].LineStyle);
   Assert.AreEqual(LineStyle.DashSmallGap, cells[0].CellFormat.Borders[BorderType.Top].LineStyle);
   Assert.AreEqual(LineStyle.Emboss3D, cells[0].CellFormat.Borders[BorderType.Bottom].LineStyle);
   Assert.AreEqual(1, cells[0].CellFormat.Borders[BorderType.Left].LineWidth);
   Assert.AreEqual(2, cells[0].CellFormat.Borders[BorderType.Right].LineWidth);
   Assert.AreEqual(1, cells[0].CellFormat.Borders[BorderType.Top].LineWidth);
   Assert.AreEqual(2, cells[0].CellFormat.Borders[BorderType.Bottom].LineWidth);

   Assert.AreEqual(10, cells[1].CellFormat.LeftPadding);
   Assert.AreEqual(10, cells[1].CellFormat.RightPadding);
   Assert.AreEqual(5, cells[1].CellFormat.TopPadding);
   Assert.AreEqual(5, cells[1].CellFormat.BottomPadding);

   Assert.AreEqual(CellVerticalAlignment.Bottom, cells[2].CellFormat.VerticalAlignment);
}
```

Our tests are split by logical categories each of which contains a set of related classes, and each class, in turn, contains individual tests. The overwhelming majority of the tests is used for the purpose mentioned above – making sure that all the features of the product function properly and other developers may comfortably continue working on their parts of code. However, we successfully use unit tests to resolve other tasks. For example, we test code reported by the customers to reproduce issues; we simply create a new test based on the customer’s code snippet. In general, we use unit tests whenever it is necessary to run Aspose.Word code and see the results. Unit tests appear to be an excellent tool whose flexibility allows reproducing any real-world situation and check if Aspose.Word is able to stand it.  

We use [NUnit][1] as the most popular unit testing framework for .NET. NUnit GUI is something like litmus paper of code quality – our goal is making it completely green so we could be sure that everything works :) Indeed, it is very convenient since Aspose.Word is a program component which does not provide graphical interface. In order to test it, we could write some testing application… or use that simple but really powerful framework.




[1]: http://www.nunit.org/



