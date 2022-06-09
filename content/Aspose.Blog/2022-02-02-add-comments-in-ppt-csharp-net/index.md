---
title: 'Add or Remove Comments in PowerPoint PPT in C#'
seoTitle: "Add or Remove Comments in PowerPoint PPT in C# | Add Comment Reply"
description: "Use .NET PowerPoint API to add comments to PPT slides programmatically in C#. Add comment replies and read or delete comments from PowerPoint presentations."
date: Wed, 02 Feb 2022 12:12:56 +0000
draft: false
url: /2022/02/02/add-comments-in-ppt-csharp-net/
author: Usman Aziz
summary: 'While reviewing the content in PowerPoint presentations, the comments are used to write the feedback. The comments can be added against a particular word, phrase, or anything on a PPT slide. In this article, you will learn **how to add comments to PowerPoint PPT slides programmatically in C#**. Moreover, we will cover how to read or remove slide comments and add their replies.'
tags: ['Add Comment Reply in PPT Slides in Csharp', 'Add Comments in PPT Slides in Csharp', 'Add Comments in PowerPoint Slides in Csharp', 'Read Comments in PPT Slides in Csharp', 'Remove Comments in PPT Slides in Csharp']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Add-Comments-to-PowerPoint-PPT-Slides.png" alt="Add or Remove Comments in PowerPoint PPT in C#">}}


While reviewing the content in PowerPoint presentations, the comments are used to write the feedback. The comments can be added against a particular word, phrase, or anything on a PPT slide. In this article, you will learn **how to add comments to PowerPoint PPT slides programmatically in C#**. Moreover, we will cover how to read or remove slide comments and add their replies.

*   [.NET API to Work with Comments in PowerPoint][1]
*   [Add Comments in PPT Slides][2]
*   [Add Comment Replies in PPT Slides][3]
*   [Read Comments from PPT Slides][4]
*   [Remove Comments from Slides][5]

## C# .NET API to Work with Comments in PowerPoint {#Library-to-Add-Comments-in-PowerPoint-PPT}

To manipulate comments in PowerPoint presentations, we will use [Aspose.Slides for .NET][6]. It is a powerful API to create and manipulate PowerPoint presentations. You can either [download][7] API’s DLL or install it using [NuGet][8].

```
PM> Install-Package Aspose.Slides.NET
```

## Add Comments to PPT Slides in C# {#Add-Comments-to-PPT-Slides}

In PowerPoint presentations, every comment is attached with a particular author. Whereas, each comment contains some additional information such as time of creation, slide where it is added, and its position. The following are the steps to add comments to a PPT slide in C#.

*   First, load the presentation file or create a new one using [Presentation][9] class.
*   Then, add a new slide or get reference of an existing slide from [Presentation.Slides][10] collection.
*   Add a new author using [Presentation.CommentAuthors.AddAuthor(string, string)][11] method.
*   Get reference of the newly created author in an object.
*   Define the position of the comment.
*   Add comment using [ICommentAuthor.Comments.AddComment(string, ISlide, Point, DateTime)][12] method.
*   Finally, save presentation using [Presentation.Save(string, SaveFormat)][13] method.

The following code sample shows how to add comments to PPT slides in C#.

{{< gist aspose-com-gists 8189e64bfacb03499ac436477a20e5df "add-comment-in-ppt-slide.cs" >}}

The following is the screenshot of the comment we have added using the above code sample.



{{< figure align=center src="images/Add-Comments-to-PPT-Slides.png" alt="Insert Comments to PPT Slides in C#">}}


## Add Comment Replies in PPT Slides in C# {#Add-Comment-Replies-in-PPT-Slides}

Aspose.Slides also allows you to add replies to the comments. A reply itself is a comment which appears as a child of an existing comment. So let's see how to add replies to comments in PowerPoint PPT slides in C#.

