---
title: 'Access SSL Enabled SMTP Server (Gmail) via Aspose.Network for .NET'
date: Wed, 06 Feb 2008 21:43:00 +0000
draft: false
url: /2008/02/06/accessing-gmail-via-aspose-network-ssl/
author: Saqib Razzaq
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

In this article, we will show you how to access Gmail via SSL. We can access gmail using following protocols:   

*   **SMTP**
*   **IMAP**
*   **POP3 **

#### SMTP

In this section we will show you how to perform various tasks on Gmail server using SMTP protocol on SSL.  
  

**Connect to Gmail SMTP server**

The following example shows you how you can connect to SSL enabled SMTP server. We will set the following properties for SSL support:

First, create a new **SmtpClient** object as follows:

\[C#\]

Aspose.Network.Mail.SmtpClient client = new SmtpClient("smtp.gmail.com");

\[VB.Net\]

Dim client As Aspose.Network.Mail.SmtpClient = New SmtpClient("smtp.gmail.com")

We have passed **smtp.gmail.com** in the constructor which is the smtp server address of Gmail. Now, set the following properties which are necessary to connect to any SSL enabled mail server.

\[C#\]

// set your Gmail username  

client.Username = "user@gmail.com";  

// set you Gmail password  

client.Password = "pwd";  

// set the port to 587. This is the SSL port of Gmail SMTP server  

client.Port = 587;  

// set the security mode to explicit  

client.SecurityMode = SmtpSslSecurityMode.Explicit;  

// enable SSL  

client.EnableSsl = true;  
  

\[VB.Net\]  
  

set your Gmail username  

client.Username = "user@gmail.com"  

' set you Gmail password  

client.Password = "pwd"  

' set the port to 587. This is the SSL port of Gmail SMTP server  

client.Port = 587  

' set the security mode to explicit  

client.SecurityMode = SmtpSslSecurityMode.Explicit  

' enable SSL  

client.EnableSsl = True  
  

**Send an email message**  
  

So far, we have setup the SMTP client object to connect to the Gmail server. To send a message using the above **client** object, we need to create a **MailMessage** object and send the message using SmtpClient object.  
  

\[C#\]  
  

Aspose.Network.Mail.MailMessage msg = new MailMessage();  
  

\[VB.Net\]  
  

Dim msg As Aspose.Network.Mail.MailMessage = New MailMessage()  
  

Set the properties of the message e.g. subject, to, body as follows:  
  

\[C#\]  
  

// from whom   

msg.From = new Aspose.Network.Mail.MailAddress("user@gmail.com");  
  

// to whom  

msg.To.Add( new Aspose.Network.Mail.MailAddress( "user@gmail.com" ) );  
  

// set the subject  

msg.Subject = "subject";  
  

// set the priority  

msg.Priority = Aspose.Network.Mail.MailPriority.High;  
  

// set the message bodies  

msg.TextBody = "Please open with html browser";  

msg.HtmlBody = "<bold>this is the mail body</bold>";  
  

// add the attachment  

Aspose.Network.Mail.Attachment attachment = new Attachment(@"c:\\File.txt");  

msg.Attachments.Add(attachment);  
  

try  

{  

// send the message  

client.Send(msg);  

}  

// catch exception  

catch( SmtpException ex )  

{  

System.Diagnostics.Trace.WriteLine( ex.ToString() );  

}  
  

\[VB.Net\]  
  

' from whom  

msg.From = New Aspose.Network.Mail.MailAddress("user@gmail.com")  
  

' to whom  

msg.To.Add(New Aspose.Network.Mail.MailAddress("user@gmail.com"))  
  

' set the subject  

msg.Subject = "subject"  
  

' set the priority  

msg.Priority = Aspose.Network.Mail.MailPriority.High  
  

' set the message bodies  

msg.TextBody = "Please open with html browser"  

msg.HtmlBody = "<bold>this is the mail body</bold>"  
  

' add the attachment  

Dim attachment As Aspose.Network.Mail.Attachment = New Attachment("c:\\File.txt")  

msg.Attachments.Add(attachment)  
  

Try  

    ' send the message  

    client.Send(msg)  

Catch ex As SmtpException  

    ' catch exception  

    System.Diagnostics.Trace.WriteLine(ex.ToString())  

End Try  
  

#### IMAP

In this section we will perform some activities on SSL enabled mail server using IMAP protocol.  
  

**Connect to the Mail Server**  
  

We will use **ImapClient** object of Aspose.Network to connect to the mail server. Server’s address, port, username and password are required for the connection to be established. Gmail uses port 993 for IMAP protocol, so in our example below we will connect to gmail using the same port.  
  

**Example:**  
  

\[C#\]  
  

// connect to gmail server  

Aspose.Network.Imap.ImapClient imap = new Aspose.Network.Imap.ImapClient("imap.gmail.com", 993, "user@gmail.com", "pwd");  

imap.EnableSsl = true; // enable the SSL  

imap.SecurityMode = Aspose.Network.Imap.ImapSslSecurityMode.Implicit; // set security mode  

imap.Connect(true); // connect and login  
  

\[VB.Net\]  
  

' connect to gmail server  

Dim imap As New Aspose.Network.Imap.ImapClient("imap.gmail.com", 993, "user@gmail.com", "pwd")  

imap.EnableSsl = True  

' enable the SSL  

imap.SecurityMode = Aspose.Network.Imap.ImapSslSecurityMode.Implicit  

' set security mode  

imap.Connect(True)  

' connect and login  
  

**Select Inbox folder and get total number of messages**  
  

Checking Inbox is the most frequent task when you check your email. Using Aspose, this can be done using just 2 simple lines of code.  
  

**Example:**  
  

\[C#\]  
  

// select the Inbox folder  

imap.SelectFolder(ImapFolderInfo.InBox);  

//gets number of messages in the folder  

Console.WriteLine(imap.CurrentFolder.TotalMessageCount + " messages found.");  
  

\[VB.Net\]  
  

' select the Inbox folder  

imap.SelectFolder(ImapFolderInfo.InBox)  

'gets number of messages in the folder  

Console.WriteLine(imap.CurrentFolder.TotalMessageCount + " messages found.")  
  

**Saving messages to your local hard drive**  
  

Once we select some folder using **SelectFolder** method, we can use **ListMessages** function to get the list of all the messages in that folder in an **ImapMessagesInfoCollection** object. We can iterate through this collection and save email messages to the local drive of computer as follows:  
  

**Example:**  
  

\[C#\]  
  

//gets the message info collection  

ImapMessageInfoCollection list = imap.ListMessages();  

//download each message  

for (int i = 0; i < list.Count; i++)  

{  

   // save the message as eml file  

   imap.SaveMessage(list\[i\].UniqueId, list\[i\].UniqueId + ".eml");  

}  
  

\[VB.Net\]  
  

'gets the message info collection  

Dim list As ImapMessageInfoCollection = imap.ListMessages()  

'download each message  

For i As Integer = 0 To list.Count - 1  

    ' save the message as eml file  

    imap.SaveMessage(list(i).UniqueId, list(i).UniqueId + ".eml")  

Next  
  

**Create a new folder**  
  

IMAP protocol also allows you to create a new folder on the email server for categorization of emails and store them in the appropriate folders. This can be done using a simple function call.  
  

**Example:**  
  

\[C#\]  
  

imap.CreateFolder("NewFolder");  
  

\[VB.Net\]  
  

imap.CreateFolder("NewFolder")  
  

**Create a New message in a folder**  
  

You can add a new message to the folder using the **MailMessage** and **ImapClient** class. We will create a MailMessage object first by providing subject, to and from. And then subscribe to a folder and add the message to it.  
  

**Example:**  
  

\[C#\]  
  

// create a message  

Aspose.Network.Mail.MailMessage msg;  

   msg = new Aspose.Network.Mail.MailMessage(  

   "user@gmail.com",  

   "user@gmail.com",  

   "subject",  

   "message"  

);  
  

// subscribe to the currently selected folder which was Inbox in previous example  

imap.SubscribeFolder(imap.CurrentFolder.Name);  
  

// append the newly created message  

imap.AppendMessage(imap.CurrentFolder.Name, msg);  
  

\[VB.Net\]  
  

' create a message  

Dim msg As Aspose.Network.Mail.MailMessage  

msg = New Aspose.Network.Mail.MailMessage("user@gmail.com", "user@gmail.com", "subject", "message")  
  

' subscribe to the currently selected folder which was Inbox in previous example  

imap.SubscribeFolder(imap.CurrentFolder.Name)  
  

' append the newly created message  

imap.AppendMessage(imap.CurrentFolder.Name, msg)  
  

#### Pop3

In this section, we will show some examples that use Pop3 protocol on SSL. For SSL, we need to define the SSL port and 2 extra properties. Rest is same as connecting to normal Pop3 servers. We will start with making a connection to the mail server.  
  

**Connecting to Mail server**  
  

We will connect to the SSL enabled mail server using the same Pop3Client class as follows:  
  

**Example:**  
  

\[C#\]  
  

// create a pop3 client  

Aspose.Network.Pop3.Pop3Client client;  

client = new Aspose.Network.Pop3.Pop3Client();  
  

// basic setings (required)  

client.Host = "pop.gmail.com";  

client.Username = "user@gmail.com";  

client.Password = "pwd";  

client.Port = 995; // set SSL port  
  

// Settings required for SSL enabled Pop3 servers  

client.SecurityMode = Aspose.Network.Pop3.Pop3SslSecurityMode.Implicit; // set implicit security mode  

client.EnableSsl = true; // enable SSL  
  

client.Connect(); // establish a connection  

client.Login(); // login  
  

\[VB.Net\]  
  

' create a pop3 client  

Dim client As Aspose.Network.Pop3.Pop3Client  

client = New Aspose.Network.Pop3.Pop3Client()  
  

' basic setings (required)  

client.Host = "pop.gmail.com"  

client.Username = "user@gmail.com"  

client.Password = "pwd"  

client.Port = 995 ' set SSL port  
  

' Settings required for SSL enabled Pop3 servers  

client.SecurityMode = Aspose.Network.Pop3.Pop3SslSecurityMode.Implicit ' set implicit security mode  

client.EnableSsl = True ' enable SSL  
  

client.Connect() ' establish a connection  

client.Login() ' login  
  

**Check the mailbox status**  
  

In this example, we will check the number of messages that are stored in the mailbox and the size of the mailbox. We will use **Pop3MailboxInfo** class for this purpose.  
  

**Example:**  
  

\[C#\]  
  

// create the object of type Pop3MailboxInfo  

Aspose.Network.Pop3.Pop3MailboxInfo info;  
  

// get the mailbox information  

info = client.GetMailboxInfo();  
  

// check number of messages  

Console.WriteLine(info.MessageCount);  
  

// check mailbox size  

Console.Write(info.OccupiedSize + " bytes");  
  

\[VB.Net\]  
  

' create the object of type Pop3MailboxInfo  

Dim info As Aspose.Network.Pop3.Pop3MailboxInfo  
  

' get the mailbox information  

info = client.GetMailboxInfo()  
  

' check number of messages  

Console.WriteLine(info.MessageCount)  
  

' check mailbox size  

Console.Write(info.OccupiedSize + " bytes")  
  

**Check messages information in the mailbox**  
  

In this example, we will check all the messages in the mailbox using **Pop3MessageInfoCollection** class. We will use **Pop3Client.ListMessages()** function to get the **Pop3MessageInfoCollection**. Then we will iterate through the collection to read the message information.  
  

**Example:**  
  

\[C#\]  
  

// get the list of messages in the mailbox  

Aspose.Network.Pop3.Pop3MessageInfoCollection infos = client.ListMessages();  
  

// iterate through the messages  

foreach(Aspose.Network.Pop3.Pop3MessageInfo info in infos)  

{  

   Console.Write("Id:" + info.UniqueId);  

   Console.Write("Index number:" + info.SequenceNumber);  

   Console.Write("Subject:" + info.Subject);  

   Console.Write("size:" + info.Size);  

}  
  

\[VB.Net\]  
  

' get the list of messages in the mailbox  

Dim infos As Aspose.Network.Pop3.Pop3MessageInfoCollection = client.ListMessages()  
  

' iterate through the messages  

For Each info As Aspose.Network.Pop3.Pop3MessageInfo In infos  

    Console.Write("Id:" + info.UniqueId)  

    Console.Write("Index number:" + info.SequenceNumber)  

    Console.Write("Subject:" + info.Subject)  

    Console.Write("size:" + info.Size)  

Next  
  

**Retrieve messages from the mailbox**  
  

To get the messages from the mailbox we will use the **FetchMessage()** method of **Pop3Client** to get the message in a **MailMessage** type object.  
  

**Example:**  
  

\[C#\]  
  

// get number of messages in the mailbox  

int messageCount = client.GetMessageCount();  
  

// iterate through the messages and retrieve one by one  

for(int i=1; i<= messageCount; i++)  

{  

       // create object of type MailMessage  

Aspose.Network.Mail.MailMessage msg;  
  

       // retrieve the message in MimeMessage format directly  

       msg = client.FetchMessage(i);  
  

       Console.WriteLine("From:" + msg.From.ToString());  

       Console.WriteLine("Subject:" + msg.Subject);  

       Console.WriteLine(msg.HtmlBody);  
  

       // save in local drive  

msg.Save(i + ".eml");  

}  
  

\[VB.Net\]  
  

' get number of messages in the mailbox  

Dim messageCount As Integer = client.GetMessageCount()  

For i As Integer = 1 To messageCount  
  

    ' iterate through the messages and retrieve one by one  

    ' create object of type MailMessage  

    Dim msg As Aspose.Network.Mail.MailMessage  
  

    ' retrieve the message in MimeMessage format directly  

    msg = client.FetchMessage(i)  
  

    Console.WriteLine("From:" + msg.From.ToString())  

    Console.WriteLine("Subject:" + msg.Subject)  

    Console.WriteLine(msg.HtmlBody)  
  

    ' save in local drive  

    msg.Save(i + ".eml")  

Next








