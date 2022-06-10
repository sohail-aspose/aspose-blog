---
title: 'Validate Email Messages (EML) with Aspose.Email for Java'
date: Wed, 22 Feb 2012 07:49:26 +0000
draft: false
url: /2012/02/22/validate-eml-messages-with-aspose.email-for-java-2/
author: Babar Raza
summary: ''
tags: ['Aspose', 'EmlValidationError', 'Home', 'MailMessage', 'Validate', 'email', 'eml', 'java', 'report']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose.email-logo120.jpg" alt="Validate Email Messages">}}


Aspose.Email for Java 1.4.0 has been released. This release includes the latest improvements made to the Aspose.Email for Java component.

An attractive feature of Aspose.Email is the ability to validate EML. The MailMessage class has exposed a new static method, ValidateMessage, that accepts an EML file through a file path or as a stream and returns an object of EmlValidationErrorCollection. If the returned collection is empty then no validation problems have been detected. Else, you may parse the collection to retrieve EmlValidationError objects. You can also inspect the cause of validation failure by using EmlValidationError class members like getErrorMessage(), getErrorType() and getLineNumber().

To download the release, [please visit the download area][1].

As usual, we can answer any questions you have in the product [forum][2].

Enjoy!




[1]: http://www.aspose.com/community/forums/aspose.email-product-family/188/showforum.aspx
[2]: https://www.aspose.com/templates/aspose/App_Themes/V3/images/words/272x272/aspose_words-for-net.png




