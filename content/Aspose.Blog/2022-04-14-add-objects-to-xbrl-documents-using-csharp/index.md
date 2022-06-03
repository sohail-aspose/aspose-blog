---
title: 'Add Objects to XBRL Documents using C#'
date: Thu, 14 Apr 2022 12:22:02 +0000
draft: false
url: /2022/04/14/add-objects-to-xbrl-documents-using-csharp/
author: 'Muzammil Khan'
summary: 'You can easily create an XBRL instance document programmatically and add objects or elements such as schema reference, context, unit, items, etc. In this article, you will learn **how to add objects to XBRL instance documents using C#**.'
tags: ['Add Context Object in XBRL using C#', 'Add Fact Object in XBRL using C#', 'Add Schema Reference to XBRL using C#', 'Create Units in XBRL using C#', 'XBRL', 'XBRL Instance C#']
categories: ['Aspose.Finance Product Family']
---



{{< figure align=center src="images/add-objects-to-xbrl-documents-using-csharp.jpg" alt="Add Objects to XBRL Documents using C#">}}


[XBRL][1] (_eXtensible Business Reporting Language_) defines and exchanges financial information, such as a financial statement. An XBRL instance document is a collection of facts that together make up a business report. We can easily create an XBRL instance document programmatically and add objects or elements such as schema reference, context, unit, items, etc. In this article, we will learn **how to add objects to XBRL instance documents using C#**.

The following topics shall be covered in this article:

