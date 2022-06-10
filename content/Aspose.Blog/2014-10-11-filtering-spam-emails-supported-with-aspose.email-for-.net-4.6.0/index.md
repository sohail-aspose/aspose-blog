---
title: 'Filtering Spam Emails Supported by Aspose.Email for .NET 4.6.0'
date: Sat, 11 Oct 2014 08:06:32 +0000
draft: false
url: /2014/10/11/filtering-spam-emails-supported-with-aspose.email-for-.net-4.6.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

[![][1]](https://products.aspose.com/email)We are pleased to announce the release of Aspose.Email for .NET 4.6.0. This month’s release empowers our API users to categorize emails as spam using the Bayesian Spam Analyzer. It also brings improvements to the Personal Storage (PST) file size created using the API. This month’s release also provides the capability to filter emails from mailbox by specifying time as well as date. To get a complete idea of what is new and fixed; please visit the [product download page][2]. You may also share your feedback with us in the [Aspose.Email forum][3].

## .NET Email Spam Filter

This month’s release introduces a high accuracy anti-spam filter that is based on the naive Bayes classifier. Bayesian spam filters provided a very powerful way for dealing with spam messages. The SpamAnalyzer class of Aspose.Email is used to train the filter to establish the criteria for determining the messages as spam or ham (non-spam).

**Train filter**: The very first step is to train the filter to recognize spam and non-spam messages. This can be done by establishing a set of (say 100-200) spam and ham messages. Once the sets are ready, the filter needs to be trained by calling the the SpamAnalyzer class’s TrainFilter method as shown in the following code sample.

```
SpamAnalyzer analyzer = new SpamAnalyzer();

for (int i = 0; i < hamFiles.Length; i++)
{
    MailMessage hamMailMessage;
    try
    {
        hamMailMessage = MailMessage.Load(hamFiles[i]);
    }
    catch (Exception)
    {
        continue;
    }

    Console.WriteLine(i);
    analyzer.TrainFilter(hamMailMessage, false);
} 
```

This is done for the spam message set as well. Once done, the classifier’s results are saved to disc in a database file. This is done by calling the SaveDatabase method:

```
analyzer.SaveDatabase(dataBaseFile); 
```

**Testing:** Once the training is done, the output database file can be used to test message filtering by calling the SpamAnalyzer’s Test method for each test message which provides the probability of a message being spam.

## Retrieving Messages based on Date & Time

The POP3 client of the Aspose.Email API already allows you to retrieve messages from a mailbox based on the date specified in MailQuery. Though this is enough to retrieve messages between two dates, it restricts the searching to dates only where the POP3 protocol also provides support for searching based on time . This month’s release further enhances the messages searching capability to be time-based. An overloaded member of MailQueryBuilder helps achieve this by setting the DateComparisonType to ByDateTime.

## Reduction in PST Size

This month’s release also brings improvement to the size of PSTs created with Aspose.Email. For a known set of emails, the API now creates a smaller PST as compared to previous versions. We are still working to bring further improvement to this area.

## Bug Fixes and Other improvements

This month’s release also fixes a number of bugs that were reported with our last month’s version. These include:

*   Encoding issues when converting messages between various formats.
*   Issues related to appointment timings when saved using Aspose.Email.
*   Output difference while saving TNEF calendar items.
*   Change in content during MSG conversion.
*   Exceptions when retrieving messages from an Exchange server, saving EML to disc and loading some MSG files.

You may also visit the Public API changes section of the documentation to get an idea about the new methods included and obsolete members/methods removal from the API.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/10/aspose-Email-for-net_100.png "aspose-Email-for-net_100"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.email-for-.net/category1411.aspx
[3]: http://www.aspose.com/community/forums/aspose.email-product-family/188/showforum.aspx




