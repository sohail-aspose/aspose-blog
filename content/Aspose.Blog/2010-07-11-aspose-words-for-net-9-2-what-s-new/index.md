---
title: 'Aspose.Words for .NET 9.2 - What''s New'
date: Sun, 11 Jul 2010 23:35:00 +0000
draft: false
url: /2010/07/11/aspose-words-for-net-9-2-what-s-new/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

If you upgrade to Aspose.Words for .NET 9.2 you will get:

**Performance improvements** to the rendering (conversion to PDF, XPS) and field update engines. We are now pleased with testing DOCX to PDF conversion of a document 526 pages long with lots of tables and a big Table Of Contents. Compare this with earlier versions where we did not expect "fast" conversion for documents bigger than 100-200 pages.

**GDI+ is no longer used for font measurement** during layout and rendering. This resolves some rare 64-bit server-side exceptions such as "cannot create a handle" etc. In one of the next versions you will be able to completely avoid relying on fonts installed on Windows. You will be able to specify folder(s) where Aspose.Words should look for TrueType font files when converting to PDF or XPS. This is also an important preparation step towards Aspose.Words for Java better conversion to PDF on other OSes such as Ubuntu.

**More field types are supported** by our world-famous field update engine. Our expert will write on this more in the next post.

**Get list labels and numbers** - This is a highly requested feature, finally available. You can now get the string that contains the list label for a paragraph that is a member of a bulleted or numbered list. Aspose.Words generates list labels in exactly the same way as Microsoft Word does it. Aspose.Words uses this list label generator internally when converting to PDF and other formats and now this is also available via the public API. More on this in a separate post.

**Get information about a document without loading it** - Previously, it was only possible to detect the document format without loading a document. Now we have extended the API so you can detect more document formats (also distinguish template formats from normal documents), detect encrypted and digitally signed documents too. It could be a good idea to detect a digitally signed document and maybe prompt the user before programmatically modifying such document, because the digital signature will be lost as you can understand.

**Tons of other important fixes and improvements**, for the full list see the download page [http://www.aspose.com/community/files/51/.net-components/aspose.words-for-.net/entry247974.aspx][1]

But here is the catch: **there are breaking changes in the public API**. In brief, I can describe them as:

**All events and delegates were removed**. In fact, they were replaced with properties and interfaces. Instead of using the .NET events and delegates we are now using the more classical approach of callbacks. All the functionality is still there, you will only need to make simple changes to your code.

**Document loading and saving methods were reworked**. All Aspose components are now moving towards the Aspose Unified Framework which basically means more consistent and robust public APIs across all Aspose products. Aspose.Words is the first one to implement the new standard for loading and saving of documents.

More info about the breaking changes will be coming soon in the documentation, in this blog and there are already some tutorial videos in the Downloads section [http://www.aspose.com/community/files/51/.net-components/aspose.words-for-.net/default.aspx][2]




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.words-for-.net/entry247974.aspx
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.words-for-.net/default.aspx




