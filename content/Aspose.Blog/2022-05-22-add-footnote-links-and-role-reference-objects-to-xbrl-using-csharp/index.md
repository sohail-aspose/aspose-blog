---
title: 'Add Footnote Links and Role Reference Objects to XBRL using C#'
seoTitle: "Add Footnote Links and Role Reference Objects to XBRL using C#"
description: "Programmatically create XBRL instance document and Add Footnote Links and Role Reference Objects to XBRL using C# with Aspose.Finance for .NET API."
date: Sun, 22 May 2022 05:46:06 +0000
draft: false
url: /2022/05/22/add-footnote-links-and-role-reference-objects-to-xbrl-using-csharp/
author: Muzammil Khan
summary: 'You can easily create an XBRL instance document programmatically and add objects or elements such as Footnote Link, Role Reference, Arc Role Reference, etc. In this article, you will learn **how to add footnote links and role reference objects to XBRL using C#**.'
tags: ['Add ArcRole in XBRL C#', 'Add Footnote in XBRL C#', 'Add Objects to XBRL C#', 'Add Role Reference in XBRL C#', 'Footnote in XBRL', 'Role Reference in XBRL', 'XBRL', 'XBRL Instance C#']
categories: ['Aspose.Finance Product Family']
---



{{< figure align=center src="images/add-footnote-links-and-role-reference-objects-to-xbrl-using-csharp.jpg" alt="Add Footnote Links and Role Reference Objects to XBRL using C#">}}


In the [previous post][1], we learned how to add schema reference, context, unit, and fact objects to XBRL instance documents using C#. In this article, we will learn **how to add footnote links and role reference objects to XBRL using C#**.

The following topics shall be covered in this article:

