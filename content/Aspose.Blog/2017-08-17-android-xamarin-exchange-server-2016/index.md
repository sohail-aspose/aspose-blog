---
title: 'Support for Exchange Server 2016 with Aspose.Email for Android via Xamarin'
date: Thu, 17 Aug 2017 12:57:26 +0000
draft: false
url: /2017/08/17/android-xamarin-exchange-server-2016/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

[](https://www.aspose.com/products/email/android-xamarin)[][1][![][2]](https://www.aspose.com/products/email/android-xamarin)[Aspose.Email for Android via Xamarin 17.8][3] is now available for download. This monthly release of the API brings all the latest improvements in [Aspose.Email for .NET API][4] to Xamarin platform. Specifically, it provides the capability of converting email messages to HTML without embedding resources. For a detailed note on what is new and fixed, please visit the [release notes][5] section of API documentation.

# Major Improvements

This latest version of the API not only includes enhancements from the equivalent .NET version of the API, but also contains all the bug fixes that were part of the .NET API. This keeps the Android API updated with the latest changes that are part of the parent .NET API. As mentioned earlier, we’ll be publishing monthly releases of this new API from now onwards to keep it abreast the .NET equivalent version.

**Exporting Messages to HTML without Embedding Resources:** Aspose.Email for iOS now supports [converting messages to HTML][6]  without embedding resources in output file. This allows users the classical approach of saving resource files along with source HTML file. The SaveResourceHandler provided with HtmlSaveOptions lets you achieve this by specifying the path to save the resources of the message. This is as shown in the code sample below.

```
MailMessage msg = MailMessage.Load(filePath);
var outFileName = Path.Combine(dataDir, fileName + ".html");

var options = new HtmlSaveOptions()
{
    EmbedResources = false,
    SaveResourceHandler =
        (AttachmentBase attachment, out string resourcePath) =>
        {
            attachment.Save(Path.Combine(dataDir, attachment.ContentId));
            resourcePath = Path.Combine(".", attachment.ContentId);
        }
};

msg.Save(outFileName, options); 
```

**Support for Exchange Server 2016:** As part of transition from Aspose.Email for .NET, Android application developers can now use this API to provide support for Exchange server 2016 in their emailing applications. This is a worthy feature as even modern emailing services like Outlook 365 have shifted to Exchange Server 2016. Thus, you can right away empower your Android application with support of Outlook 365 using our API.

# Other Improvements

The API also contains several fixes that further improve the API functionality as per the expected behavior. Details about such fixes are part of the release notes section for reference.

# API Resources

The following API resources can be of help to you in getting started with Aspose.Email API.

*   [Product Documentation][7]– Provides detailed examples of working with the API
*   [API Reference Guide][8]– Details all the namespaces and classes of the API
*   [GitHub Examples][9]– Provides ready to run API example
*   [Support Forum][10]– Write to us if you have any query or inquiry about the API




[1]: https://downloads.aspose.com/email/androidxamarin
[2]: https://blog.aspose.com/wp-content/uploads/sites/2/2017/08/aspose_email-for-android-via-xamarin-1-150x150.png
[3]: https://downloads.aspose.com/email/androidxamarin
[4]: https://blog.aspose.com/2017/08/09/exchange-server-2016-supported/
[5]: https://docs.aspose.com/display/emailnet/Aspose.Email+for+Android+via+Xamarin+17.8+Release+Notes
[6]: https://docs.aspose.com/display/emailnet/Loading+and+Saving+Message#LoadingandSavingMessage-SavingasHTMLwithoutEmbeddingResources
[7]: https://docs.aspose.com/display/emailnet/Home
[8]: https://www.aspose.com/api/net/email
[9]: https://github.com/asposeemail/Aspose_Email_NET
[10]: https://forum.aspose.com/c/email




