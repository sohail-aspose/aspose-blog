---
title: 'Create or Fill HTML Form with Submit Button using C#'
seoTitle: "Create Fill HTML Form Submit Button | Input Type Checkbox Text Radio"
description: "Create or Fill HTML Form with Submit button in C#. Set Input type checkbox, text, or radio value programmatically in C#. Btn Submit in HTML form."
date: Tue, 30 Mar 2021 08:22:00 +0000
draft: false
url: /2021/03/30/create-fill-html-form-submit-button-csharp/
author: Farhan Raza
summary: 'HTML forms are frequently used for getting input from the users. You can fill in different form fields containing Checkbox, Text, Radio, and Submit button for input. You can create or fill-in the HTML form programmatically using the C# language.'
tags: ['Create HTML Form', 'Fill HTML Form', 'Fill HTML Form in C#', 'Submit Button HTML', 'Submit HTML Form in C#', 'btn submit', 'input type checkbox']
categories: ['Aspose.HTML Product Family']
---



{{< figure align=center src="images/Create-Fill-HTML-Form-Submit.png" alt="Create Fill HTML Form Submit C#">}}


[HTML][1] forms are frequently used for getting input from the users. You can fill in different form fields containing Checkbox, Text, Radio, and Submit button for input. You can create or fill-in the HTML form programmatically using the C# language. This article covers the following sections related to HTML forms:

*   [Create or Fill HTML Form - C# API Installation][2]
*   [Create an HTML Form Programmatically using C#][3]
*   [Fill HTML Form with Submit Button in C#][4]
    *   [Select the Value in Input Type Checkbox][5]
    *   [Fill the Input Type Text and Radio Field][6]
    *   [Sending Data with Submit Button in HTML][7]
    *   [Complete Source Code][8]
*   [Free API License][9]

## Create or Fill HTML Form - C# API Installation {#section0}

[Aspose.HTML for .NET][10] API lets you create or fill HTML forms with Submit buttons programmatically using C# language. You can configure the API by downloading a DLL file from the [Downloads][11] section, or quickly install it with the following [NuGet][12] installation command:

```
PM> Install-Package Aspose.Html
```

## Create an HTML Form Programmatically using C# {#section1}

You can create a HTML form programmatically using C# language. Please follow the steps below for creating it from scratch:

1.  Initialize an instance of [HTMLDocument][13] class.
2.  Create new HTML form with [CreateNew][14]() method.
3.  Input simple text type field.
4.  Create a radio button input element.
5.  Input submit button in HTML form and add current nodes.
6.  Save HTML form.

The following code shows how to create a HTML form programmatically using C#:

{{< gist aspose-com-gists d5cbfdbf27a91d2c85ba2db154909d12 "Create-HTML-Form.cs" >}}

Moreover, below is another approach for creating HTML form using native HTML form element in C#:

{{< gist aspose-com-gists d5cbfdbf27a91d2c85ba2db154909d12 "Create-HTML-Form-Native.cs" >}}

The following screenshot shows the output HTML form created with above code snippet:



{{< figure align=center src="images/Create-HTML-Form-Submit-Btn.png" alt="Create HTML Form Submit Btn">}}


## Fill HTML Form with Submit Button in C# {#section2}

You have already explored how to create an HTML form. Now you can learn how to fill HTML form and send the data to any remote server directly from your C# application. You can iterate through different items in the form and then use Submit button for sending the data. Here you will be working with a [template form][15] created by httpbin.org. It includes filling Text, Radio buttons, as well as Checkboxes that you be learning below:

### Select the Value in Input Type Checkbox {#section3}

Checkboxes are helpful where you need to choose more than one option. You can easily select the value in input type checkbox with the following code:

{{< gist aspose-com-gists d5cbfdbf27a91d2c85ba2db154909d12 "Fill-Checkbox.cs" >}}

### Fill the Input Type Text and Radio Field {#section4}

An HTML form may contain several text boxes and radio button fields for collecting data. You can fill the input text with the following code:

{{< gist aspose-com-gists d5cbfdbf27a91d2c85ba2db154909d12 "Fill-Text-Field.cs" >}}

Likewise, you can select radio button fields with the code below:

{{< gist aspose-com-gists d5cbfdbf27a91d2c85ba2db154909d12 "Fill-Radio-Button.cs" >}}

### Sending Data with Submit Button in HTML {#section5}

You can send filled data in HTML form with the Submit button using [FormSubmitter][16] class. The following code shows how to call [Submit()][17] method in C# code:

{{< gist aspose-com-gists d5cbfdbf27a91d2c85ba2db154909d12 "Submit-Button-HTML-Form.cs" >}}

### Source Code {#section6}

Below is the complete source code to fill HTML forms programmatically using C#:

{{< gist aspose-com-gists d5cbfdbf27a91d2c85ba2db154909d12 "Fill-HTML-Form-Submit-Button.cs" >}}

## Free API License {#section7}

You can evaluate Aspose.HTML for .NET API without any Evaluation Limitations by requesting a [Free Temporary License][18].

## Conclusion

In conclusion, you have learned how to create an HTML form from scratch, as well as how to fill an existing HTML form and sending the data to a remote server from your C# application. You can also visit the [Documentation][19] section to explore several other features. Please feel free to contact us at the [Free Support Forum][20] for any of your queries.

## See Also

[Split HTML Webpage into Multiple Files Programmatically using C#][21]




[1]: https://docs.fileformat.com/web/html/
[2]: #section0
[3]: #section1
[4]: #section2
[5]: #section3
[6]: #section4
[7]: #section5
[8]: #section6
[9]: #section7
[10]: https://products.aspose.com/html/net
[11]: https://downloads.aspose.com/html/net
[12]: https://www.nuget.org/packages/Aspose.Html
[13]: https://apireference.aspose.com/html/net/aspose.html/htmldocument
[14]: https://apireference.aspose.com/html/net/aspose.html.forms/formeditor/methods/createnew
[15]: https://httpbin.org/forms/post
[16]: https://apireference.aspose.com/html/net/aspose.html.forms/formsubmitter
[17]: https://apireference.aspose.com/html/net/aspose.html.forms/formsubmitter/methods/submit/index
[18]: https://purchase.aspose.com/temporary-license
[19]: https://docs.aspose.com/html/net/
[20]: https://forum.aspose.com/c/html
[21]: https://blog.aspose.com/2020/12/22/split-html-webpage-into-multiple-files-csharp/





