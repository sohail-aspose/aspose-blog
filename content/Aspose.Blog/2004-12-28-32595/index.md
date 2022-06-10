---
title: 'Aspose.Report - How RDL define the report layout'
date: Tue, 28 Dec 2004 18:19:00 +0000
draft: false
url: /2004/12/28/32595/
author: GeorgeKahn
summary: ''
tags: ['George Kahn']
---

Inside the last post, I introduced how RDL deal with procedural flow and macro variables, the following is another sample that illuminates how RDL handle the report layout.

```
 <?xml version="1.0"?>
 <report name="TestReportItemlayout" startaction="format\_report" librarydir="E:\\reporttools\\src\\Aspose\\ReportTools\\ReportTools.RDLElement\\bin\\Debug">
   <reportaction name="format\_report">
      <log message="format report!" level="Debug" />
      <reportparameter name="body.top" value="5" />
      <reportparameter name="body.left" value="5" />
      <reportparameter name="row.height" value="10" />
      <reportparameter name="column.width" value="50" />
      <reportparameter name="header.height" value="25" />
      <reportparameter name="footer.height" value="30" />
      <reportparameter name="body.column.count" value="0" />


      <reportitem left="${body.left}" top="${body.top}" label="mainpage">
         <reportitem height="${header.height}" label="header">
            <reportitem left="${int::parse(column.width) \* rdl::get-zindex()}" width="${column.width}" height="${header.height}" label="${'column' + int::to-string(rdl::get-zindex())}" />


            <reportparameter name="body.column.count" value="${int::parse(body.column.count) + 1}" />


            <reportitem left="${int::parse(column.width) \* rdl::get-zindex()}" width="${column.width}" height="${header.height}" label="${'column' + int::to-string(rdl::get-zindex())}" />


            <reportparameter name="body.column.count" value="${int::parse(body.column.count) + 1}" />


            <reportparameter name="body.width" value="${int::parse(column.width) \* int::parse(body.column.count)}" />
         </reportitem>


         <reportitem top="${header.height}" width="${body.width}" label="body">
            <foreach item="IntLoop" in="0,5" delim="," variable="row.counter">
               <reportitem top="${int::parse(row.height) \* int::parse(row.counter)}" height="${row.height}" width="${body.width}" label="${'row' + row.counter}" />


               <reportparameter name="body.row.count" value="${int::parse(row.counter) + 1}" />
            </foreach>


            <reportparameter name="body.height" value="${int::parse(row.height) \* int::parse(body.row.count)}" />
         </reportitem>


         <reportitem top="${int::parse(body.height) + int::parse(header.height)}" width="${body.width}" height="${footer.height}" label="footer" />
      </reportitem>
   </reportaction>
 </report>



```

And the here is log output.

```
 left:5; top:5; width:0; height:0 - (0)mainpage
 left:5; top:5; width:0; height:25 - (0)header
 left:5; top:5; width:50; height:25 - (0)column0
 left:55; top:5; width:50; height:25 - (1)column1
 left:5; top:30; width:100; height:0 - (1)body
 left:5; top:30; width:100; height:10 - (0)row0
 left:5; top:40; width:100; height:10 - (0)row1
 left:5; top:50; width:100; height:10 - (0)row2
 left:5; top:60; width:100; height:10 - (0)row3
 left:5; top:70; width:100; height:10 - (0)row4
 left:5; top:80; width:100; height:10 - (0)row5
 left:5; top:90; width:100; height:30 - (2)footer



```

As we can see above, reportitem is a basis RDL element type for report visual element such as Text, Box, or Line... it has some attribute about the layout and position such as Top, Left, Width and Style. Every reportitem is capable to contain a set of child elements, and child elements will be inherited some attributes from their container such as position or style.

Another thing I 'd like to point out is that RDL supports custom functions and formulas, they are provided for some complex functionality such as calculating the element position or specifying the data binding between the RDL elements and domain objects.







