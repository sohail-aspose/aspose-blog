---
title: 'Working with MSG and VCF Contacts using C++'
seoTitle: "Working with MSG and VCF Contacts using C++ | Outlook Contacts"
description: "Work with MSG and VCF contacts using C++. Learn how to create, read and modify MSG and VCF contacts within your C++ applications."
date: Wed, 28 Apr 2021 11:39:08 +0000
draft: false
url: /2021/04/28/working-with-msg-and-vcf-contacts-using-cpp/
author: Muhammad Ahmad
summary: 'Contacts are an essential part of any email client as they facilitate the user by remembering all their contacts, similar to the contacts on your smartphone. Outlook contacts store a lot of information regarding a person, such as their name, address, contact number, email address, etc. These contacts can be stored in [MSG][1] and [VCF][2] formats. You might find yourself in scenarios where you need to create or alter MSG or VCF contacts programmatically. For that, this article will teach you **how to work with MSG and VCF** **contacts using C++**.'
tags: ['Create MSG Contact C++', 'Create VCF Contact C++', 'Modify MSG Contact C++', 'Modify VCF Contact C++', 'Read MSG Contact C++', 'Read VCF Contact C++']
categories: ['Aspose.Email Product Family']
---

Contacts are an essential part of any email client as they facilitate the user by remembering all their contacts, similar to the contacts on your smartphone. Outlook contacts store a lot of information regarding a person, such as their name, address, contact number, email address, etc. These contacts can be stored in [MSG][3] and [VCF][4] formats. You might find yourself in scenarios where you need to create or alter MSG or VCF contacts programmatically. For that, this article will teach you **how to work with MSG and VCF** **contacts using [C++][5]**.

*   [C++ API for Working with MSG and VCF Contacts][6]
*   [Create MSG and VCF Contacts][7]
*   [Read MSG and VCF Contacts][8]
*   [Modify MSG and VCF Contacts][9]
*   [Get a Free License][10]

## C++ API for Working with MSG and VCF Contacts {#CPP-API-for-Working-with-MSG-and-VCF-Contacts}

[Aspose.Email for C++][11]??is a native C++ library for creating, manipulating, and sending emails without requiring Microsoft Outlook to be installed. The API also supports working with contacts and calendars. You can either install the API through??[NuGet][12]??or download it directly from the??[Downloads][13]??section.

```
PM> Install-Package Aspose.Email.Cpp
```

## Create MSG and VCF Contacts {#Create-MSG-and-VCF-Contacts}

In this section, you will learn how to create an Outlook contact and save it in MSG and VCF format. The following are the steps to achieve that.

*   Create an instance of the [MapiContact][14] class.
*   Set the properties of the contact such as the Name, Address, Telephone, etc.
*   Save the contact using the [MapiContact->Save(System::String filePath, Aspose::Email::Mapi::ContactSaveFormat saveFormat)][15] method.

The following sample code demonstrates how to create an Outlook contact and save it in MSG and VCF format using C++.

{{< gist aspose-com-gists 1d5dbf0eb9b255417cefc38475b16b91 "Create-Outlook-Contact.cpp" >}}



{{< figure align=center src="images/CreateContactEmailCpp-1024x537.png" alt="Contact generated by the sample code" caption="Contact generated by the sample code">}}


## Read MSG and VCF Contacts {#Read-MSG-and-VCF-Contacts}

Aspose.Email for C++ supports reading contacts in both MSG and VCF formats. Here, you will see how to open MSG and VCF contacts using C++.

*   [Read MSG Contact][16]
*   [Open VCF Contact][17]

### Read MSG Contact {#Read-MSG-Contact}

The following are the steps to read an MSG contact.

*   Load the contact using the [MapiMessage][18] class.
*   Convert [MapiMessage][19] to [IMapiMessageItem][20] using the [MapiMessage->ToMapiMessageItem()][21] method and cast it to [MapiContact][22].
*   Read the properties of the contact.

The following is the sample code to read an MSG contact using C++.

{{< gist aspose-com-gists 1d5dbf0eb9b255417cefc38475b16b91 "Read-MSG-Contact.cpp" >}}

### Open VCF Contact {#Open-VCF-Contact}

