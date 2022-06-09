---
title: 'Using Aspose.Drawing in Azure Functions with C#'
seoTitle: "Use System.Drawing library in Azure Functions | Aspose.Drawing API"
description: "Use System.Drawing library in Azure Functions to avoid any issues. Aspose.Drawing is simple and compatible with cloud infrastructure using C#."
date: Wed, 22 Sep 2021 08:06:00 +0000
draft: false
url: /2021/09/22/use-system-drawing-in-azure-functions/
author: Farhan Raza
summary: 'Azure functions are event-based, serverless cloud services. You can use Aspose.Drawing for .NET API in Azure functions for drawing vector graphics or text as per your requirements. This article explains how quickly and easily you can configure the API to use in Azure Functions.'
tags: ['Aspose.Drawing in Azure', 'Aspose.Drawing in Azure Functions', 'System.Drawing in Azure', 'System.Drawing in Azure Functions']
categories: ['Aspose.Drawing Product Family']
---

Azure functions are event-based, serverless cloud services. You can use Aspose.Drawing for .NET API in Azure functions for drawing vector graphics or text as per your requirements. This article explains how quickly and easily you can configure the API to use in Azure Functions:

*   [Create an Azure Function Application.][1]
*   [Add Aspose.Drawing NuGet Package to the Project.][2]
*   [Add code for Drawing an Image.][3]
*   [Publish the Project to Azure.][4]
*   [Test the Function in Azure.][5]

## Create an Azure Functions Application {#section1}

Firstly, please create an HTTP trigger function from the Azure functions project template as shown in the following screenshot:



{{< figure align=center src="images/System.Drawing-in-AzureFunction-1024x599.png" alt="System.Drawing in Azure Function">}}


## Add Aspose.Drawing NuGet Package to the Project {#section2}

[Aspose.Drawing for .NET][6] API is hosted on [NuGet][7] gallery. Please add the dependency in the project with the user interface or using the installation command below:

```
PM> Install-Package Aspose.Drawing
```

## Add code for Drawing an Image {#section3}

Then, you need to add little code for drawing an image as the API takes care of the minor details. Please replace the following code to Function1.cs file for drawing a gradient and returning the output image for an HTTP request:

{{< gist aspose-com-gists fd329244e599249d5ef2ccde159eadf8 "Aspose-Drawing-Azure-Function.cs" >}}

Now, copy your Aspose.Drawing.NET.lic license file with Aspose.Drawing licensing information to the project directory, open this file properties from Solution Explorer and set Copy to Output Directory to Copy always. If you do not have the license then you can request a Free Evaluation License to test the API in its full capacity.

## Publish the Project to Azure {#section4}

Then, publish your project to Azure as described in [Quickstart: Create your first function in Azure using Visual Studio][8].

## Test the Function in Azure {#section5}

In the address bar of a browser, append the string _/api/Function1_ to the base URL and run the request (the full request will look like https://azurefunctionapp123456789.azurewebsites.net/api/Function1).

Finally, you will see the following drawing result:



{{< figure align=center src="images/Aspose.Drawing-Azure-Function-1.png" alt="Aspose.Drawing in Azure Function">}}


## Conclusion

In this article, you have learned how to work with Aspose.Drawing for .NET API in Azure functions. System.Drawing namespace can have compatibility issues in Azure functions so you can easily use Aspose.Drawing API without any issues. Moreover, you can always reach out to us at the [Free Support Forum][9] in case of any concerns.

## See Also

*   [Add, Insert, or Draw Text on PNG, JPEG, TIFF, Icon, GIF Image using C#][10]
*   [Apply Matrix, Global, Local, World Coordinate Transformation in C#][11]




[1]: #section1
[2]: #section2
[3]: #section3
[4]: #section4
[5]: #section5
[6]: https://products.aspose.com/drawing/net
[7]: https://nuget.org/packages/Aspose.Drawing
[8]: https://docs.microsoft.com/en-us/azure/azure-functions/functions-create-your-first-function-visual-studio#publish-the-project-to-azure
[9]: https://forum.aspose.com/c/drawing/44
[10]: https://blog.aspose.com/2021/02/28/draw-text-image-csharp/
[11]: https://blog.aspose.com/2021/03/04/matrix-global-local-world-transformation-csharp/




