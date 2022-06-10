---
title: 'Aspose.Email for Java 4.6.0 Supports Spam Message Analysis and Filtering'
date: Mon, 13 Oct 2014 14:04:54 +0000
draft: false
url: /2014/10/13/aspose.email-for-java-supports-spam-message-analysis-and-filtering/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

![](https://blog.aspose.com/wp-content/uploads/sites/2/2014/10/aspose-Email-for-Java_100.png "aspose-Email-for-Java_100")Following the latest release of Aspose.Email for .NET, we are now pleased to announce the release of Aspose.Email for Java 4.6.0 that comes with a number of enhancements and bug fixes. Similar to the equivalent .NET version, this month’s release introduces new features that let you filter spam email messages based on the naive Bayes classifiers. It also brings improvements to the size of generated PSTs. To get a complete idea of what is new, improved and fixed, please visit the [product download page][1]. The public API changes are listed in the documentation with all the changes in this latest version.

## Spam Email Analysis and Filtering

The naive Bayes classifier offers a high accuracy anti-spam message classification and provides an effective measure for distinguishing between spam and ham (non-spam) messages. This month’s release of Aspose.Email for Java introduces this new feature of spam analysis and filtering using the same proven method. Aspose.Email for Java now offers to spam analyzer to filter spam messages. The process includes the following steps to achieve this:

**Training the Filter:** This step is carried out on data sets of spam and ham messages for training the filter. Normally, a set of 100-200 messages each is used for this purpose. Once the sets are ready, the API’s SpamAnalyzer class is used to train the filter with both these sets as inputs.

**Saving the Results:** Once the training is complete, the results of the trained classifiers can be stored to disc calling the _saveDatabase_ method of the class.

**Testing:** Testing is carried out by presenting sample messages to the test method of the class. Based on the training results, the tests provide the probability of a message being spam or ham.

For working code sample, refer to the example article in the online documentation: Working with Bayesian Spam Analyzer.

## Improvement in Generated PST Size

We have also improved the size of PSTs that are generated using the Aspose.Email API. The PSTs created now are almost 25% smaller in size compared to the previous versions. We are still working to bring further improvements to this area.

## Bug Fixes

Ported from the .NET version, this month’s release includes the same bug fixes:

*   Issues with message encodings when converting between different message types.
*   Exceptions when loading certain message files and calendar items.
*   Information loss when processing TNEF files.
*   Text alignment issues when loading/saving calendar items.




[1]: http://www.aspose.com/community/files/72/java-components/aspose.email-for-java/default.aspx




