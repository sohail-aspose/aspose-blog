---
title: 'Protect or Unprotect MS Word Documents using Java'
seoTitle: ""
description: ""
date: Tue, 10 Nov 2020 22:28:46 +0000
draft: false
url: /2020/11/10/protect-or-unprotect-ms-word-files-using-java/
author: Usman Aziz
summary: 'MS Word allows you to protect the DOCX document with various mechanisms. You can set a password that is required to open the document. On the other hand, you can specify the protection levels such as making the document read-only, allowing comments or form fields only, and etc. In this article, you are going to learn how to automate the MS Word protection features in order to **protect or unprotect DOCX files in Java-based applications**.'
tags: ['protect word docx in java', 'unlock word docx in java', 'unprotect word docx in java']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Protect-Unprotect-Word-C.png" alt="Protect or Unprotect DOCX in Java">}}


MS Word allows you to protect the DOCX document with various mechanisms. You can set a password that is required to open the document. On the other hand, you can specify the protection levels such as making the document read-only, allowing comments or form fields only, and etc. In this article, you are going to learn how to automate the MS Word protection features in order to **protect or unprotect DOCX files in Java-based applications**.

*   [Java API to Protect or Unprotect Word Documents][1]
*   [Protect Word DOCX Files with Password in Java][2]
*   [Secure DOCX Files with Different Protection Types][3]
*   [Unprotect/Unlock DOCX Files using Java][4]

## Java API to Protect or Unprotect Word Files - Free Download {#Java-API-to-Protect-or-Unprotect-MS-Word-Documents}

[Aspose.Words for Java][5] is a powerful word processing API that lets you create and process MS Word documents from within your Java-based applications. In addition, it allows automating the security features in order to protect or unprotect Word DOCX documents. You can either [download][6] the API or get it installed in your Maven-based application.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
```
```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-words</artifactId>
    <type>pom</type>
</dependency>
```

## Protect Word DOCX File with Password in Java {#Protect-Word-DOCX-File-with-Password-in-Java}

The following are the simple steps to protect a Word DOCX document using a password.

*   Load the DOCX file using [Document][7] class.
*   Protect the Word document using [Document.protect(int, java.lang.String)][8]/) method.
*   Save the protected document using the [Document.save()][9] method.

The following code samples shows how to protect a Word DOCX document using Java.

{{< gist aspose-com-gists 4351f6ce87d8aaa77ceee87609e9302a "protect-docx-password.java" >}}

## Protect DOCX Files with Different Protection Types {#Secure-DOCX-Files-with-Different-Protection-Types}

You can also restrict the user's access to the document with different protection levels. In this case, the user will only be authorized to perform a certain set of operations. Aspose.Words for Java provides the following protection types:

*   **AllowOnlyComments **– To allow modification of comments only.
*   **AllowOnlyFormFields **– To allow data entry into the form fields only.
*   **AllowOnlyRevisions **– To allow adding revision marks only.
*   **ReadOnly **– Completely read-only (no changes are allowed to the document).
*   **NoProtection **– No protection at all.

The following code sample shows how to apply a particular protection type in DOCX without a password.

{{< gist aspose-com-gists 4351f6ce87d8aaa77ceee87609e9302a "add-protection-to-docx.java" >}}

## Unprotect/Unlock DOCX Files using Java {#Unprotect/Unlock-DOCX-Files-using-Java}

Aspose.Words for Java lets you unprotect or unlock MS Word DOCX files in a couple of lines of code. Not only this, but you can unprotect the files without providing the password. The following are the steps to unlock a protected DOCX file.

*   Load the DOCX file using [Document][10] class.
*   Unprotect DOCX file using [Document.unprotect()][11]/) method.
*   Save the unlocked file using the [Document.save()][12] method.

The following code sample shows how to unprotect a Word DOCX file using Java.

{{< gist aspose-com-gists 4351f6ce87d8aaa77ceee87609e9302a "unprotect-docx.java" >}}

## Conclusion

In this article, you have learned how to protect or unprotect MS Word DOCX files using Java. Furthermore, you have seen how different protection types can be applied to a DOCX file. You can explore more about Aspose.Words for Java using [documentation][13].

## See Also

*   [Merge MS Word Documents using Java][14]




[1]: #Java-API-to-Protect-or-Unprotect-MS-Word-Documents
[2]: #Protect-Word-DOCX-File-with-Password-in-Java
[3]: #Secure-DOCX-Files-with-Different-Protection-Types
[4]: #Unprotect/Unlock-DOCX-Files-using-Java
[5]: https://products.aspose.com/words/java
[6]: https://downloads.aspose.com/words/java
[7]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[8]: http://www.aspose.com/api/java/words/com.aspose.words/classes/document/methods/protect(int,java.lang.String
[9]: https://apireference.aspose.com/words/java/com.aspose.words/document#save(java.lang.String)
[10]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[11]: http://www.aspose.com/api/java/words/com.aspose.words/classes/document/methods/unprotect(
[12]: https://apireference.aspose.com/words/java/com.aspose.words/document#save(java.lang.String)
[13]: https://docs.aspose.com/words/java/getting-started/
[14]: https://blog.aspose.com/2020/09/10/merge-ms-word-documents-using-java/





