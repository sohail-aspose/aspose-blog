---
title: 'Add Comments to PowerPoint PPT Slides in Python'
date: Fri, 14 Jan 2022 04:18:00 +0000
draft: false
url: /2022/01/14/add-comments-to-ppt-slides-in-python/
author: 'Usman Aziz'
summary: 'Often, the content in presentations is required to be reviewed by other people to get their feedback. In PowerPoint, comments are used to write feedback about a particular word, phrase, or anything on a slide. In this article, we will cover **how to add comments to PowerPoint PPT slides programmatically in Python**. Moreover, you will learn how to read the existing comments and add replies.'
tags: ['Add Comment Replies in PPT Slides in Python', 'Python Library to Add Comments in PowerPoint PPT', 'Read Comments from PPT Slides in Python']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Add-Comments-to-PowerPoint-PPT-Slides-1.png" alt="Add Comments to PowerPoint PPT Slides in Python">}}


Often, the content in presentations is required to be reviewed by other people to get their feedback. In PowerPoint, comments are used to write feedback about a particular word, phrase, or anything on a slide. In this article, we will cover **how to add comments to PowerPoint PPT slides programmatically in Python**. Moreover, you will learn how to read the existing comments and add replies.

*   [Python Library to Add Comments in PowerPoint PPT][1]
*   [Add Comments to PPT Slides][2]
*   [Add Comment Replies in PPT Slides][3]
*   [Read Comments from PPT Slides][4]

## Python Library to Add Comments in PowerPoint PPT {#Library-to-Add-Comments-in-PowerPoint-PPT}

To add and read comments and their replies, we will use [Aspose.Slides for Python via .NET][5]. The library is designed to create rich PowerPoint presentations from scratch. Moreover, it allows you to manipulate the existing presentations seamlessly. You can install the library in your applications from [PyPI][6] using the following command.

```
> pip install aspose.slides
```

## Add Comments to PPT Slides in Python {#Add-Comments-to-PPT-Slides}

In PowerPoint presentations, the comments are associated with the authors. Whereas, each comment contains some additional information such as time of creation, slide where it is added, and its position. The following are the steps to add comments to a slide in PPT using Python.

*   First, load the presentation file or create a new one using **Presentation** class.
*   Then, add a new slide or get reference of an existing slide from **Presentation.slides** collection.
*   Add a new author to the authors collection using **Presentation.comment\_authors.add\_author(string, string)** method.
*   Get reference of the newly created author in an object.
*   Define the position of the comment.
*   Add comment using **Author.comments.add\_comment(string, ISlide, point, date)** method.
*   Finally, save presentation using **Presentation.save(string, SaveFormat)** method.

The following code sample shows how to add comments to PPT slides in Python.

{{< gist aspose-com-gists 6274bdcda54aa25303af9ae93109ca80 "add-comment-in-ppt-slide.py" >}}

The following is the screenshot of the slide that we get after adding the comment.



{{< figure align=center src="images/Add-Comments-to-PPT-Slides.png" alt="Insert Comments to PPT Slides in Python">}}


## Add Comment Replies in PPT Slides in Python {#Add-Comment-Replies-in-PPT-Slides}

Aspose.Slides also allows you to add replies to the comments. A reply itself is a comment which is associated with an existing comment. So let's see how to add replies to comments in PowerPoint PPT slides in Python.

*   First, load the presentation file or create a new one using **Presentation** class.
*   Then, add new slide or get reference of the existing slide from **Presentation.slides** collection.
*   Add a new author and get its reference in an object.
*   Insert comment using **Author.comments.add\_comment(string, ISlide, point, date)** method and get returned object.
*   Insert another comment in the same way and get its reference in an object.
*   Set parent of the second comment using **parent\_comment** property.
*   Finally, save presentation using **Presentation.save(string, SaveFormat)** method.

The following code sample shows how to add replies to comments in a PPTX presentation in Python.

{{< gist aspose-com-gists 6274bdcda54aa25303af9ae93109ca80 "add-comment-reply-in-ppt-slide.py" >}}

The following screenshot shows the output of the code sample above.



{{< figure align=center src="images/Add-Comment-Replies-to-PPT-Slides.png" alt="Add reply to the comments in PPT">}}


## Read Comments in PPT Slides in Python {#Read-Comments-from-PPT-Slides}

You can also read comments from the PPT slides added by a specific author or all the authors. The following are the steps to read comments in PPT slides in Python.

*   Load the presentation file using **Presentation** class.
*   Loop through the list of authors using **Presentation.comment\_authors** collection.
*   For each author, loop through its comments using **Author.comments** property.
*   Read comment using its properties.

The following code sample shows how to read comments in PPT slides in Python.

{{< gist aspose-com-gists 6274bdcda54aa25303af9ae93109ca80 "read-ppt-slide-comments.py" >}}

## Get a Free License {#Get-a-Free-API-License}

You can use Aspose.Slides for Python via .NET without evaluation limitations by requesting a [temporary license][7].

## Conclusion

In this article, you have learned how to add comments in PowerPoint PPT slides in Python. Moreover, we have covered how to add replies and read comments in PowerPoint presentations programmatically. Besides, you can visit the [documentation][8] to explore more about Aspose.Slides for Python via .NET. Also, you can post your queries to our [forum][9].

## See Also

*   [Create PowerPoint Files in Python][10]
*   [Convert PPTX to PDF in Python][11]
*   [Convert PPT to PNG in Python][12]
*   [PPT/PPTX to HTML in Python][13]




[1]: #Library-to-Add-Comments-in-PowerPoint-PPT
[2]: #Add-Comments-to-PPT-Slides
[3]: #Add-Comment-Replies-in-PPT-Slides
[4]: #Read-Comments-from-PPT-Slides
[5]: https://products.aspose.com/slides/python-net
[6]: https://pypi.org/project/aspose.slides/
[7]: https://purchase.aspose.com/temporary-license
[8]: https://docs.aspose.com/slides/python-net/
[9]: https://forum.aspose.com/
[10]: https://blog.aspose.com/2021/12/31/create-powerpoint-presentations-in-python/
[11]: https://blog.aspose.com/2021/12/28/convert-pptx-ppt-to-pdf-python/
[12]: https://blog.aspose.com/2021/12/29/convert-ppt-to-png-in-python/
[13]: https://blog.aspose.com/2021/12/16/convert-ppt-to-html-in-python/




