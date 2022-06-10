---
title: 'Aspose.Report - Some advanced features for RDL element'
date: Wed, 05 Jan 2005 15:08:00 +0000
draft: false
url: /2005/01/05/32596/
author: GeorgeKahn
summary: ''
tags: ['George Kahn']
---

As we know, most of business reports are not just based on a static SQL script, they will be varied by different situation such as field column or filter, our RDL element class model allow user to create their own data type and bind the data with our existed report element type. The following is the sample RDL script.```
 <?xml version="1.0"?>
 <report name="TestDataBinding" startaction="define\_data">
   <reportparameter id="sql.table.name" value="product" />
   <reportaction name="define\_data" nextaction="generate\_sql">
      <dataitemset id="sql.fields">
         <sqlfield id="sql.fields.1" field="category\_name" alias="cat" />
         <sqlfield id="sql.fields.2" field="brand\_name" alias="brand" />
         <sqlfield id="sql.fields.3" field="upc\_id" alias="UPC" />
      </dataitemset>
   </reportaction>
```<reportaction name="generate\_sql" nextaction="format\_report"> <sqlitem root="true"> <sqlitem begin="select "> <reportparameter id="sql.comma" value="" /> <foreach item="DataItems" variable="sql.fields.counter"> <dataitems refid="sql.fields" /> <sqlitem text="${sql.comma}" /> <sqlitem> <binding sourceid="sql.fields" sourceprop="field" targetprop="text" index="${sql.fields.counter}" /> </sqlitem> <sqlitem text=" as " /> <sqlitem> <binding sourceid="sql.fields" sourceprop="alias" targetprop="text" index="${sql.fields.counter}" /> </sqlitem> <reportparameter id="sql.comma" value=", " /> </foreach> </sqlitem> <sqlitem text="from ${sql.table.name}" newline="true" /> <sqlitem text=" order by 1" /> </sqlitem> </reportaction> <reportaction name="format\_report"> <reportitem label="${sql.table.name}"> <foreach item="DataItems" variable="sql.fields.counter"> <dataitems refid="sql.fields" /> <reportitem> <binding sourceid="sql.fields" sourceprop="alias" targetprop="label" index="${sql.fields.counter}" /> </reportitem> </foreach> </reportitem> </reportaction> </report> And here is log output.```
    SqlItem output
```select category\_name as cat, brand\_name as brand, upc\_id as UPC from product order by 1 ReportItem output left:0; top:0; width:0; height:0 - (0)brand left:0; top:0; width:0; height:0 - (0)UPC left:0; top:0; width:0; height:0 - (0)product Instead of specifiying the customized data types in **DataItemSet** inside the RDL script, the framework also provide the development API extension to allow developers to write their own functions that could load their own data types into **DataItemSet** from the database or file and compile the data types and functions into a standalone library.```
 <dataitemset id="sql.fields" loadfunc="${sqlfield::insert-fields()}" />
```Our RDL element class model provide the support for embedding a RDL script file into another RDL script file, user will benefit from it by sharing the reporting logic among different reports, such as a set of RDL to retrieve the definition from user data dictionary or define the report layout style. The following is the sample RDL script.```
 <?xml version="1.0"?>
 <report name="TestNestedReport" startaction="gather\_data" >
   <reportparameter id="global.var1" value="test\_subreport1" />
   <reportparameter id="global.var2" value="test\_subreport2" />
```<reportaction name="gather\_data" nextaction="format\_report"> <rdl startaction="subreport2"> <reportfiles> <include name="E:\\\\reporttools\\\\data\\\\SubNestedReport1.RDL" /> </reportfiles> </rdl> </reportaction> <reportaction name="format\_report"> <log message="format\_report" level="Debug" /> </reportaction> </report>







