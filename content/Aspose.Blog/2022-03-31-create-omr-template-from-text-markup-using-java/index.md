---
title: 'Create OMR Template from Text Markup using Java'
date: Thu, 31 Mar 2022 09:19:39 +0000
draft: false
url: /2022/03/31/create-omr-template-from-text-markup-using-java/
author: ''Muzammil Khan''
summary: 'As a Java developer, you can easily generate OMR surveys, quizzes, or answer sheets from text markup programmatically. In this article, you will learn **how to create an OMR Template from text markup using Java**.'
tags: ['Create OMR Survey from Text Markup', 'Create OMR Template Java', 'Generate OMR Template using Java', 'Java API to Generate OMR Template', 'Java OMR API', 'OMR Java', 'OMR Template from Text Markup']
categories: ['Aspose.OMR Product Family']
---



{{< figure align=center src="images/create-omr-template-from-text-markup-using-java.jpg" alt="Create OMR Template from Text Markup using Java">}}


OMR Templates are readable with Optical Mark Recognition (OMR) software or APIs. OMR software reads the information marked/ filled by people on surveys, tests, and other paper documents. We can easily generate OMR surveys, quizzes, or answer sheets from text markups programmatically. In this article, we will learn **how to create an OMR Template from text markup using Java**.

The following topics shall be covered in this article:

*   [Java API to Create OMR Template from Text Markup][1]
*   [Create OMR Survey Form from Text Markup][2]
*   [Create OMR Test from Text Markup][3]
*   [Generate Answer Sheet from Text Markup][4]

## Java API to Create OMR Template from Text Markup {#Java-API-to-Create-OMR-Template-from-Text-Markup}

For creating OMR templates from text markups, we will be using the [Aspose.OMR for Java API][5]. It allows designing, creating, and recognizing answer sheets, tests, MCQ papers, quizzes, feedback forms, surveys, and ballots. Please either [download][6] the JAR of the API or add the following _pom.xml_ configuration in a Maven-based Java application.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>http://repository.aspose.com/repo/</url>
</repository>
```
```
<dependency>
     <groupId>com.aspose</groupId>
     <artifactId>aspose-omr</artifactId>
     <version>19.12</version>
</dependency>
```

## Create OMR Survey Form from Text Markup using Java {#Create-OMR-Survey-Form-from-Text-Markup-using-Java}

We can create a survey form from text markup by following the steps given below:

*   Firstly, create an instance of the [_**OmrEngine**_][7] class.
*   Next, call the **_[GenerateTemplate][8]_** method with text markup file path as an argument.
*   After that, get results as an object of the **_[GenerationResult][9]_** class.
*   Finally, call the **_[Save][10]_** method to save template images and OMR template. It takes the path of the local disk folder and name of the template as arguments.

The following code example demonstrates **how to create an OMR survey template from text markup using Java**.

{{< gist aspose-com-gists fc68cf555dcca0e2a5050b989fe149eb "CreateOMRTemplateFromTextMarkup_Java_Generate.java" >}}

We have used the following text markup in the code example mentioned above.

{{< gist aspose-com-gists fc68cf555dcca0e2a5050b989fe149eb "CreateOMRTemplateFromTextMarkup_Java_SurveyMarkup.txt" >}}



{{< figure align=center src="images/Create-OMR-Survey-Form-from-Text-Markup-using-Java-724x1024.png" alt="OMR Survey from Text Markup" caption="OMR Survey from Text Markup">}}


## Create OMR Test from Text Markup using Java {#Create-OMR-Test-from-Text-Markup-using-Java}

We can create a quiz or a test by following the steps mentioned earlier. However, we just need to use the following text markup for this purpose.

{{< gist aspose-com-gists fc68cf555dcca0e2a5050b989fe149eb "CreateOMRTemplateFromTextMarkup_Java_TestMarkup.txt" >}}



{{< figure align=center src="images/Create-OMR-Test-from-Text-Markup-using-Java-724x1024.png" alt="OMR Test from Text Markup" caption="OMR Test from Text Markup">}}


## Generate OMR Answer Sheet from Text Markup using Java {#Generate-OMR-Answer-Sheet-from-Text-Markup-using-Java}

We can create a ready-to-print OMR answer sheet by following the steps mentioned earlier. However, we just need to use the following text markup for this purpose.

{{< gist aspose-com-gists fc68cf555dcca0e2a5050b989fe149eb "CreateOMRTemplateFromTextMarkup_Java_SheetMarkup.txt" >}}



{{< figure align=center src="images/Generate-OMR-Answer-Sheet-from-Text-Markup-using-Java-724x1024.png" alt="OMR Answer Sheet from Text Markup" caption="OMR Answer Sheet from Text Markup.">}}


## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][11] to try the library without evaluation limitations.

## Conclusion

In this article, we have learned **how to create an OMR survey template from text markup **and generate survey images. We have also seen **how to generate a quiz and an answer sheet from text markup** programmatically. Besides, you can learn more about Aspose.OMR for Java API using the [documentation][12]. In case of any ambiguity, please feel free to contact us on the [forum][13].

## See Also

*   [Create OMR Sheet Checker or Scanner with Java][14]




[1]: #Java-API-to-Create-OMR-Template-from-Text-Markup
[2]: #Create-OMR-Survey-Form-from-Text-Markup-using-Java
[3]: #Create-OMR-Test-from-Text-Markup-using-Java
[4]: #Generate-OMR-Answer-Sheet-from-Text-Markup-using-Java
[5]: https://products.aspose.com/omr/java/
[6]: https://downloads.aspose.com/omr/java
[7]: https://apireference.aspose.com/omr/java/com.aspose.omr/OmrEngine
[8]: https://apireference.aspose.com/omr/java/com.aspose.omr/OmrEngine#generateTemplate-java.lang.String-
[9]: https://apireference.aspose.com/omr/java/com.aspose.omr/GenerationResult
[10]: https://apireference.aspose.com/omr/java/com.aspose.omr/GenerationResult#save-java.lang.String-java.lang.String-
[11]: https://purchase.aspose.com/temporary-license
[12]: https://docs.aspose.com/omr/java/
[13]: https://forum.aspose.com/c/omr/38
[14]: https://blog.aspose.com/2021/08/05/create-omr-sheet-checker-or-scanner-with-java/




