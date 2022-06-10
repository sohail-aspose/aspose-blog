---
title: 'Handle Mixed LTR/RTL Text, Render DrawingML and Breaking of Floating Tables in Word Documents'
date: Tue, 11 Nov 2014 09:45:15 +0000
draft: false
url: /2014/11/11/handle-mixed-ltrrtl-text-render-drawingml-and-breaking-of-floating-tables-in-word-documents/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

[](http://www.aspose.com/.net/word-component.aspx)[Aspose.Words][1] 14.10.0 has been released. This month’s release contains over 106 useful new features, enhancements and bug fixes to the Aspose.Words products.

You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 14.10.0][2]
*   [Aspose.Words for Java 14.10.0][3]

Here is a look at just a few of the biggest features and API changes in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the links above.

*   Improved DocumentBuilder to handle mixed LTR/RTL text.
*   Improved breaking of floating tables in layout.
*   Improved custom tab stop beyond line ending.
*   Implemented new features and effects for DrawingML rendering.
*   Added the LoadOptions.WebRequestTimeout property.

## LoadOptions.WebRequestTimeout Public Property Added

We have now added hte LoadOptions.WebRequestTimeout option. Previously, HTML import tried to load images using WebRequest with default time out 100000ms which some times failed for every image with the error 'Unable to connect to the remote server' exception.

```
 /// <summary>
/// The number of milliseconds to wait before the web request times out. The default value is 100000 milliseconds (100 seconds).
/// </summary>
/// <remarks>
/// The number of milliseconds that Aspose.Words waits for a response, when loading external resources (images, style sheets)
/// linked in HTML and MHTML documents.
/// </remarks>
public int WebRequestTimeout
{
    get { return mWebRequestTimeout; }
    set { mWebRequestTimeout = value; }
} 
```

## Rendering of DrawingML Textboxes now Supported

In earlier versions when Aspose.Words encountered DrawingML text box, it rendered fallback VML Shape textbox. That is why rotation and some other formatting properties were lost. In the new version of Aspose.Words, it renders true DrawingML textboxes. Also, to be able to render DrawingML textboxes, DmlRenderingMode.DrawingML must be set.




[1]: https://products.aspose.com/words/
[2]: https://products.aspose.com/words/net
[3]: https://products.aspose.com/words/java