*   First, load the presentation file or create a new one using [Presentation][14] class.
*   Then, add new slide or get reference of the existing slide from [Presentation.Slides][15] collection.
*   Add a new author and get its reference in an object.
*   Insert comment using [ICommentAuthor.Comments.AddComment(string, ISlide, Point, DateTime)][16] method and get returned object.
*   Insert another comment in the same way and get its reference in an object.
*   Set parent of the second comment using [ParentComment][17] property.
*   Finally, save presentation using [Presentation.Save(string, SaveFormat)][18] method.

The following code sample shows how to add replies to comments in a PPTX presentation in C#.

{{< gist aspose-com-gists 8189e64bfacb03499ac436477a20e5df "add-comment-reply-in-ppt-slide.cs" >}}

The following screenshot shows the output of the above code sample.



{{< figure align=center src="images/Add-Comment-Replies-to-PPT-Slides.png" alt="Add reply to the comments in PPT">}}


## Read Comments in PPT Slides in C# {#Read-Comments-from-PPT-Slides}

Using Aspose.Slides, you can either read comments of a particular author or all the authors. The following are the steps to read comments in PPT slides in C#.

*   Load the presentation file using [Presentation][19] class.
*   Loop through the list of authors using [Presentation.CommentAuthors][20] collection.
*   For each author, loop through its comments using [CommentAuthor.Comments][21] property.
*   Read and print comment details.

The following code sample shows how to read comments in PPT slides in C#.

{{< gist aspose-com-gists 8189e64bfacb03499ac436477a20e5df "read-ppt-slide-comments.cs" >}}

## Remove Comments from PowerPoint PPT in C# {#Remove-Comments-in-PowerPoint-PPT}

In the previous section, you have seen how to read a comment by accessing it from the comments collection. Similarly, you can remove a comment after getting its reference. The following code sample shows how to remove comments in PowerPoint presentations in C#.

{{< gist aspose-com-gists 8189e64bfacb03499ac436477a20e5df "remove-ppt-slide-comments.cs" >}}

## Get a Free License {#Get-a-Free-API-License}

You can use Aspose.Slides for .NET without evaluation limitations by requesting a [temporary license][22].

## Conclusion

In this article, you have learned how to add comments in PowerPoint PPT slides in C#. Moreover, we have covered how to add replies to the comments programmatically. At the end, we have demonstrated how to read or remove comments from PPT slides. You can visit the [documentation][23] to explore more about Aspose.Slides for .NET. Also, you can post your queries to our [forum][24].

## See Also

*   [Create MS PowerPoint Presentations in C#][25]
*   [Add or Remove Shapes in PowerPoint Slides using C#][26]




[1]: #Library-to-Add-Comments-in-PowerPoint-PPT
[2]: #Add-Comments-to-PPT-Slides
[3]: #Add-Comment-Replies-in-PPT-Slides
[4]: #Read-Comments-from-PPT-Slides
[5]: #Remove-Comments-in-PowerPoint-PPT
[6]: https://products.aspose.com/slides/net
[7]: https://downloads.aspose.com/slides/net
[8]: https://www.nuget.org/packages/Aspose.Slides.Net
[9]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[10]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/properties/slides
[11]: https://apireference.aspose.com/slides/net/aspose.slides/icommentauthorcollection/methods/addauthor
[12]: https://apireference.aspose.com/slides/net/aspose.slides/icommentcollection/methods/addcomment
[13]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[14]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[15]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/properties/slides
[16]: https://apireference.aspose.com/slides/net/aspose.slides/icommentcollection/methods/addcomment
[17]: https://apireference.aspose.com/slides/net/aspose.slides/comment/properties/parentcomment
[18]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[19]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[20]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/properties/commentauthors
[21]: https://apireference.aspose.com/slides/net/aspose.slides/commentauthor/properties/comments
[22]: https://purchase.aspose.com/temporary-license
[23]: https://docs.aspose.com/slides/net/
[24]: https://forum.aspose.com/
[25]: https://blog.aspose.com/2020/12/04/create-powerpoint-presentations-in-csharp/
[26]: https://blog.aspose.com/2020/12/24/add-shapes-to-powerpoint-slides-in-csharp/




