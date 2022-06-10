---
title: 'Export Message Headers to HTML with Aspose.Email for Java 6.3.0'
date: Mon, 14 Mar 2016 15:18:15 +0000
draft: false
url: /2016/03/14/detect-file-formats-and-export-message-headers-to-html-output-with-aspose.email-for-java-6.3.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-Java_100.png" alt="">}}


We are pleased to announce the release of [Aspose.Email for Java 6.3.0][1]. Ported from its equivalent .NET version, this month’s release includes new features, enhancements and a number of bug fixes. A complete list of all public API Changes can be found in our documentation section, [Public API Changes in Aspose.Email for Java 6.3.0][2].

## Exporting Message Headers to Output HTML

Aspose.Email API already provides the capability of converting email messages to Html output. This month’s release further enhances the capability of exporting [message headers to Html][3] output. The _setHtmFormatOptions_ method of _HtmlSaveOptions_ class provides additional parameters to write header as well as complete email address information to output html.

## Detecting File Format

Aspose.Email for Java now provides the capability to [detect input file][4] format. The API provides the _FileFormatUtil_ class to detect the input file type using the _detectFileFormat_ method. It can detect file format from string input path of the file or from stream as well.

## Using Detached Signature Option

Aspose.Email API already provides the capability of signing messages using the _AttachSignature_ method. However, there were issues faced while sending signed messages to web-based email services. This issue has been resolved now by enhancing the capability of sending signed messages with [detached signature][5] option. The overloaded version of attachSignature method provides a _Boolean_ flag for specifying the signature as detached before it could be sent out. This enables web based email services to display the email contents properly.

## Bug Fixes

This month’s release of Aspose.Email for Java includes the same bug fixes as were present in the .NET equivalent version of the product. For a complete list of the issues that have been fixed in this month’s release, please visit our [Product download][6] page.

## API Resources

We have detailed information available online for getting started with the Aspose.Email for Java API. These are:

*   [Product Documentation][7] – Provides detailed examples of working with the API
*   [API Reference Guide][8] – Details all the packages and classes of the API
*   [GitHub Examples][9] – Provides ready to run API examples
*   [Aspose.Email Forum][10] – Feel free to contact us on Aspose.Email forum for your queries




[1]: http://www.aspose.com/community/files/72/java-components/aspose.email-for-java/default.aspx
[2]: http://docs.aspose.com/display/emailjava/Public+API+Changes+in+Aspose.Email+6.3.0
[3]: http://docs.aspose.com/display/emailjava/Converting+Email+Messages#ConvertingEmailMessages-SaveAsHTML
[4]: https://docs.aspose.com/display/emailjava/Loading+and+Saving+Message#LoadingandSavingMessage-DetectingFileFormats
[5]: https://docs.aspose.com/display/emailjava/Utility+Features+-+SMTP+Client#UtilityFeatures-SMTPClient-WorkingwithSignedMessages
[6]: http://www.aspose.com/community/files/72/java-components/aspose.email-for-java/default.aspx
[7]: http://docs.aspose.com/display/EmailJava/Home
[8]: http://docs.aspose.com/display/emailjava/Aspose.Email+for+Java+API+Reference
[9]: https://github.com/aspose-email/Aspose.Email-for-Java
[10]: http://www.aspose.com/community/forums/aspose.email-product-family/188/showforum.aspx




