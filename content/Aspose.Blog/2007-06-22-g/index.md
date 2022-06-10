---
title: 'Retrieving Property Information by Mapi Property Tag'
date: Fri, 22 Jun 2007 20:08:00 +0000
draft: false
url: /2007/06/22/g/
author: Iret
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

**MapiProperty** Class represents a Mapi property, which contains:

*   _Name_, a string represents the name of the property
*   _Tag_, a long represents the tag of the property
*   _Data_, a byte array represents the data of the property

## Steps to Query Mail Box Status

*   Create a MapiMessage instance by loading from files or stream
*   Get the MapiProperty from MapiMessage.Properties by MapiPropertyTag keys
*   Get the Data of the MapiProperty by method GetXXXX

**Example**

```
 \[C#\]
```
```
 //load from file
 MapiMessage msg = MapiMessage.FromFile(@”c:\test.msg”);

 string subject;

 //access the MapiPropertyTag.PR_SUBJECT property 
 MapiProperty prop = msg.Properties[MapiPropertyTag.PR_SUBJECT];

 //if the prop is not found, check the MapiPropertyTag.PR_SUBJECT_W (which is a unicode peer of the MapiPropertyTag.PR_SUBJECT)
 if (prop == null)
 {
   prop = msg.Properties[MapiPropertyTag.PR_SUBJECT_W];
 }

 //cannot found
 if (prop == null)
 {
   Console.WriteLine(“No property found!”);
   return;
 }

 //get the property data as string
 subject = prop.GetString();

 Console.WriteLine(“Subject:” + subject);
```

\[VB.NET\]

```
 ‘load from file
 Dim msg As MapiMessage =  MapiMessage.FromFile(“c:\test.msg”) 
 
 Dim subject As String
 
 ‘access the MapiPropertyTag.PR_SUBJECT property 
 Dim prop As MapiProperty =  msg.Properties(MapiPropertyTag.PR_SUBJECT) 
 
 ‘if the prop is not found, check the MapiPropertyTag.PR_SUBJECT_W (which is a unicode peer of the MapiPropertyTag.PR_SUBJECT)
 If prop Is Nothing Then
   prop = msg.Properties(MapiPropertyTag.PR_SUBJECT_W)
 End If
 
 ‘cannot found
 If prop Is Nothing Then
   Console.WriteLine(“No property found!”)
   Return
 End If
 
 ‘get the property data as string
 subject = prop.GetString()
 
 Console.WriteLine(“Subject:” + subject)
```








