---
title: 'Aspose Customer Newsletter, March 2007'
date: Mon, 05 Mar 2007 16:43:00 +0000
draft: false
url: /2007/03/05/69526/
author: Salman Sarfraz
summary: ''
tags: ['Customer Newsletters']
---

**In This Issue...**

*   **Welcome!**
*   **Product Spotlight: [Aspose.Form][1]**
*   **Aspose.Grid 1.9 Released!**
*   **Aspose.Pdf.Kit for .NET has just got better**
*   **Technical Tip: Multiple addresses for an email message**
*   **Aspose becomes a Sun Business Partner**
*   **Aspose.Cells for .NET 4.1.2 Mega Hotfix**

Welcome to the March 2007 issue of the Aspose Newsletter! In this month’s newsletter, we will provide some introductory information about our recently released spotlight product: Aspose.Form. We will also cover the new business partnership of Aspose with the company Sun and look at the new exciting features offered by Aspose.Grid in its recent major release. You will learn about the latest news from Aspose along with the monthly Tech-Tip, which demonstrates how you can specify multiple email addresses for an email message in a smarter way using Aspose.Network.

**Product Spotlight**

[Aspose.Form][2] is a GUI based .NET component that provides a set of powerful web controls to operate InfoPath templates through web browser. Aspose.Form is written in native C#, is lightening fast and works great with all kinds of ASP.NET web applications. Whenever you want to expand the power of InfoPath templates across internet, Aspose.Form is sure to fully accommodate your needs.

Aspose.Form can easily be embedded in your web pages. All you have to do is just to provide the path of your InfoPath template to Aspose.Form control and it will automatically open the InfoPath form in the web page. All InfoPath controls like Plain Text, Check Box, Option Button, Drop Down, List Box, Rich Text, Bulleted List, Numbered List, Date Picker, Inline Image, Linked Image, Repeating Table, Section & Repeating Section etc. are fully supported by Aspose.Form. Users can fill forms manually. However, it's also possible to fill forms automatically using Xml based data files. Please [download][3] the free evaluation version of Aspose.Form to see how it fulfills your business needs. To learn more about its usage, please [click here][4].

![](https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/total/272x272/aspose_total-for-net.png)  
[![][5]](https://downloads.aspose.com/)

**Aspose.Grid 1.9 Released!**

![](https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/total/272x272/aspose_total-for-net.png)

We are happy to announce a new release of [Aspose.Grid][6]. With the new and exciting features of Aspose.Grid 1.9, you will feel an improved web experience. These new features include the support of multiple languages, multiple rows selection, selecting cells through keyboard, creating hints in row and column headers, pasting a string to multiple cells and date time calculation etc. Moreover, many new client and server side events and functions are also added to provide more control of the Grid to the developers. The performance of formula engine is also greatly optimized to make it 20 times faster than the older one. For more details, please [visit][7] the official release page of Aspose.Grid 1.9.

**Aspose.Pdf.Kit for .NET has just got better**

![](https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/pdf/272x272/aspose_pdf-for-net.png)

With the addition of some nice features and few important bug fixes, [Aspose.Pdf.Kit][8] 2.3.3.0 has just got better. Now, developers can set page numbers on different positions of a page. It’s also possible to delete pages from a PDF document. Moreover, the support for reading strange PDFs with long “refx” and flattening fields on PDFs created by Adobe Designer 8.0 is also provided. Few bugs related to reading, printing, converting and concatenating PDF documents are also fixed. To get more details about the improvements made in Aspose.Pdf.Kit 2.3.3.0, please [click here][9].

**Technical Tip**

**Multiple addresses for an email message**  
  
Sending an email message to multiple recipients is a very common scenario and there are many ways to do that using [Aspose.Network][10]. Normally, we add a recipient of an email message by using **MailMessage.To.Add()** method. But, to add more recipients, **Add()** method needs to be called many times. So, Aspose.Network also provides a smarter way to perform this task using its powerful email address parser as shown below:

\[C#\]

//Instantiating a MailMessage object that represents an email message  
Aspose.Network.Mail.MailMessage message;  
message = new MailMessage();

//Specifying multiple recipients for the email message  
message.To = "Tom <Tom@aspose.com>, Jerry <Jerry@aspose.com>";

\[VB\]

‘Instantiating a MailMessage object that represents an email message  
Dim message As New Aspose.Network.Mail.MailMessage

‘Specifying multiple recipients for the email message  
message.To = "Tom <Tom@aspose.com>, Jerry <Jerry@aspose.com>"

Using this approach, email addresses are specified as a string with display names followed by their email addresses separated by commas, which tell the parser that multiple addresses are used.

**Aspose becomes a Sun Business Partner**

![](https://purchase.aspose.com/temporary-license)

We are very pleased to announce our new business partnership with the company Sun. For many years the development community has primarily known Aspose as a .NET component provider. However, Aspose has also had a very strong initiative to support the Java platform as well. This new partnership is another effort to help extend that initiative and continually provide better support for Java developers. If you would like to read the full story, please [click here][11].  
 

**Aspose.Cells for .NET 4.1.2 Mega Hotfix**

![](https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/total/272x272/aspose_total-for-net.png)

In the month of February, 2007, the Aspose.Cells team released a Mega Hotfix [Aspose.Cells][12] 4.1.2 that provides about 9 bug fixes related to concatenation of ASCII characters, copying of worksheets with images, pivot table, formula calculation engine and other general issues. Moreover, besides these bug fixes, few new features are also added to Aspose.Cells to make it more powerful. Be sure to check out the [full list][13] of these bug fixes and newly added features. Please [download][14] the latest release now to make your applications work better using Aspose.Cells.




[1]: https://downloads.aspose.com/
[2]: https://downloads.aspose.com/
[3]: https://downloads.aspose.com/
[4]: https://blog.aspose.com/
[5]: https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/total/272x272/aspose_total-for-net.png
[6]: https://downloads.aspose.com/
[7]: https://blog.aspose.com/
[8]: https://downloads.aspose.com/pdf
[9]: https://blog.aspose.com/
[10]: https://downloads.aspose.com/
[11]: https://blog.aspose.com/
[12]: https://downloads.aspose.com/cells
[13]: https://blog.aspose.com/
[14]: https://downloads.aspose.com/cells



