---
title: 'New MailMerge features in Aspose.Network'
date: Fri, 11 Aug 2006 00:15:00 +0000
draft: false
url: /2006/08/11/54272/
author: Iret
summary: ''
tags: ['Kyle Huang']
---

Aspose.Network 3.0 makes it simpler and easier to create E-Mail newsletter or subscription solutions. A new sophisticated E-Mail Template Engine is embeded, which provides lots of cool features and function and greatly reduce the the programming works.

Top Features in MailMerge:

*   The **First** Email Component supports using **Customer Defined Function** in the template. For example, you can register a _**TemplateRoutine**_, and use it in the template file.
*   **Creates E-mail template from file**
*   **Creates** **E-mail** **template from MailMessage** instance
*   Supports **DataTable** as data source.
*   Supports **DataRowCollection** as data source
*   Supports **DataReader** as data source
*   **Asynchronous** and **Synchronous** programming models
*   Support **Event** model

A new class called _**TemplateEngine**_ is created, for generating the E-Mail messages from the template and data source. After the E-Mail messages is created by the _**TemplateEngine**_ , Use the _**SmtpClient**_ to send the messages.

Sample:

 \[C#\]  

 //template routine to provide signature  
 static object GetSignature(object\[\] args)  
 {  
    return "John Smith<br>Product Lead<br>Aspose Ltd.<br>" + DateTime.Now.ToShortDateString();  
 }

  

 static void Main(string\[\] args)  
 {  

>  //create a new MailMessage instance as a template  
>  MailMessage template = new MailMessage();  
>    
>  //add template field to subject  
>  template.Subject = "Hello, #FirstName#";  
>  template.From = "sale@aspose.com";  
>    
>  //add template field to receipt  
>  template.To.Add(new MailAddress("#Receipt#", false));  
>    
>  //add template field to html body  
>  //use GetSignment as the template routine, which will provide the same signature.  
>  template.HtmlBody = "Dear #FirstName# #LastName#,<br><br>";  
>  template.HtmlBody += "Thank you for your interest in <STRONG>Aspose.Network</STRONG>.";  
>  template.HtmlBody += "<br><br>Have fun with it.<br><br>#GetSignature()#";  
>    
>  //create a new TemplateEngine with the template message.  
>  TemplateEngine engine = new TemplateEngine(template);  
>    
>  //register the GetSignment as a templet routine, for we use it in the template.  
>  engine.RegisterRoutine("GetSignature", new TemplateRoutine(GetSignature));  
>   
>  //fill a DataTable as data source  
>  DataTable dt = new DataTable();  
>  dt.Columns.Add("Receipt", typeof(string));  
>  dt.Columns.Add("FirstName", typeof(string));  
>  dt.Columns.Add("LastName", typeof(string));  
>   
>  DataRow dr;  
>  dr = dt.NewRow();  
>  dr\["Receipt"\] = "Nancy.Davolio<Nancy@somedomain.com>";  
>  dr\["FirstName"\] = "Nancy";  
>  dr\["LastName"\] = "Davolio";  
>  dt.Rows.Add(dr);  
>  dr = dt.NewRow();  
>  dr\["Receipt"\] = "Andrew.Fuller<Andrew@somedomain.com>";  
>  dr\["FirstName"\] = "Andrew";  
>  dr\["LastName"\] = "Fuller";  
>  dt.Rows.Add(dr);  
>  dr = dt.NewRow();  
>  dr\["Receipt"\] = "Janet.Leverling<Janet@somedomain.com>";  
>  dr\["FirstName"\] = "Janet";  
>  dr\["LastName"\] = "Leverling";  
>  dt.Rows.Add(dr);  
>    
>  MailMessageCollection messages;  
>  try  
>  {  
>    //create the messages from the template and datasource.  
>    messages= engine.Instantiate(dt);
> 
>    SmtpClient client = new SmtpClient("smtp.somedomain.com", 25, "someone","password");
> 
>    client.BulkSendAsync(messages, null);  
>  }  
>  catch (MailException ex)  
>  {  
>    System.Diagnostics.Debug.WriteLine(ex.ToString());  
>  }  
>  catch (SmtpException ex)  
>  {  
>   System.Diagnostics.Debug.WriteLine(ex.ToString());  
>  }  

 }  

  
 \[VB\]  

//template routine to provide signature  
 Shared Function GetSignature(ByVal args() As Object) As Object  
     Return "John Smith<br>Product Lead<br>Aspose Ltd.<br>" + DateTime.Now.ToShortDateString()  
 End Function  

  

 Shared Sub Main(ByVal args() As String)  

>  'create a new MailMessage instance as a template  
>  Dim template As MailMessage = New MailMessage()  
>    
>  'add template field to subject  
>  template.Subject = "Hello, #FirstName#"  
>  template.From = "sale@aspose.com"  
>   
>  'add template field to receipt  
>  template.To.Add(New MailAddress("#Receipt#",False))  
>    
>  'add template field to html body  
>  'use GetSignment as the template routine, which will provide the same signature.  
>  template.HtmlBody = "Dear #FirstName# #LastName#,<br><br>"  
>  template.HtmlBody += "Thank you for your interest in <STRONG>Aspose.Network</STRONG>."  
>  template.HtmlBody += "<br><br>Have fun with it.<br><br>#GetSignature()#"
> 
>   
>  'create a new TemplateEngine with the template message.  
>  Dim engine As TemplateEngine = New TemplateEngine(template)  
>    
>  'register the GetSignment as a templet routine, for we use it in the template.  
>  engine.RegisterRoutine("GetSignature",New TemplateRoutine(GetSignature))  
>   
>  'fill a DataTable as data source  
>  Dim dt As DataTable = New DataTable()  
>  dt.Columns.Add("Receipt", Type.GetType(String))  
>  dt.Columns.Add("FirstName", Type.GetType(String))  
>  dt.Columns.Add("LastName", Type.GetType(String))  
>    
>  Dim dr As DataRow  
>  dr = dt.NewRow()  
>  dr\["Receipt"\] = "Nancy.Davolio<Nancy@somedomain.com>"  
>  dr("FirstName") = "Nancy"  
>  dr("LastName") = "Davolio"  
>  dt.Rows.Add(dr)  
>  dr = dt.NewRow()  
>  dr\["Receipt"\] = "Andrew.Fuller<Andrew@somedomain.com>"  
>  dr("FirstName") = "Andrew"  
>  dr("LastName") = "Fuller"  
>  dt.Rows.Add(dr)  
>  dr = dt.NewRow()  
>  dr\["Receipt"\] = "Janet.Leverling<Janet@somedomain.com>"  
>  dr("FirstName") = "Janet"  
>  dr("LastName") = "Leverling"  
>  dt.Rows.Add(dr)  
>   
>  Dim messages As MailMessageCollection  
>  Try  
>    'create the messages from the template and datasource.  
>    messages= engine.Instantiate(dt)  
>    Dim smtpClient as New SmtpClient()  
>    smtpClient.Host="smtp.domain.com"  
>    smtpClient.Username="someone"  
>    smtpClient.Password="passoword"  
>    smtpClient.BulkSentAsync(messages, null)  
>   
>  Catch ex As MailException  
>    System.Diagnostics.Debug.Write(ex.ToString())  
>   Catch ex As SmtpException  
>    System.Diagnostics.Debug.Write(ex.ToString())  
>  End Try  

 End Sub







