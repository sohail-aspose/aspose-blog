---
title: 'Aspose Customer Newsletter, February 2007'
date: Fri, 02 Feb 2007 15:36:00 +0000
draft: false
url: /2007/02/02/69518/
author: Salman Sarfraz
summary: ''
tags: ['Customer Newsletters']
---

  

**In This Issue...** 

*   **Welcome!**
*   **Product Spotlight:** [**Aspose.Workflow**][1]
*   **Aspose.Words runs on Mono!**
*   **Aspose.BarCode supports Compact Framework**
*   **Technical Tip**
*   **Aspose.Words for .NET 4.0.5 Mega Hotfix**

Welcome to the February 2007 issue of the Aspose Newsletter! In this month’s newsletter, we will provide some introductory information about our spotlight product: Aspose.Workflow. We will also cover newly added support for the Compact Framework by Aspose.BarCode and look at the new love story between Aspose.Words and Mono. You will learn about the latest news from Aspose along with the monthly Tech-Tip, which demonstrates how Aspose.Slides can be used to update OLE objects automatically when opening presentations in MS PowerPoint.  

**Product Spotlight**

[Aspose.Workflow][2] is a .NET component that provides a powerful workflow engine along with a full set of industry standard workflow objects. The heart of Aspose.Workflow is built around the WFMC standards. It utilizes XPDL (XML Process Definition Language) definitions in order to manage workflow information. Aspose.Workflow is lightening fast and works great with all kinds of .NET applications. Whether you are new to workflow or a workflow veteran, Aspose.Workflow is sure to fully accommodate your needs. Aspose.Workflow also provides an XPDL Designer that allows you to define your business processes in a GUI based environment.

Workflow is the next evolution of Business Process Management (BPM). If you are new to workflow, please take some time to [learn][3] about it. And if you are a developer looking for some solution to develop a business workflow system with great flexibility and freedom then please [download][4] the free evaluation version of Aspose.Workflow right now to see how this great component can work for you.

[![][5]](https://downloads.aspose.com/)

[![][6]](https://downloads.aspose.com/)

**Aspose.Words Runs on Mono!**

**![](https://www.aspose.com/templates/aspose/App_Themes/V3/images/words/272x272/aspose_words-for-net.png)**

We've been asked several times by our customers if [Aspose.Words][7] supports the [Mono][8] framework. Our development staff has been working on this effort and their latest testing shows Aspose.Words works with Mono version 1.2 without problems. That makes Aspose.Words the only library available in the world that deals with Microsoft Word documents on Mono. If you would like to learn more, please [click here][9] for more details.  
  
  

**Aspose.Barcode Supports Compact Framework**

**![](https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/barcode/272x272/aspose_barcode-for-net.png)**

One of the most exciting features added to [Aspose.BarCode][10] 2.2.0.0 is the support of the compact framework. All existing features of Aspose.BarCode have been successfully ported to compact framework including support for the generation and recognition of more than 20 barcode symbologies. Many new sample applications have also been added to demonstrate the barcode image recognition on smart devices. For more details, please [click here][11].  
  
  

**Technical Tip** 

**Updating OLE objects automatically using MS PowerPoint Add-In**  
  
The most frequent question asked by [Aspose.Slides][12] customers is how to create or change editable charts or any other OLE objects and have them automatically updated when opening the presentation. Unfortunately PowerPoint does not support any automatic macros, which are available in Excel and Word. The only ones available are the **_Auto\_Open_** and **_Auto\_Close_** macros. However, those only run automatically from an add-in. This short technical tip shows how to achieve that.  
  
First, there are available several freeware add-ins that add the **_Auto\_Open_** macro feature to PowerPoint for example [AutoEvents Add-in][13] and [Event Generator][14].  
  
After installing such Add-in, just add **_Auto\_Open()_** macro (**_OnPresentationOpen()_** in case of "Event Generator") to your template presentation as shown below:  
  
Sub Auto\_Open()  
   Dim oShape As Shape  
   Dim oSlide As Slide  
   Dim oGraph As Object  
  
   ' Loop through each slide in the presentation.  
   For Each oSlide In ActivePresentation.Slides  
  
      ' Loop through all the shapes on the current slide.  
      For Each oShape In oSlide.Shapes  
  
         ' Check whether the shape is an OLE object.  
         If oShape.Type = msoEmbeddedOLEObject Then  
  
            ' Found an OLE object; obtain object reference, and then update.  
            Set oObject = oShape.OLEFormat.Object  
            oObject.Application.Update  
  
            ' Now, quit out of the OLE server program. This frees  
            ' memory, and prevents any problems. Also, set oObject equal  
            ' to Nothing to release the object.  
            oObject.Application.Quit  
            Set oObject = Nothing  
         End If  
      Next oShape  
   Next oSlide  
End Sub  
  
Any change made to OLE objects with Aspose.Slides, will be updated automatically when PowerPoint opens the presentation. If you have many OLE objects in a presentation and do not want to update them all, just add a custom tag to the shapes you need to process and check it in the macro.  
  
  

**Aspose.Words for .NET 4.0.5 Mega Hotfix**

**![](https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/cells/272x272/aspose_cells-for-net.png)**

In the month of January, 2007, the Aspose.Words team released a Mega Hotfix [Aspose.Words][15] 4.0.5 that provides about 20 bug fixes related to DOC, Html, PDF and other general issues. Be sure to check out the [full list][16] of these bug fixes and [download][17] the latest release now to make your applications work better using Aspose.Words.




[1]: https://downloads.aspose.com/
[2]: https://downloads.aspose.com/
[3]: https://docs.aspose.com/display/diagramjava/How+to+Convert+a+Visio+Diagram
[4]: https://downloads.aspose.com/
[5]: https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/total/272x272/aspose_total-for-net.png
[6]: https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/total/272x272/aspose_total-for-net.png
[7]: https://downloads.aspose.com/words
[8]: http://www.mono-project.com/Main_Page
[9]: https://blog.aspose.com/
[10]: https://downloads.aspose.com/barcode
[11]: https://blog.aspose.com/
[12]: https://downloads.aspose.com/
[13]: http://skp.mvps.org/autoevents.htm
[14]: http://officeone.mvps.org/eventgen/eventgen.html
[15]: https://downloads.aspose.com/words
[16]: https://blog.aspose.com/
[17]: https://downloads.aspose.com/words



