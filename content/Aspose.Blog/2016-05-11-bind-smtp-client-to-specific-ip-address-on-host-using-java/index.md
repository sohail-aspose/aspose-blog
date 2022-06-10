---
title: 'Bind SMTP Client to specific IP Address on Host using Java'
date: Wed, 11 May 2016 10:31:22 +0000
draft: false
url: /2016/05/11/bind-smtp-client-to-specific-ip-address-on-host-using-java/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-Java_100.png" alt="">}}


[Aspose.Email for Java 6.5.0][1] has been released. Ported from its equivalent .NET version, this month’s release includes the same features, enhancements and bug fixes as were included in the .NET version of the API. Specifically, the API has been enhanced to bind SmtpClient to specific IP address and the functionality of working with events on secondary calendar folder of Office 365. For a complete list of public API changes, please visit the Release Notes article in Aspose.Email for Java documentation section.

## Binding SMTP Client to Specific IP Address using Java

For a server having multiple interfaces for communicating with external world, it may sometimes be required to use a specific IP address for sending out emails. This month’s release of Aspose.Email for Java enhances the API’s SmtpClient to specify the IP address through which all the emails should be sent out.

```
SmtpClient client = new SmtpClient(
    server.SmtpUrl,
    server.SmtpPort,
    user.Name,
    user.Password,
    server.SmtpSecurityOptions);
try
{
    client.bindIPEndPoint( new BindIPEndPointHandler() {
        @Override
        public InetSocketAddress invoke(InetSocketAddress remoteEndPoint) {
            return new InetSocketAddress(0);
        }
    });
    client.noop();
}
finally { if (client != null) ((IDisposable)client).dispose(); } 
```

## Using EWS Client to Work with Secondary Calendar Folder

This month’s release introduces a new feature of working with Secondary Calendar folder on Office 365 server. This enables you to:

*   Add a secondary Calendar folder to the server
*   Create calendar events
*   Update and Delete calendar events

## Adding Mail Header at Specific Location

This month’s release also enhances the functionality of adding headers to a message’s header collection. It now provides the capability of inserting the new header at a specific location. If the collection contains headers with the same name, this header will be inserted before other headers with the same name.

## Other Improvements

This month’s release also fixes a number of bugs that were reported with the last version of the API. As the version is auto-ported from the .NET version of the API, it also inherits all the fixes from the .NET version as well.

## API Resources

We have detailed information available online for getting started with the Aspose.Email for Java API. These are:

*   [Product Documentation][2] – Provides detailed examples of working with the API
*   [API Reference Guide][3] – Details all the packages and classes of the API
*   [GitHub Examples][4] – Provides ready to run API examples
*   [Aspose.Email Forum][5] – Feel free to contact us on Aspose.Email forum for your queries




[1]: https://products.aspose.com/email/java
[2]: https://docs.aspose.com/email/net
[3]: https://apireference.aspose.com/email/net
[4]: https://github.com/aspose-email/Aspose.Email-for-Java
[5]: http://www.aspose.com/community/forums/aspose.email-product-family/188/showforum.aspx




