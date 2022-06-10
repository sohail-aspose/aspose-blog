---
title: 'Aspose.AdHoc 1.6.0 Released!'
date: Wed, 25 Mar 2009 21:38:00 +0000
draft: false
url: /2009/03/25/aspose-adhoc-1-6-0-released/
author: PavelM
summary: ''
tags: []
categories: ['Aspose.Total Product Family']
---

Dear Customers,  

We've released Aspose.AdHoc v1.6.0!It contains most recent bug fixes and new features.  
  
**Custom localization  
  
**By default AdHoc is translated to three languages: English, Arabic and Dutch (Nederland).  
From now, you can create custom localization resource sets based on a template provided in Downloads section of the web site.  
  
All you need to do is:  

*   Change (localize) string resources from template project
*   Compile project and copy resource set binary to Aspose.AdHoc directory
*   Set _Aspose.AdHoc.UseUnsignedResource_ to "true"
*   Assign your culture to _Aspose.AdHoc.CultureInfo_  
    

Now run your application localized.  
  
**NOTE:** Custom localization works only when Aspose.AdHoc binary is not placed to Global Assembly Cache.  

For more information refer http://www.aspose.com/documentation/visual-components/aspose.adhoc-for-.net/internationalize-and-localize.html  
  

  
**Data Source lifetime control**  
  
Aspose.AdHoc stores reference to data source DataTable in Page.Session and as a result, the data source may be lost when session expires. The control's behavior related to session expiration has been improved the following way:  
  
If you are using Aspose.AdHoc in DisconnectedData mode (_Aspose.AdHoc.DisconnectedData_ is set to "true"), Aspose.AdHoc needs _Page.Session_ only before DataSource was bound with Aspose.AdHoc._DataBind_ method.  

If _Aspose.AdHoc.DisconnectedData_ is set to "false", _Aspose.AdHoc.DataSourceInaccessible_ event will warn you that reference to data source was lost due to session timeout or session clearing. You will be able to reassign data source through event handler arguments. If data source was not reassigned, component will switch to DisconnectedData mode automatically.  
  
**NOTE:** Don't forget about DisconnectedData mode restrictions.  

You can find resource template project in Resources section.  
  

Thanks!