*   [C# API to Add Footnote Links and Role Reference Objects to XBRL][2]
*   [Add Footnote Links to XBRL][3]
*   [Add Role Reference Object to XBRL][4]
*   [Arc Role Reference Object in XBRL][5]

## C# API to Add Footnote Links and Role Reference Objects to XBRL {#CSharp-API-to-Add-Footnote-Links-and-Role-Reference-Objects-to-XBRL}

For adding role reference and arc role reference objects to an XBRL instance document, we will be using the [Aspose.Finance for .NET][6] API. It allows creating XBRL instances, parsing, and validating the XBRL or iXBRL files. The **_[XbrlDocument][7]_** class of the API represents an XBRL document that contains one or more XBRL instances. An XBRL instance is an XML fragment, with the root element having an XBRL tag. The **_[XbrlInstance][8]_** class provides various methods and properties to work with the XBRL instance. The _**[FootnoteLink][9]**_ class contains locators, resources, and arcs to describe the relationships between facts in an XBRL Instance. The API provides _**[RoleReference][10]**_ class that allows referencing the definitions of any custom role attribute values used in footnote links in the XBRL instance. Similarly, the **_[ArcRoleReference][11]_** class allows resolving custom arc role values that are used in a Link base or an XBRL Instance.

Please either [download][12] the DLL of the API or install it using [NuGet][13].

```
PM> Install-Package Aspose.Finance
```

## Add Footnote Links to XBRL using C# {#Add-Footnote-Links-to-XBRL-using-CSharp}

We can add a footnote link in an XBRL instance document by following the steps given below:

1.  Firstly, create an instance of the **_XbrlDocument_** class.
2.  Add a new XBRL instance to the _XbrlDocument_ object’s instances.
3.  Add a new schema reference to the _**XbrlInstance**_ object’s schema references.
4.  Get _**[SchemaRef][14]**_ by its index from _**SchemaRefCollection**_.
5.  Initialize the **_[Context][15]_** instance and add it to the [Context objects][16] collection.
6.  Define a _**[Footnote][17]**_ instance and set its label and text.
7.  Initialize Locator type using the [Loc][18] class instance.
8.  Define _**[FootnoteArc][19]**_ with Locator label and Footnote label as arguments.
9.  Create an instance of the **_FootnoteLink_** class.
10.  Add Footnote, Locator, and _FootnoteArc_ to relevant _FootnoteLink_ collections.
11.  After that, add the _FootnoteLink_ to the _FootnoteLinks_ collection.
12.  Finally, save the XBRL file using [**_XbrlDocument.Save()_**][20] method. It takes the output file path as an argument.

The following code sample shows **how to add a footnote link in an XBRL instance document using C#**.

{{< gist aspose-finance-gists 7b1a43f85e5af3c61fa9a35d00dd61e9 "Add-Footnote-Links-and-Role-Reference-to-XBRL-CSharp_AddFootnoteLink.cs" >}}

## Add Role Reference Object to XBRL using C# {#Add-Role-Reference-Object-to-XBRL-using-CSharp}

We can add a Role reference in an XBRL instance document by following the steps given below:

1.  Firstly, create an instance of the **_XbrlDocument_** class.
2.  Next, add a new XBRL instance to the _XbrlDocument_ object’s instances.
3.  Then, add a new schema reference to the **_XbrlInstance_** object’s schema references.
4.  Get **_SchemaRef_** by its index from **_SchemaRefCollection_**.
5.  Next, get the **_[RoleType][21]_** from the **_[GetRoleTypeByURI()][22]_** method.
6.  Then, create an instance of the **_RoleReference_** class with the **_RoleType_** object as an argument.
7.  After that, add the _RoleReference_ to the _RoleReference_ objects collection.
8.  Finally, save the XBRL file using [**_XbrlDocument.Save()_**][23] method. It takes the output file path as an argument.

The following code sample shows **how to add role reference in an XBRL instance document using C#**.

{{< gist aspose-finance-gists 7b1a43f85e5af3c61fa9a35d00dd61e9 "Add-Footnote-Links-and-Role-Reference-to-XBRL-CSharp_AddRoleRef.cs" >}}

## Add Arc Role Reference Object to XBRL using C# {#Add-Arc-Role-Reference-Object-to-XBRL-using-CSharp}

We can add an Arc role reference in an XBRL instance document by following the steps given below:

1.  Firstly, create an instance of the **_XbrlDocument_** class.
2.  Next, add a new XBRL instance to the _XbrlDocument_ object’s instances.
3.  Then, add a new schema reference to the **_XbrlInstance_** object’s schema references.
4.  Next, get **_SchemaRef_** by its index from **_SchemaRefCollection_**.
5.  Then, get the **_[ArcRoleType][24]_** from the **_[GetArcroleTypeByURI()][25]_** method.
6.  Next, create an instance of the **_ArcRoleReference_** class with the **_ArcRoleType_** object as an argument.
7.  After that, add the **_ArcRoleReference_** to the **_ArcRoleReference_** objects collection.
8.  Finally, save the XBRL file using [**_XbrlDocument.Save()_**][26] method. It takes the output file path as an argument.

The following code sample shows **how to add arc role reference in an XBRL instance document using C#**.

{{< gist aspose-finance-gists 7b1a43f85e5af3c61fa9a35d00dd61e9 "Add-Footnote-Links-and-Role-Reference-to-XBRL-CSharp_AddArcRoleRef.cs" >}}

## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][27] to try the library without evaluation limitations.

## Conclusion

In this article, we have learned how to:

*   create an XBRL document using C#;
*   add a footnote and footnote arc using footnote link to XBRL objects programmatically;
*   add role and arc role references in XBRL in C#.

Besides, you can learn more about Aspose.Finance for .NET API using the [documentation][28]. In case of any ambiguity, please feel free to contact us on the [forum][29].

## See Also

*   [Convert XBRL to PDF using C#][30]




[1]: https://blog.aspose.com/2022/04/14/add-objects-to-xbrl-documents-using-csharp/
[2]: #CSharp-API-to-Add-Footnote-Links-and-Role-Reference-Objects-to-XBRL
[3]: #Add-Footnote-Links-to-XBRL-using-CSharp
[4]: #Add-Role-Reference-Object-to-XBRL-using-CSharp
[5]: #Add-Arc-Role-Reference-Object-to-XBRL-using-CSharp
[6]: https://products.aspose.com/finance/net
[7]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrldocument
[8]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstance
[9]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/footnotelink
[10]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/rolereference
[11]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/arcrolereference
[12]: https://downloads.aspose.com/finance/net
[13]: https://www.nuget.org/packages/Aspose.Finance/
[14]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/SchemaRef
[15]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/Context
[16]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstance/properties/contexts
[17]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/Footnote
[18]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/loc
[19]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/FootnoteArc
[20]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrldocument/methods/save
[21]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/RoleType
[22]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/schemaref/methods/getroletypebyuri
[23]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrldocument/methods/save
[24]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/ArcRoleType
[25]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/schemaref/methods/getarcroletypebyuri
[26]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrldocument/methods/save
[27]: https://purchase.aspose.com/temporary-license
[28]: https://docs.aspose.com/finance/net/
[29]: https://forum.aspose.com/c/finance/
[30]: https://blog.aspose.com/2022/03/20/convert-xbrl-to-pdf-using-csharp/




