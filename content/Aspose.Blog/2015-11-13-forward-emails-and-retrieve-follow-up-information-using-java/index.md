---
title: 'Forward Emails and Retrieve Follow-Up Information from Messages using Java'
date: Fri, 13 Nov 2015 15:31:47 +0000
draft: false
url: /2015/11/13/forward-emails-and-retrieve-follow-up-information-using-java/
author: Muhammad Waqas
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-Java_100.png" alt="">}}


We are pleased to announce the release of [Aspose.Email for Java 5.9.0][1]. This month’s release includes a number of enhancements related to the API's communication clients and further improves the API functionality by fixing a number of bugs. Our documentation article, Public API changes in Aspose.Email for Java 5.9.0, lists all the changes that are part of this month’s release.

## Forwarding Emails using SMTP in Java

This month’s release enhances the functionality of API’s SmtpClient by providing the facility of forwarding email messages to specific recipients. This provides the capability to send a received message to desired recipients.

## Accessing Follow-Up Information from Message in Java

Messages received as acknowledgment to sender’s requests contain information such as delivery notification, read receipt delivery time, voting results and vote submission time. This month’s release provides new Mapi Properties for retrieving such information from received messages. These properties are:

*   PR\_RECIPIENT\_TRACKSTATUS\_TIME\_DELIVERY
*   PRRECIPIENT\_TRACKSTATUS\_TIME\_READ
*   PR\_RECIPIENT\_AUTORESPONSE\_PROP\_RESPONSE
*   PR\_RECIPIENT\_TRACKSTATUS\_TIME

And can be retrieved as shown in our documentation article, Accessing FollowUp Information from Message.

## Getting Copied Message URI using EWS

The EWSClient of Aspose.Email API provides the capability to copy a message from one Exchange folder to another Exchange folder. This month’s release further enhances this method so as to return the copied message’s unique identifier that was not available earlier. More Info

## Other Improvements

This month’s release also fixes a number of bugs that were reported with our last month’s release. A complete list of issues, that are fixed as part of this month’s release, can be viewed by visiting our [product download page][2].

## API Resources

We have detailed information available online for getting started with the Aspose.Email for Java API. These are:

*   [Product Documentation][3] – Provides detailed examples of working with the API
*   [API Reference Guide][4] – Details all the packages and classes of the API
*   [GitHub Examples][5] – Provides ready to run API examples
*   [Aspose.Email Forum][6] – Feel free to contact us on Aspose.Email forum for your queries




[1]: https://products.aspose.com/email/java
[2]: https://downloads.aspose.com/email/java
[3]: https://docs.aspose.com/email/java
[4]: https://apireference.aspose.com/email/java
[5]: https://github.com/aspose-email/Aspose.Email-for-Java
[6]: http://www.aspose.com/community/forums/aspose.email-product-family/188/showforum.aspx




