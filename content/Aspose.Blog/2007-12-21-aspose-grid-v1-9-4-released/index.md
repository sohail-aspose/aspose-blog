---
title: 'Aspose.Grid v1.9.4 Released!'
date: Fri, 21 Dec 2007 12:20:00 +0000
draft: false
url: /2007/12/21/aspose-grid-v1-9-4-released/
author: Henry
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

Dear Customers,  
 We have just released Aspose.Grid v1.9.4.

**What's New?  
**Aspose.Grid.Web  
1\. Added Native AJAX Support. Set the new property GridWeb.EnableAJAX to true to activate this new feature. When a cell is changed by a user at the client side, the grid will automatically recalculate the related formulas by using AJAX calls. Note: This feature doesn't require any other AJAX frameworks.

2\. Support Custom Context Menu Items. We just extended the CustomCommandButton class, added a property CommandType. Set this property to ContextMenuItem to let it display as a Menu Item.  
3\. Support "$" reference style. For examples: $A$1, SUM($A:$B)

Aspose.Grid.Desktop  
1\. Added Autofit Feature. If a column header split line is double clicked, the column will auto resize. Worksheet class also provides Autofit methods from columns to rows.  
2\. Added Comment feature. Comments data can be read and save from file.  
3\. New property Button.AlwaysVisible, indicates if the button should be visible when cell is not in focus. This property only takes effect when the button is in a cell.

**What's Improved?**  
Aspose.Grid.Web  
1\. Improved Formula Engine. Lift the performance up to 90%. Uses new algorithm to avoid stack overflow in deep nested call.  
2\. Improved the sorting performance.  
3\. Optimized the client side cell selecting event.

**What's Fixed?  
**Aspose.Grid.Web  
1\. Fixed a minor display issue in IE7.

Aspose.Grid.Desktop  
1\. Fixed the FreezeCols and Cell Merge issue.  
2\. Fixed an cell input issue.








