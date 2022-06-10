---
title: 'Aspose.AdHoc 1.5.5.0 Released!'
date: Tue, 28 Nov 2006 16:36:00 +0000
draft: false
url: /2006/11/28/62209/
author: Iret
summary: ''
tags: []
categories: ['Aspose.Total Product Family']
---

Dear Customers,

  

 We’ve released Aspose.AdHoc 1.5.5.0!

  

** What’s new:**

  

 **1.An editable dropdownlist was added to the filtering screen as showing below:**

![](/Products/Aspose.AdHoc/Images/EDITABLE_DDL.JPG)

 And more, the editable dropdownlist supports autocomplete function, that is, the user can only type part of the word and the component will pick up the matched value in the list automatically.

  

** 2\. New event 'PreSelectableItemBound' was added:**

 This new event provides a way to customize the items in the dropdownlist rather than display the values in the binding table only in the old version.Please refer to the post:      

http://www.aspose.com/Community/forums/thread/61681.aspx  

 If you have the same scenario in your application, please follow the steps below:

 1). Defined a method for handling the PreSelectableItemBound event as below:

 private void AdHoc1\_PreSelectableItemBound(string columnName, ref ArrayList valueItems)  
 {  
 if(columnName.Equals("FName"))  
 {  
 valueItems = new ArrayList();  
 valueItems.Add("FName1");  
 valueItems.Add("FName2");  
 valueItems.Add("hello");  
 valueItems.Add("welcome");  
 }  
 }

 2). Listen to the PreSelectableItemBound event with the method above:

 private void InitializeComponent()  
 { ......  
 this.ahMain.PreSelectableItemBound += new  
AdHoc.PreSelectableItemBoundEventHandler(this.AdHoc1\_PreSelectableItemBound);  
 ......  
 }

Then the dropdownlist will fill its items with the values in the ArrayList that you set in the AdHoc1\_PreSelectableItemBound method.

  

**3\. Fixed the bug in parsing SQL with quotes. Refer:**

http://www.aspose.com/Community/forums/thread/58518.aspx