*   [C# API to Add Objects to XBRL Instance Documents][2]
*   [Add Schema Reference to XBRL][3]
*   [Add Context Object in XBRL][4]
*   [Create a Unit in XBRL][5]
*   [Add Fact Object in XBRL][6]

## C# API to Add Objects to XBRL Instance Documents {#CSharp-API-to-Add-Objects-to-XBRL-Instance-Documents}

For creating an XBRL instance document and adding objects, we will be using the [Aspose.Finance for .NET][7] API. It allows creating XBRL instances, parsing, and validating the XBRL or iXBRL files. Please either [download][8] the DLL of the API or install it using [NuGet][9].

```
PM> Install-Package Aspose.Finance
```

## Add Schema Reference to XBRL using C# {#Add-Schema-Reference-to-XBRL-using-CSharp}

We can add schema reference in an XBRL instance document by following the steps given below:

1.  Firstly, create an instance of the [XbrlDocument][10] class.
2.  Next, get the _XbrlDocument_ object's instances’ collection into [XbrlInstanceCollection][11] object.
3.  Then, add a new XBRL instance using [XbrlInstanceCollection.Add()][12] method.
4.  Next, get the XbrlInstance object's schema reference collection into [SchemaRefCollection][13] object.
5.  After that, add a new schema reference using [SchemaRefCollection.Add()][14] method.
6.  Finally, save the XBRL file using [XbrlDocument.Save()][15] method. It takes the output file path as an argument.

The following code sample shows **how to add schema reference in an XBRL instance document using C#**.

{{< gist aspose-com-gists 10d18f8c84c8f6622d805c4599213dd0 "AddObjectsToXBRL_CSharp_AddSchemaRef.cs" >}}

## Add Context Object in XBRL using C# {#Add-Context-Object-in-XBRL-using-CSharp}

We can add a context to an XBRL instance document by following the steps given below:

1.  Firstly, create an instance of the [XbrlDocument][16] class.
2.  Next, get _XbrlDocument_ object's instances’ collection into [XbrlInstanceCollection][17] object.
3.  Then, add a new XBRL instance using [XbrlInstanceCollection.Add()][18] method.
4.  Next, create an instance of the [ContextPeriod][19] class with the start and end dates.
5.  Then, create a [ContextEntity][20] and provide schema and identifier.
6.  Next, create an instance of the [Context][21] class with the defined ContextPeriod and ContextEntity.
7.  After that, add the Context object to the [Context objects][22] collection.
8.  Finally, save the XBRL file using [XbrlDocument.Save()][23] method. It takes the output file path as an argument.

The following code sample shows **how to add a context object in an XBRL instance document using C#**.

{{< gist aspose-com-gists 10d18f8c84c8f6622d805c4599213dd0 "AddObjectsToXBRL_CSharp_AddContext.cs" >}}

## Create Units in XBRL using C# {#Create-Units-in-XBRL-using-CSharp}

The units in XBRL measure numeric Items. We can add a unit in an XBRL instance document by following the steps given below:

1.  Firstly, create an instance of the [XbrlDocument][24] class.
2.  Next, get _XbrlDocument_ object's instances’ collection into [XbrlInstanceCollection][25] object.
3.  Then, add a new XBRL instance using [XbrlInstanceCollection.Add()][26] method.
4.  Next, create an instance of the [Unit][27] class with the [UnitType][28] as Measure.
5.  Then, add QualifiedName to the MeasureQualifiedNames collection.
6.  After that, add the Unit to the [Unit objects][29] collection.
7.  Finally, save the XBRL file using [XbrlDocument.Save()][30] method. It takes the output file path as an argument.

The following code sample shows **how to add a unit object in an XBRL instance document using C#**.

{{< gist aspose-com-gists 10d18f8c84c8f6622d805c4599213dd0 "AddObjectsToXBRL_CSharp_AddUnit.cs" >}}

## Add Fact Object in XBRL using C# {#Add-Fact-Object-in-XBRL-using-CSharp}

Facts in XBRL are defined using item elements. An item in XBRL contains the value of the simple fact and a reference to the context to correctly interpret that fact. We can add an item in an XBRL instance document by following the steps given below:

1.  Firstly, create an instance of the [XbrlDocument][31] class.
2.  Add a new XBRL instance to the _XbrlDocument_ object's instances.
3.  Add a new schema reference to the XbrlInstance object's schema references.
4.  Get SchemaRef by its index from SchemaRefCollection.
5.  Initialize the Context instance and add it to the [Context objects][32] collection.
6.  Define a Unit instance and add it to the [Unit objects][33] collection.
7.  Create a [Concept][34] class instance using the [SchemaRef.GetConceptByName()][35] method.
8.  Create an instance of the [Item][36] class with the Concept object as an argument.
9.  Set item properties such as _ContextRef_, _UnitRef_, _Precision_, _Value_, etc.
10.  After that, add the Item to the [Fact objects][37] collection.
11.  Finally, save the XBRL file using [XbrlDocument.Save()][38] method. It takes the output file path as an argument.

The following code sample shows **how to add a fact as an item element in an XBRL instance document using C#**.

{{< gist aspose-com-gists 10d18f8c84c8f6622d805c4599213dd0 "AddObjectsToXBRL_CSharp_AddFact.cs" >}}

## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][39] to try the library without evaluation limitations.

## Conclusion

In this article, we have learned **how to create an XBRL document using C#**. We have also seen **how to add various XBRL objects to the created XBRL instance document** programmatically. Besides, you can learn more about Aspose.Finance for .NET API using the [documentation][40]. In case of any ambiguity, please feel free to contact us on the [forum][41].

## See Also

*   [Convert XBRL to PDF using C#][42]
*   [Create, Parse and Validate XBRL and iXBRL Financial Reports using C#][43]




[1]: https://docs.fileformat.com/finance/xbrl/
[2]: #CSharp-API-to-Add-Objects-to-XBRL-Instance-Documents
[3]: #Add-Schema-Reference-to-XBRL-using-CSharp
[4]: #Add-Context-Object-in-XBRL-using-CSharp
[5]: #Create-Units-in-XBRL-using-CSharp
[6]: #Add-Fact-Object-in-XBRL-using-CSharp
[7]: https://products.aspose.com/finance/net
[8]: https://downloads.aspose.com/fincance/net
[9]: https://www.nuget.org/packages/Aspose.Finance/
[10]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrldocument
[11]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstancecollection
[12]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstancecollection/methods/add
[13]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/schemarefcollection
[14]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl.schemarefcollection/add/methods/1
[15]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrldocument/methods/save
[16]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrldocument
[17]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstancecollection
[18]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstancecollection/methods/add
[19]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/contextperiod
[20]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/contextentity
[21]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/context
[22]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstance/properties/contexts
[23]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrldocument/methods/save
[24]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrldocument
[25]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstancecollection
[26]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstancecollection/methods/add
[27]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/unit
[28]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/unittype
[29]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstance/properties/units
[30]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrldocument/methods/save
[31]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrldocument
[32]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstance/properties/contexts
[33]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstance/properties/units
[34]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/concept
[35]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/schemaref/methods/getconceptbyname
[36]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/item
[37]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrlinstance/properties/facts
[38]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrldocument/methods/save
[39]: https://purchase.aspose.com/temporary-license
[40]: https://docs.aspose.com/finance/net/
[41]: https://forum.aspose.com/c/finance/
[42]: https://blog.aspose.com/2022/03/20/convert-xbrl-to-pdf-using-csharp/
[43]: https://blog.aspose.com/2020/04/29/create-xbrl-instances-and-parse-and-validate-xbrl-and-ixbrl-files-in-csharp-asp.net/




