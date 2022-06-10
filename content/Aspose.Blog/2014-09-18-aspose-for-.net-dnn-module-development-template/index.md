---
title: 'Support for Aspose.Note for .NET and Visual Studio 2013 Added to Aspose for .NET DNN Module Development Template'
date: Thu, 18 Sep 2014 11:43:43 +0000
draft: false
url: /2014/09/18/aspose-for-.net-dnn-module-development-template/
author: Zaheer Tariq
summary: ''
tags: ['News Release']
categories: ['Aspose.Total Product Family', 'Aspose.Note Product Family']
---

Aspose for .NET DNN Module Development Template provides a quick and easy way to use module development template for DNN 7+. We are pleased to announce a new release which now supports exploring examples of our new product [Aspose.Note for .NET][1]. This module development template can automatically download Aspose components and seamlessly add them to your DNN module project during project creation.

The new improved version provides the following features:

*   Supports **Visual Studio 2010, 2012 and 2013.**
*   Create DNN modules with C# or VB.NET.
*   Create DNN modules with the new DAL2 data access layer available in DNN 7 for C# or VB.NET.
*   Select one or more Aspose components during module creation.
*   The latest version of the selected Aspose components are automatically downloaded and referenced in your DNN Module.



{{< figure align=center src="images/aspose-dnn-supports-vs2010-vs2012-vs2013-300x246.png" alt="Aspose DNN Template supports Visual Studio 2010, 2012 and 2013" caption="Aspose DNN Template supports Visual Studio 2010, 2012 and 2013">}}




{{< figure align=center src="images/preview-300x239.png" alt="Aspose .NET Module Development Template for DNN" caption="Aspose .NET Module Development Template for DNN">}}


## New Features

This release has the following new features:

1.  Support for **Visual Studio 2013**.  
    It is the only Development template which supports 3 versions of Visual Studio.
2.  Integrated new Aspose product: Aspose.Note for .NET

You can use this module development template to download and explore the following exciting features of Aspose.Note for .NET.

Loading, saving and converting:

*   Converting OneNote to PDF.
*   Converting OneNote to image.

Working with images:

*   Extract images from a OneNote document.
*   Get information of each image from OneNote document.

Working with pages:

*   Get number of pages from OneNote document.

Working with text:

*   Extract text from OneNote document.
*   Replace text in pages of a OneNote document.

## Customer Feedback

Your feedback is very important to us. Please feel free to provide feedback and raise feature requirements. We are keen to implement customer driven features since we are a 100% customer driven company.

## System Requirements

In order to install and use Aspose .NET Module Development Template for DNN you need to have one of the following Visual Studio version installed

*   Visual Studio 2010
*   Visual Studio 2012
*   Visual Studio 2013

Please feel free to contact us if you find any issues in installing or using this plugin.

## Installing Aspose for .NET DNN Module Development Template

Installing the Aspose DotNetNuke project templates is pretty easy. There are multiple ways to install: choose one of these options below.

### Install manually by downloading the VSIX file from the DNN Store

1.  Visit the DNN Store - [Aspose DotNetNuke Module Development Template page][2].
2.  Click **Add to Cart** and then proceed to checkout to download the VSIX file.
3.  Double-click the downloaded file to install the templates.

### Install manually by downloading from Codeplex

1.  Download the VSIX file from Codeplex.
2.  Double-click the downloaded file to install the templates.

**Note:** Please make sure to restart Visual Studio for the changes to take effect.

## Creating a DNN Module using the Template

Once you've installed the templates, you can set up a project based on them. To do so you should follow the steps below. Before you can use them, you should have installed Visual Studio 2010, 2012 or 2013 and Aspose DotNetNuke Project Templates (described above).

1.  Set up the DotNetNuke Development environment following the steps in the Wiki (the templates assume you have your development environment set up at http://dnndev.me/). Development Environment
2.  Run Visual Studio 2010, 2012 or 2013 as an Administrator (right-click the desk-top shortcut to do so)
3.  From the **File** menu, select **New Project**.
4.  Choose either C# or VB.Net from the Languages section of the new project dialog.



{{< figure align=center src="images/create-dnn-project-300x193.png" alt="Create DNN Project" caption="Create DNN Module Project">}}


Select the DotNetNuke Folder under your preferred language (C# or Visual Basic). Choose either the **Aspose DotNetNuke C# Compiled Module** or **Aspose DotNetNuke 7 C# DAL2 Compiled Module** template for your project template (or the VB.NET versions). For the new project creation screen using the following settings

1.  Name: ModuleName  
    Something unique here, example DNNTaskManager
2.  Location: c:\\websites\\dnndev.me\\desktopmodules\\  
    This assumes you set up your development environment as instructed in step 1.
3.  Solution: Create new solution
4.  Create directory for solution : **Unchecked**  
    If checked, this option will cause path problems. The templates assume that the SLN is in the same folder as the project file.
5.  Click **OK**.

A screen is shown containing all Aspose components (screenshot below). Select one or more components from the list.  
Each component's common uses is shown upon selection. Click **Next** to continue once done.



{{< figure align=center src="images/aspose-dnn-select-aspose-components-300x239.png" alt="Aspose DNN create project select components" caption="Aspose DNN create project wizard select Aspose components">}}


The Next screen shows the download progress for each selected component.



{{< figure align=center src="images/ddn-wizard-aspose-product-download-300x239.png" alt="Aspose DNN create project component download" caption="Aspose DNN create project wizard Aspose component download">}}


Once the downloading is completed the module is created with the selection components automatically reference. Aspose DNN created module

This creates a folder under c:\\websites\\dnndev.me\\desktopmodules\\ModuleName which should contain all the files necessary for your module, including the solution.

There are a couple of final steps just to finalize the process, documented in the **Documentation\\Documentation.html** file, which should open up automatically in Visual Studio after the project is created. Follow the steps to configure the final project properties and then you are ready to build/deploy a module. You can delete the documentation folder once you have completed those steps.




[1]: https://products.aspose.com/note/net
[2]: http://store.dnnsoftware.com/home/product-details/aspose-net-module-development-template-for-dnn




