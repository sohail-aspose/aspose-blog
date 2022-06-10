---
title: 'Auto Discover Exchange Server settings using Aspose.Email for Java 18.5'
date: Sat, 09 Jun 2018 20:08:01 +0000
draft: false
url: /2018/06/09/auto-discover-exchange-server-settings-using-aspose.email-for-java-18.5/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

[![aspose-email-for-java][1]](https://products.aspose.com/email/java)[Aspose.Email for Java 18.5][2] has been released. This month’s release includes new feature of Auto Discovery of Exchange Server settings using the API’s EWS client. It also enhances the PST to Exchange server import operation. For a detailed note on what is new and fixed, please visit the [release notes][3] section of the API documentation.

# Support for Auto Discovery Feature using Aspose.Email for Java 18.5

This release introduces a new feature of [auto-discovery of Exchange server settings][4] using account’s user name and password. The AutoDiscoverService introduced by the API gets this information from the exchange server using the username and password specified by application user. In addition to other settings returned by the API, you can get the server’s EWS Url as well using this feature.

```
String email = "...";
String password = "...";
AutodiscoverService svc = new AutodiscoverService();
svc.setCredentials(new NetworkCredential("username@domain.com", "password"));

IGenericDictionary<Integer,Object> userSettings = svc.getUserSettings(email, UserSettingName.ExternalEwsUrl).getSettings();
String ewsUrl = (String)userSettings.get_Item(UserSettingName.ExternalEwsUrl);
System.out.println("Exchange Server Url: " + ewsUrl); 
```

# Abort PST to Exchange Server Operation

Import of large size PSTs to Exchange server can result in operation timeout which can lead to unexpected results. This month’s release provides the capability to defined timeout for the operation so that it can stop upon meeting the desired criterion. This allows users to [abort the PST restore operation][5] in case it is taking too long to complete the operation.

```
PersonalStorage pst = PersonalStorage.fromFile("");
		
IEWSClient client = EWSClient.getEWSClient("https://exchange.domain.com", "username", "password");
		
final AtomicInteger numberOfProcessedItems = new AtomicInteger(0);

RestoreSettings rs  = new RestoreSettings();
		
rs.setBeforeItemCallback(new BeforeItemCallback() {
    public void invoke(ItemCallbackArgs item) {
        if (numberOfProcessedItems.get() >= 1)
        {
            throw new AbortRestoreException();
        }

        numberOfProcessedItems.incrementAndGet();
    }
});

try {
    client.restore(pst, rs);
} catch (AbortRestoreException e) {
    System.out.println("1 resored");
} 
```

# API Resources

We have detailed information available online for getting started with the Aspose.Email for Java API. These are:

*   [Product Documentation][6]– Provides detailed examples of working with the API
*   [API Reference Guide][7]– Details all the packages and classes of the API
*   [GitHub Examples][8]– Provides ready to run API examples
*   [Aspose.Email Forum][9]– Feel free to contact us on Aspose.Email forum for your queries




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2016/09/aspose-Email-for-Java_100.png
[2]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-email
[3]: https://docs.aspose.com/display/emailjava/Aspose.Email+for+Java+18.5+Release+Notes
[4]: https://docs.aspose.com/display/emailjava/Utility+Features#UtilityFeatures-AutoDiscoverFeatureusingEWS
[5]: https://docs.aspose.com/display/emailjava/Utility+Features#UtilityFeatures-AbortingPSTtoExchangeServerOperation
[6]: https://docs.aspose.com/display/emailjava/Home
[7]: http://www.aspose.com/api/java/email
[8]: https://github.com/aspose-email/Aspose.Email-for-Java
[9]: https://forum.aspose.com/c/email




