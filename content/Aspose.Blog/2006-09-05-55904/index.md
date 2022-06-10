---
title: 'Happy Import of HTML Tables and CSS Length Units'
date: Tue, 05 Sep 2006 13:28:00 +0000
draft: false
url: /2006/09/05/55904/
author: Romank
summary: ''
tags: ['Roman Korchagin']
---

There's been a public outcry for Aspose.Words inability to import CSS length units other than points. A related issue was about Aspose.Words throwing exceptions when encountering HTML that it cannot recognize. Yet another popular support issue was about HTML tables, that when imported, had cell and table widths quite different from the original.

We are happy to announce all of these issues were addressed in Aspose.Words 4.0.

All CSS length units (except em and ex at this stage) are now supported. Here is an example HTML that imports nicely:

  <table border="1">  
   <tr>  
    <td style="width: 1in;">1 inch</td>  
    <td style="width: 2CM;">2 cm</td>  
    <td style="width: 15mM;">15 mm</td>  
    <td style="width: 36Pt;">36 pt</td>  
    <td style="width: 6pc;">6 pc (72pt)</td>  
    <td style="width: 60px;">60 px</td>  
    <td style="width: 60;">60</td>  
    <td style="width: 10%;">10%</td>  
    <td style="width: -1in;">-1 in</td>  
   </tr>  
  </table>

  
Em and Ex units are not yet supported because they are relative to the current font and what the current font during HTML import into Aspose.Words is something that we still have to solve.

Also an improvement is that Aspose.Words now recognize cell and table widths specified either as an HTML or CSS width attribute. The CSS attribute will take precedence if both are specified.

  Table width specified both directly (100 pixels) and in CSS style (100 points).  
   CSS takes precedence.  
  <table border="1" width="100" style="width:100pt">  
   <tr>  
    <td> </td>  
    <td> </td>  
   </tr>  
  </table>  

Regardless of these and other improvements I must admit we are quite far away from flawlessy importing any HTML with CSS files, especially where a lot of CSS is involved. The notable problem area is CSS stylesheets with their rules, selectors and so on. Perfect (high-fidelity) import of HTML and CSS into Aspose.Words is hard because there is such a big difference between CSS and Microsoft Word formatting models. We will continue our work on improving HTML import in Aspose.Words.







