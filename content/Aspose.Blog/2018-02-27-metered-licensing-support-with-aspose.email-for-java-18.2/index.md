---
title: 'Metered Licensing Support in Aspose.Email for Java 18.2'
date: Tue, 27 Feb 2018 13:07:35 +0000
draft: false
url: /2018/02/27/metered-licensing-support-with-aspose.email-for-java-18.2/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-Java_100.png" alt="">}}


[Aspose.Email for Java 18.2][1] has been released. This release introduces the support for Metered Licensing using the Aspose.Email for Java API. It also provides fixes for user’s issues reported issues with the previous version of the API. For a detailed note on what is new and fixed, please visit the [release notes][2] section of API.

## Use Metered License with Aspose.Email for Java

We are glad to share the support for Metered Licensing in Aspose.Email for Java API. For those who are new to the term “Metered Licensing”, it is a form of consumptive licensing for which you pay royalties for the use of product every month. You can also visit the [Metered Licensing FAQs][3] section to know more about this type of licensing.

### Using the Metered Licensing in API

Usage of Metered Licensing scheme is simple and can be used along with existing licensing method. The new licensing mechanism will be used along with existing licensing method. Those customers who want to be billed based on the usage of the API features can use the metered licensing. 

```
Metered metered = new Metered();
// Access the SetMeteredKey property and pass public and private keys as parameters
metered.setMeteredKey("*****", "*****");

// The path to the documents directory. 
String dataDir = Utils.getSharedDataDir(DisplayEmailInformation.class) + "email/";

// Load the document from disk.
MailMessage eml = MailMessage.load(dataDir + "test.eml");
//Get the page count of document
System.out.println(eml.getSubject()); 
```

## API Resources

We have detailed information available online for getting started with the Aspose.Email for Java API. These are:

*   [Product Documentation][4] – Provides detailed examples of working with the API
*   [API Reference Guide][5] – Details all the packages and classes of the API
*   [GitHub Examples][6] – Provides ready to run API examples
*   [Aspose.Email Forum][7] – Feel free to contact us on Aspose.Email forum for your queries




[1]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-email/
[2]: https://docs.aspose.com/display/emailjava/Aspose.Email+for+Java+18.2+Release+Notes
[3]: https://purchase.aspose.com/faqs/licensing/metered
[4]: https://docs.aspose.com/display/emailjava/Home
[5]: http://www.aspose.com/api/java/email
[6]: https://github.com/aspose-email/Aspose.Email-for-Java
[7]: https://forum.aspose.com/c/email