To read a VCF contact, simply load the contact using the [MapiContact::FromVCard][23] method. The following sample code shows how to read a VCF contact using C++.

{{< gist aspose-com-gists 1d5dbf0eb9b255417cefc38475b16b91 "Read-VCF-Contact.cpp" >}}

## Modify MSG and VCF Contacts {#Modify-MSG-and-VCF-Contacts}

In order to modify an MSG/VCF contact, open the contact as demonstrated in the previous section and then change its properties. The following are the steps to modify contacts.

*   Load the MSG/VCF contact as shown in the [Read MSG and VCF Contacts][24] section.
*   Change the desired properties of the contact.
*   Save the contact using the [MapiContact->Save(System::String filePath, Aspose::Email::Mapi::ContactSaveFormat saveFormat)][25] method.

The following sample code demonstrates how to modify MSG/VCF contacts using C++.

{{< gist aspose-com-gists 1d5dbf0eb9b255417cefc38475b16b91 "Modify-Outlook-Contact.cpp" >}}

## Get a Free License {#Get-a-Free-License}

You can try the API without evaluation limitations by requesting??[a free temporary license][26].

## Live Demo

*   [Email Metadata][27]

## Conclusion

In this article, you have learned how to work with MSG and VCF contacts using C++. Specifically, you have learned how to create, read and modify contacts using Aspose.Email for C++ API. The API provides a bunch of additional features for automating your email-related tasks. You can explore the API in detail by visiting the??[official documentation][28]. If you have any questions, please feel free to reach us on our??[free support forum][29].

## See Also

*   [Convert Email Messages to PDF using C++][30]
*   [Read Email Messages using C++][31]




[1]: https://docs.fileformat.com/email/msg/
[2]: https://docs.fileformat.com/email/vcf/
[3]: https://docs.fileformat.com/email/msg/
[4]: https://docs.fileformat.com/email/vcf/
[5]: https://docs.fileformat.com/programming/cpp/
[6]: #CPP-API-for-Working-with-MSG-and-VCF-Contacts
[7]: #Create-MSG-and-VCF-Contacts
[8]: #Read-MSG-and-VCF-Contacts
[9]: #Modify-MSG-and-VCF-Contacts
[10]: #Get-a-Free-License
[11]: https://products.aspose.com/email/cpp
[12]: https://www.nuget.org/packages/Aspose.Email.Cpp
[13]: https://downloads.aspose.com/email/cpp
[14]: https://apireference.aspose.com/email/cpp/class/aspose.email.mapi.mapi_contact
[15]: https://apireference.aspose.com/email/cpp/class/aspose.email.mapi.mapi_contact#a285e3b88074f7e98168f90c06c9545ce
[16]: #Read-MSG-Contact
[17]: #Open-VCF-Contact
[18]: https://apireference.aspose.com/email/cpp/class/aspose.email.mapi.mapi_message
[19]: https://apireference.aspose.com/email/cpp/class/aspose.email.mapi.mapi_message
[20]: https://apireference.aspose.com/email/cpp/class/aspose.email.mapi.i_mapi_message_item
[21]: https://apireference.aspose.com/email/cpp/class/aspose.email.mapi.mapi_message#a4b5a7ec1af1b48ab7dc62400a91029a0
[22]: https://apireference.aspose.com/email/cpp/class/aspose.email.mapi.mapi_contact
[23]: https://apireference.aspose.com/email/cpp/class/aspose.email.mapi.mapi_contact#a1c8336426e6dc8a98ca0675a08f79e24
[24]: #Read-MSG-and-VCF-Contacts
[25]: https://apireference.aspose.com/email/cpp/class/aspose.email.mapi.mapi_contact#a285e3b88074f7e98168f90c06c9545ce
[26]: https://purchase.aspose.com/temporary-license
[27]: https://products.aspose.app/email/metadata
[28]: https://docs.aspose.com/email/cpp/
[29]: https://forum.aspose.com/c/email/12
[30]: https://blog.aspose.com/2021/02/13/convert-email-messages-to-pdf-using-cpp/
[31]: https://blog.aspose.com/2021/04/22/read-email-messages-using-cpp/





