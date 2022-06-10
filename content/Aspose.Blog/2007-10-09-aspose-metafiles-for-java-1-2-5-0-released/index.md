---
title: 'Aspose.Metafiles for Java 1.2.5.0 Released'
date: Tue, 09 Oct 2007 03:29:00 +0000
draft: false
url: /2007/10/09/aspose-metafiles-for-java-1-2-5-0-released/
author: Alcrus
summary: ''
tags: []
categories: ['Aspose.Total Product Family']
---

**What's New:**  

*   Reading comments from a metafile. Small example how to read comments:

> ```
> WmfMetafile wfile = new WmfMetafile(file);  
> MetafileComment\[\] comments = wfile.getComments();  
> for(int i = 0; i < comments.length; i++) {  
>     System.out.println("comment " + comments\[i\].getRecordIndex() + ": " +  
>     Charset.defaultCharset().decode(ByteBuffer.wrap(comments\[i\].getCommentData())).toString());  
> }  
> 
> ```

*   Rendering text in different charsets. Aspose.Metafiles should select right charset automatically but it is possible to override it through rendering hints.

> ```
> MetafileCharsetCollection cc = new MetafileCharsetCollection();  
> Charset charset = (Charset)Charset.availableCharsets().get("windows-1251");  
> cc.SetCharset(MetafileCharsetCollection.DEFAULT\_CHARSET, charset);  
> renderingHints.put(MetafileCharsetCollection.METAFILES\_CHARSET\_COLLECTION, cc);  
>   
> 
> ```

**Fixed:**  

*   3862 - Aspose.Metafiles didn't work with Aspose.Total for Java license.

To download: [http://www.aspose.com/Community/Files/51/aspose.metafiles/default.aspx][1]




[1]: http://www.aspose.com/Community/Files/51/aspose.metafiles/default.aspx




