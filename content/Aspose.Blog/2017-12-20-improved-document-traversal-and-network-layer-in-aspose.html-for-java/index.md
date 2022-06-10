---
title: 'Improved Document Traversal and Network Layer in Aspose.HTML for Java'
date: Wed, 20 Dec 2017 21:45:15 +0000
draft: false
url: /2017/12/20/improved-document-traversal-and-network-layer-in-aspose.html-for-java/
author: Asad Ali
summary: ''
tags: ['Asad Ali']
categories: ['Aspose.HTML Product Family']
---



{{< figure align=center src="images/aspose_html-for-java-128x128.png" alt="">}}


We at Aspose are honored to announce the November release of [Aspose.HTML for Java][1], which is available on maven repository for download. As per regular monthly update process, we have made improvements as well as introduced new features in the API. Furthermore, we have also made some internal bug fixes, in order to provide better performance. An overview of public API changes and improvements is given in the [release notes][2] of the Aspose.Html for Java 17.11.

HTML is composed of a tree of HTML nodes, such as text nodes and each node can have HTML attributes specified. In [Aspose.HTML for Java 17.11][3], we have introduced ‘live’ and ‘static’ collections of HTML nodes according to HTML Traversal recommendations. HTMLCollection collection has been replaced with NodeList which provides ordered collection of nodes. In order to get node list by specifying selector, you can use com.aspose.html.dom.Document.QuerySelectorAll(String selector) or com.aspose.html.dom.Element.QuerySelectorAll(String selector) method(s).

```
com.aspose.html.HTMLDocument document = 
new com.aspose.html.HTMLDocument(dataDir + "example.html");

com.aspose.html.collections.NodeList nodelist = 
document.getDocumentElement().querySelectorAll("img");
```

In [Aspose.HTML for Java 17.11][4], the transport layer of library has been improved and it allows to read the document encoding from web requests/response. Along with that an enumeration “PdfPermissions” has been introduced, which is used for configuring com.aspose.html.rendering.pdf.Encryption() method.

## Miscellaneous Resources

Please visit the following links for information regarding [Aspose.HTML for Java 17.11][5] and [Release Notes ][6]section.

*   [Home page for Aspose.HTML for Java][7]
*   [Download Aspose.HTML for Java][8]
*   [Aspose.HTML product family forum][9]– Post your technical questions and queries, or any other problem you faced while running Aspose.HTML APIs.
*   [Aspose.HTML for Java online documentation][10]– help documentation on using Aspose.HTML for Java API.
*   [Aspose.HTML for Java API Reference][11]– Online public API reference for using the API.
*   [Enable Blog Subscription][12]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.HTML APIs, new features, fixes and other API related topics by subscribing to Aspose.HTML blog.




[1]: https://products.aspose.com/html/java
[2]: https://docs.aspose.com/html/java/aspose-html-for-java-17-11-release-notes/
[3]: http://maven.aspose.com/artifactory/simple/ext-release-local/com/aspose/aspose-html/17.11/
[4]: http://maven.aspose.com/artifactory/simple/ext-release-local/com/aspose/aspose-html/17.11/
[5]: http://maven.aspose.com/artifactory/simple/ext-release-local/com/aspose/aspose-html/17.11/
[6]: https://docs.aspose.com/html/java/aspose-html-for-java-17-11-release-notes/
[7]: https://www.aspose.com/products/html/java
[8]: http://maven.aspose.com/artifactory/simple/ext-release-local/com/aspose/aspose-html/17.11/
[9]: https://forum.aspose.com/c/html
[10]: https://docs.aspose.com/display/htmljava/Home
[11]: https://apireference.aspose.com/java/html
[12]: https://blog.aspose.com/category/aspose-products/aspose-html-product-family/




