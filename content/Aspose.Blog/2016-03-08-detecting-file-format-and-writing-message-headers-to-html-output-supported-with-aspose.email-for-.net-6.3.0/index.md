---
title: 'Detecting File Format and Writing Message Headers to HTML Output supported with Aspose.Email for .NET 6.3.0'
date: Tue, 08 Mar 2016 14:30:26 +0000
draft: false
url: /2016/03/08/detecting-file-format-and-writing-message-headers-to-html-output-supported-with-aspose.email-for-.net-6.3.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

[![][1]](https://products.aspose.com/email)We are pleased to announce the release of [Aspose.Email for .NET 6.3.0][2]. This month’s release comes with new features and enhancements that  add to the list of features supported by the API. To get a complete list of what is new and fixed, please visit our product download page. You can also have an idea about the API changes in this month’s release by visiting our product documentation section, Public API Changes in Aspose.Email for .NET 6.3.0.

# Enhancements

**Capability to Detect File Formats:** This month’s release includes a new feature of detecting file format of provided email message file. The _FileFormatUtil_ class provides the capability to detect the file type of provided message file and returns the results as an object of _FileFormatInfo_. It can be used to detect message type from both message file or from stream.

**Writing Message Headers to Html Output:** We introduced the feature of exporting message data to html format in one of our earlier releases. This month’s release further enhances this feature by providing the capability of writing message headers to html output. The _HtmlSaveOptions_ class can be used to specify the option of writing message headers to output html as shown in the following code sample.

```
MailMessage eml = MailMessage.Load(fileName);
HtmlSaveOptions options = SaveOptions.DefaultHtml;
options.EmbedResources = false;
//save the message headers to output HTML using the formatting options
options.HtmlFormatOptions = HtmlFormatOptions.WriteHeader | HtmlFormatOptions.WriteCompleteEmailAddress; 
eml.Save(outFileName, options); 
```

**Message Signing with Detached Signature:** With this month’s release, the API now provides the capability to sign messages with the option to detach signature before sending. Detaching the signature before sending the email enables the web-based email clients to display message contents which was not the case earlier. The overloaded method of _AttachSignature_ provides the _boolean_ flag that can be set to false for detaching a signature from a message prior to sending.

# Bug Fixes

This month’s release also fixes a number of bugs that were reported by our valued customers. These further add to the overall performance improvement of the API functionality. Complete list of fixed bugs can be viewed by visiting our product [download page][3].

# API Resources

The following API resources can be of help to you in getting started with Aspose.Email API.

*   Product Documentation – Provides detailed examples of working with the API
*   API Reference Guide – Details all the namespaces and classes of the API
*   [GitHub Examples][4] – Provides ready to run API example
*   [Support Forum][5] – Write to us if you have any query or inquiry about the API




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2016/03/aspose-Email-for-net_100.png "Aspose.Email for .NET"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.email-for-.net/category1411.aspx
[3]: http://www.aspose.com/community/files/51/.net-components/aspose.email-for-.net/category1411.aspx
[4]: https://github.com/asposeemail/Aspose_Email_NET
[5]: http://www.aspose.com/community/forums/aspose.email-product-family/188/showforum.aspx




