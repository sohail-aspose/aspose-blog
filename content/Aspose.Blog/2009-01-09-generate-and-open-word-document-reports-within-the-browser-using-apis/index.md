---
title: 'The University of North Carolina Generates, Prints and Performs Mail Merge in Word Document Reports all within Web Browser'
date: Fri, 09 Jan 2009 16:43:00 +0000
draft: false
url: /2009/01/09/generate-and-open-word-document-reports-within-the-browser-using-apis/
author: Alex Cougarman
summary: ''
tags: ['Aspose.Words', 'Dynamically fill database content inside Word template', 'Dynamically generate MS Word documents', 'Insert Image/Logo inside Word document', 'Mail Merge in MS Word Documents', 'Manipulate Header &amp; Footer inside DOC DOCX files', 'Print MS Word files using Aspose.Words for .NET', 'Success Stories', 'Work with Page Breaks inside Word document']
categories: ['Aspose.Words Product Family']
---

## About University of North Carolina



{{< figure align=center src="images/Screenshot-2020-04-29-at-3.32.17-AM.png" alt="">}}


I work as an analyst in the Department of Application Services, which ensures consistency and quality in the development, implementation, distribution, and support of software solutions supporting campus-wide data management needs at the division, school, department, or any other administrative unit level. We recently were tasked to replace the legacy Immunization Tracking System on OpenVMS with a Web-based, ASP.NET application.

## Project

The Immunization Tracking System ASP.NET application allows the [UNCW Student Health Services (SHS)][1] staff to add, view, edit, maintain and report against immunization information for the students. The application implements a master/details scenario to access the students’ information: A search page enables the staff to enter a person’s first and/or last name and term, and view a hyperlinked result set; upon clicking a person’s name, they are presented with the editable immunization details for that individual. In addition, the users required reports and labels to be created against the Oracle database

The users required that these reports and labels take parameters and be easily saved and printed from the Web. Generation of HTML reports was problematic for a number of reasons:

*   Formatting HTML pages to fit correctly on 8 ½ X 11 paper is next to impossible. HTML does not allow correct page breaks and header/footers.
*   The generation of labels that will print correctly from HTML poses an interesting (if not) impossible challenge.
*   Information cannot be saved from Web browsers to a format that non-technical users can decipher and use.



{{< figure align=center src="images/university-of-north-carolina-immunization-tracking-case-study-aspose-words.png" alt="Immunisation Tracking System preview" caption="Image 1:- The main screen of the Tracking System ASP.NET application.">}}


## Solution

After reviewing the available ASP.NET components in the market, I found the [Aspose.Words for .NET][2] component as the best designed, most powerful, and easiest-to-use choice for generating Word documents on the fly:

*   I just needed to create a template file for the component (_following the [great examples][3] and [documentation][4] on the [Aspose.com site][5]_), instantiate the component in code, and then pass the filename and the data to it. The [Aspose.Words for .NET][6] component took care of the rest. That was easy!
*   I could [include headers and footers][7] in the template files as well as [embed fonts][8] for the users, plus [logos and background images][9] where necessary.
*   Saving the document was an easy task – just choose “Save” from the popup dialog! (_Editor: In this scenario, the Save As dialog is brought up by the browser on the client machine when the document is saved by Aspose.Words into a stream at the server._)
*   [Printing][10] became a no-brainer: Users could output their reports and labels to any printer on the network in any format. [Page breaks][11] were automatically handled by Microsoft Word. (_Editor: The customer relies on Microsoft Word installed on the client machine to open the document and print._)
*   Using Microsoft Word’s built-in Letters and Mailings > Envelopes and Labels, I created Avery label templates for the [Aspose.Words for .NET][12] component to generate the users’ mailing labels as well as labels for their folders and printed records.

In addition, we reviewed service policies: [Aspose’s support][13] is the best! Questions are answered quickly, courteously, and accurately by the [Aspose][14] professionals.

Critical to our project’s success was the power and ease-of-use of the components, and Aspose’s are the most powerful and fit perfectly into a rapid application development environment similar to ours. The [Aspose.Words for .NET][15] API has fit us like a glove; it includes features we didn’t know were possible or so easy to implement. Using simple **[Merge Field][16]** codes in Word along with even simpler calls to the database, we’ve created some powerful documents for the users.

We thought about using Microsoft Word automation in ASP.NET, but its complexity, scalability, security, speed, and lack of features convinced us there had to be a better way. With one developer devoted to this project as well as other tasks and projects, we would have had to forgo many features and provide a rather bland product to our users, without the functionality they needed. Tight deadlines have a tendency to quickly shrink the feature set of an application.

## Conclusion

With [Aspose.Words for .NET][17], we did not have to give up anything! We rapidly and easily implemented the features we wanted (_and those we didn’t know w_ere even _possible_) – all at a very reasonable price and with great service to boot. Additionally, the [Aspose products][18] aren’t tied to any specific database; we’ve got SQL Server, Oracle, and Access. All work with equal aplomb with the component. With [Aspose.Words for .NET][19] API, we can have our cake and eat it, too!

Our development time was reduced dramatically, we got the features we needed, and we got [great service and support][20]. Who else provides these many features, ease-of-use, and such great service? [Aspose.Words for .NET][21] is not just done right – **it is done perfectly!** Thank you [Aspose.Words for .NET][22] for making our job so easy!



{{< figure align=center src="images/university-of-north-carolina-immunization-tracking-case-study-aspose-words-1.png" alt="Preview of document with details" caption="Image 2:- Document preview">}}




{{< figure align=center src="images/university-of-north-carolina-immunization-tracking-case-study-aspose-words-2.png" alt="Preview of output generated with Aspose.Words for .NET" caption="Image 3:- Reports generated by [Aspose.Words for .NET](https://products.aspose.com/words/net)">}}


The reports were sent to the client browser and opened in Microsoft Word.




[1]: https://studentaffairs.unc.edu/
[2]: https://products.aspose.com/words/net
[3]: https://github.com/aspose-words/Aspose.Words-for-.NET
[4]: https://docs.aspose.com/display/wordsnet/Home
[5]: https://www.aspose.com/
[6]: https://products.aspose.com/words/net
[7]: https://docs.aspose.com/display/wordsnet/Working+with+Headers+and+Footers
[8]: https://docs.aspose.com/display/wordsnet/Working+with+Fonts
[9]: https://docs.aspose.com/display/wordsnet/Working+with+Images
[10]: https://docs.aspose.com/display/wordsnet/Print+a+Document+Programmatically+or+Using+Dialogs
[11]: https://docs.aspose.com/display/wordsnet/Working+with+Sections#WorkingwithSections-InsertingaBreak
[12]: https://products.aspose.com/words/net
[13]: https://forum.aspose.com/c/words
[14]: https://www.aspose.com/
[15]: https://www.aspose.com/
[16]: https://docs.aspose.com/display/wordsnet/Mail+Merge+and+Reporting
[17]: https://products.aspose.com/words/net
[18]: https://products.aspose.com/
[19]: https://products.aspose.com/words/net
[20]: https://forum.aspose.com/c/words
[21]: https://products.aspose.com/words/net
[22]: https://products.aspose.com/words/net




