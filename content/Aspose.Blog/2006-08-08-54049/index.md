---
title: 'Aspose.Network 3.0 Beta Available'
date: Tue, 08 Aug 2006 13:18:00 +0000
draft: false
url: /2006/08/08/54049/
author: Iret
summary: ''
tags: ['Kyle Huang']
---

Dear Customers,

**Aspose.Network 3.0 Beta **, version 3.0.0.0807, is available. 

**What's New in Aspose.Network** **3.0 Beta**

*   High compatible with .NET 2.0 E-Mail APIs, and Work fine under **.NET 1.1 and .NET 2.0** frameworks. Therefore, .NET developers can easily migrate their E-Mail applications.
    
    **Example code**  
    // Command line argument must the the SMTP host.  
    SmtpClient client = new SmtpClient("localhost", "test001", "test");  
    // Specify the e-mail sender.  
    // Create a mailing address that includes a UTF8 character  
    // in the display name.  
    MailAddress from = new MailAddress("test001@aspose.com",  
    "Jane " + (char)0xD8 + " Clayton");  
    // Set destinations for the e-mail message.  
    MailAddress to = new MailAddress("test002@aspose.com");  
    // Specify the message content.  
    MailMessage message = new MailMessage(from, to);  
    message.TextBody = "This is a test e-mail message sent by an application. ";  
    // Include some non-ASCII characters in body and subject.  
    string someArrows = new string(new char\[\] { '\\u2190', '\\u2191', '\\u2192', '\\u2193' });  
    message.TextBody += Environment.NewLine + someArrows;  
    message.BodyEncoding = System.Text.Encoding.UTF8;  
    message.Subject = "test message 1" + someArrows;  
    message.SubjectEncoding = System.Text.Encoding.UTF8;  
    // Set the method that is called back when the send operation ends.  
    client.SendCompleted += new  
    SendCompletedEventHandler(SendCompletedCallback);  
    // The userState can be any object that allows your callback  
    // method to identify this send operation.  
    // For this example, the userToken is a string constant.  
    string userState = "test message1";  
    client.SendAsync(message, userState);
    
*   **Unique** **Object Model** for E-Mail creating and parsing functions. The MailMessage class provides the unique and simple entry for creating and parsing E-Mail messages.
    
    **Example**  
    //Load eml format file to MailMessage instance  
    MailMessage message = MailMessage.Load(@"../message.eml");  
    SmtpClient client = new SmtpClient("localhost","test001", "test");  
    //Send the message via Smtp  
    client.SendAsync(message);
    
*   **Stronger MailMerge** features due to new template rendering engine.  
*   **Higher performance** in Bulk Send E-Mail messages.
*   **Parse Mhtml format file** (.mht), **Load Mhtml format** file to MailMessage instance.
*   **Parse Eml format file** (.eml), **Load eml format** file to MailMessage instance.
    
*   **Parse Msg format file** (.msg), **Load Msg format** file to MailMessage instance.

**HowTo get Beta and support**

*   Download the beta from the attachment .net 1.1 built here / .NET 2.0 built [here][1] 
*   Send E-Mail to [guangzhou@aspose.com][2] asking for beta or support.

**Other Changes**

*   API changes in Mail components, to provide compatible with .NET 2.0 E-Mail APIs
*   Other API changes in Pop3 and Imap components, to provide sameness interfaces and object models.

**Known Issues**

*   **No Backward Compatibility** in Aspose.Network 3.0. Aspose.Network 3.0 does not provide backward compatibility with Aspose.Network 2.\*. However, We will provide technical supports and hotfixes for any known bugs.
*   The breaking APIs Only affect the Mail components, **Aspose.Network.Mail**, **Aspose.Network.Pop3**,  and **Aspose.Network.Imap**. **Other namespaces will keep their backward compatibility.***   This Beta release for Aspose.Network is for the community reviewing and feedbacks. **It will keep compatible with the official release later**. Therefore, if Aspose.Network is new for you, Please use the Beta version for your evaluation and development. And if you are willing to migrate the Old Aspose.Network apps to New one, we will be more than glad to provide any help we can.
*   The demos / samples /documents for Aspose.Network 3.0 will be provided ASAP.
*   Any feedbacks and idea is Welcome for this beta release.

Thanks.




[1]: /products/aspose.network/releases/Aspose.Network3betaforNET2.zip
[2]: mailto:guangzhou@aspose.com



