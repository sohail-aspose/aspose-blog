---
title: 'Use IMAP Multi-Connection Backup and Restore Option in C# and Java'
date: Tue, 18 Jun 2019 04:34:17 +0000
draft: false
url: /2019/06/18/imap-multi-connection-backup-and-restore-option-available-in-aspose.email-19.5/
author: Mudassir
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

[![][1]](https://products.aspose.com/email/net)Hello firends! in today's blog, I am going to introduce you to what new features have been included in Aspose.Email 19.5. As always, Aspose team has published both .NET and Java based API having same features sets simultaneously. This way, the users of both API's can make use of new features irrespective of application and platform type. In following sections, I will shed some light on new features available in API and how to use them.

## Getting OLM Folder path

Now, you have got support to traverse through folders and sub-folders inside OLM storage file and access them [OlmFolder.Path][2] property which returns the folder path. In following example, we have demonstrated the recursive use of [OlmFolder.Path][3] property to get the folder and sub-folders paths in the OML file.

{{< gist aspose-com-gists 522d47278b8ca448dc1d7eb97193322c "Examples-CSharp-Outlook-OLM-GetFolderPathInOLM-1.cs" >}}

The similar Java based example for this is:

{{< gist aspose-com-gists 709d733586ce50505c3bca3f6e8bd18d "Examples-src-main-java-com-aspose-email-examples-outlook-olm-GetFolderPathInOLM-1.java" >}}

## Getting user defined folders only inside PST

The PST/OST files may contain folders which have been created by user. Now, Aspose.Email provides the ability to access only user-defined folders by using the [PersonalStorageQueryBuilder.OnlyFoldersCreatedByUser][4] property. One can set the [PersonalStorageQueryBuilder.OnlyFoldersCreatedByUser][5] property to **True** to get only user-defined folders. The following example demonstrates the use of [PersonalStorageQueryBuilder.OnlyFoldersCreatedByUser][6] and getting user-defined folders.

{{< gist aspose-com-gists 522d47278b8ca448dc1d7eb97193322c "Examples-CSharp-Outlook-PST-GetFoldersCreatedByUserOnly-1.cs" >}}

The similar Java based example for this is:

{{< gist aspose-com-gists 709d733586ce50505c3bca3f6e8bd18d "Examples-src-main-java-com-aspose-email-examples-outlook-pst-GetFoldersCreatedByUserOnly-1.java" >}}

## IMAP Multi-connection Backup and Restore {#ConnectingtoIMAPServer-ConnectingtoServerinRead-Onlymode}

When working with a large number of messages, the backup/restore operation can take a long time. For this, the API provides support for multiple connections during backup and restore operation. To enable the MultiConnection mode, set [ImapClient.UseMultiConnection][7] property to [MultiConnectionMode.Enable][8]. The following examples demonstrate the use backup and restore operation with MultiConnection mode enabled.

{{< gist aspose-com-gists 522d47278b8ca448dc1d7eb97193322c "Examples-CSharp-IMAP-ImapBackupOperationWithMultiConnection-1.cs" >}} {{< gist aspose-com-gists 522d47278b8ca448dc1d7eb97193322c "Examples-CSharp-IMAP-ImapRestoreOperationWithMultiConnection-1.cs" >}}

The similar Java based example for this is:

{{< gist aspose-com-gists 709d733586ce50505c3bca3f6e8bd18d "Examples-src-main-java-com-aspose-email-examples-imap-ImapBackupOperationWithMultiConnection-1.java" >}} {{< gist aspose-com-gists 709d733586ce50505c3bca3f6e8bd18d "Examples-src-main-java-com-aspose-email-examples-imap-ImapRestoreOperationWithMultiConnection-1.java" >}}

There's many other features, enhancement, and bug fixes included in this release. [Here you can get the detail!][9]

When time allows you can check out API [examples at Github][10], talk about this release and other API related issues in our [forum][11].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2016/12/Aspose.Email-for-.NET_.png
[2]: https://apireference.aspose.com/net/email/aspose.email.storage.olm/olmfolder/properties/path
[3]: https://apireference.aspose.com/net/email/aspose.email.storage.olm/olmfolder/properties/path
[4]: https://apireference.aspose.com/net/email/aspose.email.storage.pst/personalstoragequerybuilder/properties/onlyfolderscreatedbyuser
[5]: https://apireference.aspose.com/net/email/aspose.email.storage.pst/personalstoragequerybuilder/properties/onlyfolderscreatedbyuser
[6]: https://apireference.aspose.com/net/email/aspose.email.storage.pst/personalstoragequerybuilder/properties/onlyfolderscreatedbyuser
[7]: https://apireference.aspose.com/net/email/aspose.email.clients/emailclient/properties/usemulticonnection
[8]: https://apireference.aspose.com/net/email/aspose.email.clients/multiconnectionmode
[9]: https://docs.aspose.com/display/emailnet/Aspose.Email+for+.NET+19.5+Release+Notes
[10]: https://github.com/aspose-email
[11]: https://forum.aspose.com/c/email




