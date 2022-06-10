---
title: 'Hollings Cancer Center developed an offline feature for Creating and Parsing Word files'
date: Thu, 06 Jun 2019 02:44:53 +0000
draft: false
url: /2019/06/06/create-and-parse-word-files-and-insert-data-into-database-using-apis/
author: William Morgenweck
summary: ''
tags: ['.NET API for Word processing in Web Application', 'Aspose.Words', 'Dynamically create and update MS Word documents', 'Free Technical support', 'MS Word DOC/DOCX parsing API', 'Manipulate content inside MS Word document', 'Parse content of MS Word file', 'Process MS Word files using Aspose.Words for .NET', 'Success Stories', 'free trial']
categories: ['Aspose.Words Product Family']
---

## About Hollings Cancer Center



{{< figure align=center src="images/39242373_10155521618683414_1542351171497230336_n.jpg" alt="">}}


[Hollings Cancer Center][1] is part of the Medical University of South Carolina. When a Researcher asks for data from our various departments, we need to send the request to an Evaluation Committee. We currently have a Web application that asks a series of 10 topics to a committee of evaluators and from the topics, each Evaluator then develops their own set of questions individually to be sent back to the Researcher. The Researcher then needs to respond to each question. If the Evaluator does not think that the question is answered completely, then the process is started over again. All of this information needs to be stored in a database for easy analysis. The initial problem that we had with the Web System was that lots of work needed to be applied to each area of interest. Once a Researcher had spent hours answering one question, sometimes the Internet connectivity is lost. This created the requirement to work off-line.

## Requirements Scenario

We needed a way to work off-line and still be able to parse data back into a  
database. We needed a solution that was available to all end users. We needed a way to present information that was common to the end-user.

## Solution Implementation

Since we had a complete working Web Application, we added the ability to work offline by having the end-user to click on a button and have an email sent to them with a Word Document attachment. The Word document is created with [Aspose.Words][2] on the fly from the series of questions and responses between that Evaluator and the Researcher. We identify each area with [bookmarks][3] and once the document is returned, we have an automatic process that reads the emails and with the help of [Aspose.Words][4], we [parse the Word document][5] and enter the data into the database. Once the process is completed, the parties are notified and the process starts over again. From the time the email is returned, it takes less than 2 seconds to have the data entered into the database. This gives the end-user the comfort that their data is safe on their local machine.

## Benefits

We tried emails but end users would sometimes change too much of our identifying information and we would not know which Study the email would relate. Using the Word document, we could create a cleaner experience with the end-user.

## Future Implementations

In the future, we plan to add additional word documents to the process, such as the final recommendations from the committee.

## Conclusion

There is nothing worse than creating a web application that needs constant monitoring. Using [Aspose.Words for .NET][6], we eliminated the problems that end-users faced while ensuring that their data and work was safe and secure.



{{< figure align=center src="images/Hollings-Cancer-Center-Aspose-Words-Case-study.png" alt="Preview of form with questions" caption="Image 1:- Preview of form with questions">}}




{{< figure align=center src="images/Hollings-Cancer-Center-Aspose-Words-Case-study-1-806x1024.png" alt="Preview of Word document created using Aspose.Words for .NET" caption="Image 2:- Preview of Word document created using [Aspose.Words for .NET](https://products.aspose.com/words/net)">}}




[1]: https://www.hollingscancercenter.org/index.html
[2]: https://products.aspose.com/words
[3]: https://docs.aspose.com/display/wordsnet/Working+with+Bookmarks
[4]: https://products.aspose.com/words/family
[5]: https://docs.aspose.com/display/wordsnet/Working+with+Document
[6]: https://products.aspose.com/words/net




