---
title: 'Enhanced Support for Scalable Vector Graphics in Aspose.HTML for Java'
date: Fri, 22 Jun 2018 18:30:46 +0000
draft: false
url: /2018/06/22/enhanced-support-for-scaleable-vector-graphics-in-aspose.html-for-java/
author: Farhan Raza
summary: ''
tags: []
categories: ['Aspose.HTML Product Family']
---



{{< figure align=center src="images/aspose_html-for-java-128x128.png" alt="">}}


We are glad to announce the latest release [Aspose.HTML for Java 18.5][1], which can be downloaded from [Aspose Artifactory][2]. In this release, we have enhanced support for Scalable Vector Graphics (SVG) format. Aspose.HTML for Java 18.5 offers the capabilities to manipulate SVG, both as a part of HTML document and single SVGDocument object. It is fully compatible with the W3C [SVG2 recommendations][3] and previously implemented HTML format, so every manipulation feature, including the loading, saving, editing, navigating or rendering, is supported exactly the same way. You can refer to the summary of public API changes and improvements in [release notes][4] of [Aspose.HTML for Java 18.5][5].

## Support for Metered License

We have also introduced support for metered license mechanism for the customers who want to be billed based on the usage of API features. After reviewing the released API, we have found some issues while using new feature i.e Metered License and worked over fixing this. Since we intended to provide this feature in June Release of the API, we have fixed this issue in a hotfix version i.e. **Aspose.HTML for Java 18.5.1**. For convenience of our customers and API users, we have only shared the download link of latest version as usual, so that the downloaded API have all the features and enhancement which has been announced along with its release.

By downloading latest available version of Aspose.HTML for Java, you will be able to use metered license feature as well as other mentioned enhancements regarding Scalable Vector Graphics (SVG). However, in order to use metered license feature, you can implement this feature in your application by using the following code snippet:

**Java**

```
// Set metered public and private keys
com.aspose.html.Metered metered = new com.aspose.html.Metered();
// Access the setMeteredKey property and pass public and private keys as parameters
metered.setMeteredKey("*****", "*****");

// Load the document from disk.
com.aspose.html.HTMLDocument document = new com.aspose.html.HTMLDocument("Test.html");
// Print inner HTML of file to console
System.out.println(document.getBody().getInnerHTML());
```

## Miscellaneous Resources

As we always recommend our customers to use latest version of the API, please visit the following links for information regarding [Aspose.HTML for Java 18.5 (hotfixed 18.5.1)][6] and [Release Notes][7] section. In case of any inquiry, regarding Aspose.HTML for Java API, please feel free to create a topic and post your query on our [Support Forums][8]. We will be more than happy to assist you accordingly.

*   [Home page for Aspose.HTML for Java][9]
*   [Download Aspose.HTML for Java][10]
*   [Aspose.HTML product family forum][11]– Post your technical questions and queries, or any other problem you faced while running Aspose.HTML APIs.
*   [Aspose.HTML for Java online documentation][12]– help documentation on using Aspose.HTML for Java API.
*   [Aspose.HTML for Java API Reference][13]– Online public API reference for using the API.
*   [Enable Blog Subscription][14]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.HTML APIs, new features, fixes and other API related topics by subscribing to Aspose.HTML blog.




[1]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-html/18.5.1
[2]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-html/18.5.1
[3]: https://www.w3.org/TR/SVG2/
[4]: https://docs.aspose.com/
[5]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-html/18.5.1
[6]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-html/18.5.1
[7]: https://docs.aspose.com/
[8]: https://forum.aspose.com/c/html
[9]: https://products.aspose.com/html/java
[10]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-html/18.5.1
[11]: https://forum.aspose.com/c/html
[12]: https://docs.aspose.com/display/htmljava/Home
[13]: https://apireference.aspose.com/java/html
[14]: https://blog.aspose.com/category/aspose-products/aspose-html-product-family/




