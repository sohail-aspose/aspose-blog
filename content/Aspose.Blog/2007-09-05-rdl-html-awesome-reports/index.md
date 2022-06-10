---
title: 'RDL + HTML = AWesome Reports!'
date: Wed, 05 Sep 2007 22:25:00 +0000
draft: false
url: /2007/09/05/rdl-html-awesome-reports/
author: DmitryV
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

We often stress that the development of our products is customer-driven. This means we respond to customer requests quickly and exhaustively, making customers feel as if they directly participated in the development. This cooperation is mutually beneficial and sometimes results in brilliant ideas indeed.

Yesterday I had a conversation with a customer whose requirement was exporting RDL reports to Microsoft Word documents. The problem was that he wanted his reports to have quite a lot of inline formatting, which is to format text differently within the same textbox.

Some of this text is **bold** and another text is _italic_.

As you know, even such a basic formatting is not supported in Reporting Services. The whole text within a textbox can only have the same formatting. So since this is by design, the problem seems unsolvable…

…unless you have the latest [Aspose.Words for Reporting Services 1.4.1.0][1] installed. Yes, we did come up with some solution and implemented it shortly. The solution is… why not use HTML to format the text within a textbox? Indeed, wouldn't it be nice to simply specify how the text should be formatted:

Some of this text is <b>bold</b> and other text is <i>italic</i>.

and get a proper result when the report is exported to a Word document?

Of course, there are some obvious limitations to this approach:

*   The formatting isn't visible in design time (in Report Builder, Report Manager, etc). Instead, you will see the HTML text as-is.
*   Aspose.Words for Reporting Services is the only rendering extension able to understand and properly format HTML code in textboxes. No one of the "standard" extensions does so.
*   Since the text is hosted in text boxes, all the corresponding restrictions apply. For example, you cannot have form fields within a textbox.

However, if you wish to make your RDL reports formatted much richer when exported to Word documents, this solution is right for you. If you don't care about the appearance of the report in design time, you can insert as complex HTML as you wish, and even use inline CSS styles! That means you can edit a fragment of the report in your favorite HTML editor and then just copy/paste the HTML code into a textbox. Just make sure the report exports without issues (because, as mentioned above, the resulting content may appear not eligible to be hosted within a textbox).

Please refer to the product's [online documentation][2] to know how to enable the "HTML formatting" mode.




[1]: https://downloads.aspose.com/words
[2]: https://products.aspose.com/words




