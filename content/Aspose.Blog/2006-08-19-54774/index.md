---
title: 'Aspose.Network 3.0.0.0 Released'
date: Sat, 19 Aug 2006 00:16:00 +0000
draft: false
url: /2006/08/19/54774/
author: Iret
summary: ''
tags: ['Kyle Huang']
---

**Aspose.Network 3.0** is the next major official release version of our comprehensive network programming components. 

**Here is what's new in Aspose.Network** **3.0:**

*   **Unique** **Object Model** for E-Mail creating and parsing functions. The MailMessage class provides the unique and simple entry for creating and parsing E-Mail messages.
    **Example**  
    //Load outlook message format file (\*.msg) to MailMessage instance  
    MailMessage message = MailMessage.Load(@"../message.msg", MessageFormat.Msg);  
    SmtpClient client = new SmtpClient("localhost","test001", "test");  
    //Send the message via Smtp  
    client.SendAsync(message);
*   **Enhanced IMAP component** for adding more functions and tuning performance.
*   **Improved POP3 component** for adding more functions and tuning performance.
*   Supports loading and parsing **Microsoft Outlook E-Mail Message Format** (\*.Msg). Aspose.Network 3.0 is the **FIRST** .NET component provides the function to parse the Outlook message file.
*   Supports loading and parsing **Microsoft Html Format** file (\*.mht). Aspose.Network 3.0 can load a mht file and send it out through SMTP server.
*   Supports loading and parsing **RFC 822 compliant Email Message Format** file (\*.eml), and send it out through SMTP server.
*   **High compatible** with .NET 2.0 E-Mail APIs, and Work fine under **.NET 1.1 and .NET 2.0** frameworks. Therefore, .NET developers can easily migrate their E-Mail applications to Aspose.Network.
    **Example code**  
      
    // Command line argument must the SMTP host.  
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

*   **Sophisticated Template-based MailMerge** features due to new template rendering engine.
    
    *   Aspose.Network 3.0 supports generate E-Mail messages from **DataTable**, **DataRow** and **DataReader**
    *   The template could be a run-time **MailMessage instance** and **Eml format file**.
    *   Aspose.Network 3.0 supports template merge against a runtime MailMessage, which can be use to add extra format info the E-Mail message like pre-defined signature in the Microsoft Outlook.*   Aspose.Nework is the **FIRST** .NET component that supports to use User defined function in the E-Mail template. With using function field in the template, we can easily do lots of amazing things like provide unique signature and ect.
    
      
    **           Example code**
    
    //template routine to provide signature  
    static object GetSignature(object\[\] args)  
    {  
    return "John Smith<br>Product Lead<br>Aspose Ltd.<br>" + DateTime.Now.ToShortDateString();  
    }  
      
    static void Main(string\[\] args)  
    {  
      
    //create a new MailMessage instance as a template  
    MailMessage template = new MailMessage();  
      
    //add template field to subject  
    template.Subject = "Hello, #FirstName#";  
    template.From = "sale@aspose.com";  
      
    //add template field to receipt  
    template.To.Add(new MailAddress("#Receipt#", false));  
      
    //add template field to html body  
    //use GetSignment as the template routine, which will provide the same signature.  
    template.HtmlBody = "Dear #FirstName# #LastName#,<br><br>";  
    template.HtmlBody += "Thank you for your interest in <STRONG>Aspose.Network</STRONG>.";  
    //use user-defined routine  
    template.HtmlBody += "<br><br>Have fun with it.<br><br>#GetSignature()#";  
      
    //create a new TemplateEngine with the template message.  
    TemplateEngine engine = new TemplateEngine(template);  
      
    //register the GetSignment as a templat routine, for we use it in the template.  
    engine.RegisterRoutine("GetSignature", new TemplateRoutine(GetSignature));  
      
    //fill a DataTable as data source  
    DataTable dt = new DataTable();  
    dt.Columns.Add("Receipt", typeof(string));  
    dt.Columns.Add("FirstName", typeof(string));  
    dt.Columns.Add("LastName", typeof(string));  
      
    DataRow dr;  
    dr = dt.NewRow();  
    dr\["Receipt"\] = "Nancy.Davolio<Nancy@somedomain.com>";  
    dr\["FirstName"\] = "Nancy";  
    dr\["LastName"\] = "Davolio";  
    dt.Rows.Add(dr);  
    dr = dt.NewRow();  
    dr\["Receipt"\] = "Andrew.Fuller<Andrew@somedomain.com>";  
    dr\["FirstName"\] = "Andrew";  
    dr\["LastName"\] = "Fuller";  
    dt.Rows.Add(dr);  
    dr = dt.NewRow();  
    dr\["Receipt"\] = "Janet.Leverling<Janet@somedomain.com>";  
    dr\["FirstName"\] = "Janet";  
    dr\["LastName"\] = "Leverling";  
    dt.Rows.Add(dr);  
      
    MailMessageCollection messages;  
    try  
    {  
    //create the messages from the template and datasource.  
    messages= engine.Instantiate(dt);  
    SmtpClient client = new SmtpClient("smtp.somedomain.com", 25, "someone","password");  
    //bulk send the message  
    client.BulkSendAsync(messages);  
    }  
    catch (MailException ex)  
    {  
    System.Diagnostics.Debug.WriteLine(ex.ToString());  
    }  
    catch (SmtpException ex)  
    {  
    System.Diagnostics.Debug.WriteLine(ex.ToString());  
    }  
      
    }
    
