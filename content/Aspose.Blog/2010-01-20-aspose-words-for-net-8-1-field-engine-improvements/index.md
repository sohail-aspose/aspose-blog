---
title: 'Aspose.Words for .NET 8.1 Field Engine Improvements'
date: Wed, 20 Jan 2010 19:18:00 +0000
draft: false
url: /2010/01/20/aspose-words-for-net-8-1-field-engine-improvements/
author: DmitryV
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Field update was first introduced in Aspose.Words for .NET 7.0 a few months ago (in fact, it was the last decade – just think about it!). You can read about it in this post: http://www.aspose.com/community/blogs/aspose.words-product-family/archive/2009/09/13/field-update-in-aspose-words-the-killer-feature-of-2009.aspx. Since then, the module we call field engine (or field evaluation engine) was significantly improved. In this post I will tell you what enhancements were made in Aspose.Words for .NET 8.1 we have just released and show what Aspose.Words is now able to do.

*   Preserve Formatting in IF Fields
*   Bookmark References
*   Cell References
*   Fixes

**Preserve Formatting in IF Fields**

IF fields were number one our customers wanted to be updated by the component. That’s why we implemented them from the very beginning, starting with the release where field evaluation engine was first introduced. However, there used to be a limitation: rich contents for _TrueText_ or _FalseText_ were not preserved. It means that if you used something like “**_Tr_**ue” or “False”, you saw just a plain text “True” or “False” after field update. Moreover, if you inserted a table or a shape into an IF field as an argument, it got lost completely.

We are happy to announce that Aspose.Words for .NET 8.1 does support this feature. You can set anything as _TrueText_ or _FalseText_ value and it will be preserved when evaluating field result. Imagine you have a complex IF field whose _TrueText_ is a table and _FalseText_ is a shape:

Now let’s update fields via Aspose.Words:

Document doc = new  Document("TestPreserveTables.docx");  
doc.UpdateFields();  
doc.Save("TestPreserveTables Out.docx");

(which is a standard code to update fields in the whole document). Open the resulting document, press Alt-F9 to switch to field result mode and you will notice that field result is the table, because it is _TrueText_ for the IF field and the expression is **2 > 1**, which is true:

Now let’s change the expression to false:

Run the field update code and open the resulting document. You will notice that field result is the shape, because it is _FalseText_ for the IF field and the expression was changed to **2 < 1**, which is false:

Even more, _TrueText_ or _FalseText_ may include paragraph or section breaks, and they will be preserved as well! Let’s make sure:

After updating fields, we see the following (note Word shows section breaks within field result as page breaks for some reason):

**Bookmark References**

Microsoft Word allows to reference bookmarked contents from expressions. That means that you can bookmark two numbers, say **2** and **3**, as **A** and **B**, respectively, and then reference them from a formula field looking like **\=A+B**:

After the field is updated, its value should be **5**. Let’s check if Aspose.Words knows arithmetic. Run the field update code shown above and open the resulting document. Voila:

Too easy, isn’t it? A good pupil should handle more difficult tasks. What about **A** being a four cells table with a number in each cell and **B** being an expression that includes a formula field?

Let’s calculate the correct result. For the bookmark **A**, Word sums up the values in the table, so **A = 1 + 2 + 5 + 6 = 14**. The average between **2** and **6** is **4**, so **B = 3 + 4 – 4 = 3**. Hence **A + B = 14 + 3 = 17**.

Run field update code and make sure the result is correct:

Good boy! :)

**Cell References**

Another great feature offered by Microsoft Word (and now supported by Aspose.Words) is cell references. When an expression is inside a table, you can reference its cells by using special identifiers, which resembles the way Microsoft Excel works. For example, you can reference a single cell by using an identifier like **A1**, **B4**, **F8** etc, where the letter means a column and the number means a row, thus **A1** referencing the upper left cell in the table:

Updating fields in this document by means of Aspose.Words gives the expected result:

Apart from that, you can designate a whole cell range in your expression. Cell range may serve as an argument of a function that accepts a list of values, i.e. _SUM_, _AVERAGE_, _MIN_, _MAX_ etc. In this case the function subsequently takes the value of each cell in the range.

You can specify an explicit rectangular range like **A1:B2**, which means the function should work with four cells **A1**, **A2**, **B1** and **B2**. You also can omit a letter or a number, instructing the function to take all cells between two columns or two rows, inclusively. For example, **A:D** means all cells between the columns **A** and **D**, including the columns themselves, and **3:3** means all cells in the row **3**.

Finally, you can use a special word like **ABOVE**, **BELOW**, **LEFT** or **RIGHT** to tell the function it should take all cells above, below, to the left or to the right of the cell the expression resides in.

I tried to create a table that demonstrates some of these features:

Running field update via Aspose.Words produces correct results everywhere:

Another trick is that you can reference table cells even from outside the table. To achieve that, you should bookmark the table and precede a cell range serving as a function argument with the name of the bookmark. Let’s bookmark the table from the last example, name the bookmark **Table** and try to calculate the biggest value in the table using the _MAX_ function placed outside:

Aspose.Words correctly handles what’s going on:

**Fixes**

No need to say that Aspose.Words for .NET 8.1 includes a bunch of fixes for the field engine. For example, there used to be a problem with double quotes messed up when IF fields contained merge fields enclosed in double quotes. Also, hyperlinks could lose formatting after update… These and other bugs are now fixed, and as ever, feel free to post an inquiry in our [support forums][1] if you encounter any problem.




[1]: http://www.aspose.com/community/forums/aspose.words-product-family/75/showforum.aspx




