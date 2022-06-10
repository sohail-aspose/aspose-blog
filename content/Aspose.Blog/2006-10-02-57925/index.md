---
title: 'Aspose.Words: We Eat Our Own Dog Food'
date: Mon, 02 Oct 2006 12:52:00 +0000
draft: false
url: /2006/10/02/57925/
author: Romank
summary: ''
tags: ['Roman Korchagin']
---

We now use Aspose.Words in the process of generating documentation for Aspose products.

We prepare documentation in Microsoft Word documents, and then use some logic plus Aspose.Word's capability to convert DOC to HTML to produce HTML and CHM documentation.

The first documentation project built this way is [Feature Overview for Aspose.Editor][1]. Next in line is migration of all Aspose.Words documentation to this technology. Other Aspose components are likely to follow too.

Aspose.Words is used not only to convert DOC to HTML, but it allows us to perform some programmatic tasks during conversion:

*   Split a single document into topics. Each topic is in its own section.
*   Detect each topic's heading - it is in the first paragraph marked with the Heading 1 style.
*   Modify hyperlinks. Original .DOC file can contain multiple topics and links between them are using bookmarks. But when exported to HTML, each topic goes into separate HTML file and the links between them must be updated accordingly.
*   Rescale images (change them to 100% zoom).
*   Modify document properties - when exported to HTML, they form keywords and title in the resulting HTML.

Let us know if you like the documentation and if you are interested in the tools used to build it. Maybe we will end up turning it into a product.




[1]: /Products/Aspose.Editor/Api/Index.html?url=FeatureOverview.html