*   **Higher performance** in Bulk Send E-Mail messages. Aspose.Network 3.0 provides high performance multi-threading and thread pool to improve the bulk sending emails.

**HowTo Aspose.Network and Technical Support**

*   Download the Aspose.Network 3.0 here
*   Online support forum 
*   E-Mail support : [guangzhou@aspose.com][1] 
*   [Online Demo][2]

**Other Changes**

*   API changes in Aspose.Network.Mail, Aspose.Network.Mime namespaces, to provide compatible with .NET 2.0 E-Mail APIs
*   API changes in Pop3 and Imap components, to provide sameness interfaces and object models.

**Known Issues**

*   **No Backward Compatibility** in Aspose.Network 3.0. Aspose.Network 3.0 does not provide backward compatibility with Aspose.Network 2.\*.*   The breaking APIs Only affect the Mail components, **Aspose.Network.Mail**, **Aspose.Network.Pop3**,  and **Aspose.Network.Imap**. **Other namespaces will keep their backward compatibility.**
*   **Aspose.Network 2.\* will be continuously maintained and supported**. We will provide technical supports and hotfixes for any existing bugs.

**Questions:**

> **Should I migrate the existing code to Aspose.Network 3.0?**
> 
> *   If you are new starter for Aspose.Network, Please use the Aspose.Network 3.0 for your evaluation and development.  
>     However, if you already using the old version of Aspose.Network, you can just keep the existing code without any changes. We will keep to support the old version of Aspose.Network.  
>     But we strongly suggest that you port the existing to the latest version, which can buy you more amazing features.

> **Can I get the help from product development for the code migration?**
> 
> *   Yes, We are more than glad to help provide any help. Just post you concerns on the technical support forum, our support engineer will response within 24 hour. 
> 
> **Does Aspose.Network 3.0 support .NET 2.0?**
> 
> *   Yes, we released a built on .NET 1.1, which can run under .NET 2.0. And the .NET 2.0 build will be also released the days to come.
> 
> **What's the most effective way to get technical support?**
> 
> *   Technical question can be posted to our support forum, this is the most effective ways to get supports. And other support ways: Email support: [guangzhou@aspose.com][3], IM support: guangzhou@aspose.com




[1]: mailto:guangzhou@aspose.com
[2]: /Products/Aspose.Network/Demos/
[3]: mailto:guangzhou@aspose.com



