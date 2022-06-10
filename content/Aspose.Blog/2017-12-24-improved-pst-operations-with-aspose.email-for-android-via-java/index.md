---
title: 'Preserve Attachment''s Format when Exporting Tasks and Contacts from PST in Android'
date: Sun, 24 Dec 2017 03:48:47 +0000
draft: false
url: /2017/12/24/improved-pst-operations-with-aspose.email-for-android-via-java/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose_email-for-android-min-150x150.png" alt="aspose-email-for-android-via-java">}}


We are pleased to announce the release of [Aspose.Email for Andorid via Java 17.12][1]. This month’s release includes an enhancement for preserving attachment’s format while exporting Tasks and Contacts from PST file. It also includes several other improvements in terms of bug fixes that further add to the overall stability of the API. For a detailed note on what is new and fixed, you may visit the [release notes][2] section in the API documentation.

# Preserving Attachments Format During Conversion

This release introduces the capability to save Outlook item’s attachment format during saving to disc. Attachment MSG formats can now be preserved while exporting Outlook Contacts and Tasks from the PST file. This can be achieved using the setPreserveEmbeddedMessageFormat method of EmlSaveOptions to true.

{{< gist aspose-com-gists 709d733586ce50505c3bca3f6e8bd18d "Examples-src-main-java-com-aspose-email-examples-email-PreservingEmbeddedMessageFormatduringLoading-PreservingEmbeddedMessageFormatduringLoading.java" >}}

# Other Improvements

This release also includes several improvements in terms of bug fixes. These include issues related to:

*   Processing of encrypted messages
*   Email messages to MHTML
*   Rendering of hyperlinks to HTML during conversion
*   Timezone changes during the conversion of EML to MSG
*   Exceptions while converting messages to MSG and ICS
*   Loss of formatting during messages conversion to XPS

# API Resources

Aspose.Email for Android via Java [documentation section][3] is your one-stop for learning all about the API. You can visit the documentation page of the API to know more about the API. For any of your queries, feel free to write to us over [Aspose.Email forum][4].




[1]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-email/17.12/
[2]: https://docs.aspose.com/display/emailjava/Aspose.Email+for+Android+via+Java+17.12+Release+Notes
[3]: https://docs.aspose.com/display/emailjava
[4]: https://forum.aspose.com/c/email




