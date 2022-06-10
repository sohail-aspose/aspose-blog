---
title: 'Retrieving Extended Properties for Contacts Supported with Aspose.Email for .NET 16.10.0'
date: Mon, 17 Oct 2016 17:09:23 +0000
draft: false
url: /2016/10/17/retrieving-extended-properties-for-contacts-supported-with-aspose.email-for-.net-16.10.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

[![][1]](http://www.aspose.com/products/email/net)

We are pleased to announce the release of [Aspose.Email for .NET 16.10.0][2]. This month’s release enhances the capabilities of Exchange Server Client of the API for different functionalities. Specifically, this include the functionality of getting contacts information along with retrieving extended properties and querying exchange server for listing messages using specific properties. It also contains a number of improvements where the API functionality was not according to expected behavior. For a complete list of what is new and fixed, please visit the Release Notes page of the API’s latest version.

# New Features and Enhancements

**Working with Extended Properties of Contacts on Exchange Server:** This month’s release enhances the fetching contacts information from Exchange server. This provides the support for adding as well as reading Extended properties for contact items. The _Contact_ class now contains a collection of _ExtendedProperties_ that can be set and read from the fetched contacts. In order to retrieve these extended properties from the server, the request needs to be set for the Exchange client using the Extended Properties Definition. The following code shows sample example for usage of this feature.

```
IEWSClient client = EWSClient.GetEWSClient("https://outlook.office365.com/ews/exchange.asmx", "testUser", "pwd", "domain");

//The required extended properties must be added in order to create or read them from the Exchange Server
string[] extraFields = new string[] {{ "User Field 1", "User Field 2", "User Field 3", "User Field 4" }};
foreach (string extraField in extraFields)
    client.ContactExtendedPropertiesDefinition.Add(extraField);

//Create a test contact on the Exchange Server
Contact contact = new Contact();
contact.DisplayName = "EMAILNET-38433 - " + Guid.NewGuid().ToString();
foreach (string extraField in extraFields)
    contact.ExtendedProperties.Add(extraField, extraField);

string contactId = client.CreateContact(contact);

//retrieve the contact back from the server after some time
Thread.Sleep(5000);
contact = client.GetContact(contactId);

//Parse the extended properties of contact 
foreach (string extraField in extraFields)
    if (contact.ExtendedProperties.ContainsKey(extraField)) 
        Console.WriteLine(contact.ExtendedProperties[extraField].ToString()); 
```

**Listing Messages by Extended Properties:** This month’s release also enhances the functionality of listing messages from Exchange server. This refers to the modifications that help retrieve messages from server by Extended properties. This helps in filtering messages from Exchange server using specified extended properties only.

**Retrieving Extra Parameters with IMAP:** This month’s release also introduces a new feature of retrieving extra parameters using the IMAP Client API of Aspose.Email for .NET. This is sort of alternative for SendCustomCommand that was previously supported by the API. These extra parameters can be retrieved as part of summary information listed from the IMAP server. Information about these extra parameters can be retrieved for specific messages using the message’s unique id and sequence number, as well as for multiple messages based on these parameters.

# Other Improvements

As always, this month’s release also brings a number of improvements to the API functionality by fixing a number of API bugs. This further adds to the overall stability of the API.

# API Resources

The following API resources can be of help to you in getting started with Aspose.Email API.

*   Product Documentation – Provides detailed examples of working with the API
*   API Reference Guide – Details all the namespaces and classes of the API
*   [GitHub Examples][3] – Provides ready to run API example
*   [Support Forum][4] – Write to us if you have any query or inquiry about the API




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2016/09/Aspose.Email-for-.NET_.png "Aspose.Email for .NET"
[2]: http://www.aspose.com/downloads/email/net
[3]: https://github.com/asposeemail/Aspose_Email_NET
[4]: http://www.aspose.com/community/forums/aspose.email-product-family/188/showforum.aspx




