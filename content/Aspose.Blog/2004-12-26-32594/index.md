---
title: 'Aspose.Report - A unit test case for RDL element types'
date: Sun, 26 Dec 2004 17:58:00 +0000
draft: false
url: /2004/12/26/32594/
author: GeorgeKahn
summary: ''
tags: ['George Kahn']
---

The following is RDL script used by one of unit test cases.

```
 <?xml version="1.0"?>
 <report name="Simple" startaction="prepare\_query"  librarydir="E:\\reporttools\\src\\Aspose\\ReportTools\\ReportTools.RDLElement\\bin\\Debug">
   <variable name="var\_action\_1" value="gather\_data" />
   <variable name="var\_action\_2" value="format\_report" />
   <reportaction name="prepare\_query" nextaction="check\_sql" description="generate the Sql script for reports">
      <log message="generate the SQL for report query!" level="Debug" />
 <!-- Putting the RDL elements that are used for specifying or assembling the SQL script here -->
      <variable name="action\_result" value="good" />
      <if condition="${action\_result=='bad'}">
         <variable name="var\_action\_1" value="done" />
      </if>
   </reportaction>
   <reportaction name="check\_sql" nextaction="${var\_action\_1}">
      <log message="the SQL is ${action\_result}, so next action is ${var\_action\_1}!" level="Debug" />
   </reportaction>
   <reportaction name="gather\_data" nextaction="${var\_action\_2}">
      <log message="gather the data for report, its next action is ${var\_action\_2}!" level="Debug" />
 <!-- Putting the RDL elements that are used for retrieving the data here -->
   </reportaction>
   <reportaction name="format\_report" nextaction="done">
      <log message="format report!" level="Debug" />
 <!-- Putting the RDL elements that are used for specifying the output type and layout here-->
   </reportaction>
   <reportaction name="done">
      <log message="Done!" level="Debug" />
   </reportaction>
 </report>





```

And here is the log information produced by this test case.

```
               First action specified: prepare\_query 
               prepare\_query:
                     \[log\] generate the SQL for report query!


               check\_sql:
                     \[log\] The SQL is good, so next action is gather\_data!


               gather\_data:
                    \[log\] gather the data for report, its next action is format\_report!
 .
               format\_report:
                     \[log\] format report!


               done:
                     \[log\] Done!



```

We could get some feels about the RDL element types from the sample above. There are five RDL element types inside this RDL snippet that are report, reportaction, variable, if, and log, every element type has respective attributes and functionality, such as [reportaction][1] and [if][2] are mainly used for controlling the procedural flow, [variable][3] is used for specifying the new macro variables and assigning the value to existed variables, [log][4] is used for writing the log




[1]: /wiki/wikiedit.aspx?topic=MyWiki.reportaction&return=MyWiki.FlowControl "Click here to create this topic"
[2]: /wiki/wikiedit.aspx?topic=MyWiki.if&return=MyWiki.FlowControl "Click here to create this topic"
[3]: /wiki/wikiedit.aspx?topic=MyWiki.variable&return=MyWiki.FlowControl "Click here to create this topic"
[4]: /wiki/wikiedit.aspx?topic=MyWiki.log&return=MyWiki.FlowControl "Click here to create this topic"



