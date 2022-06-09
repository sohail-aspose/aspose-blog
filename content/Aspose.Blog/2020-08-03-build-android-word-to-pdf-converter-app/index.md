---
title: 'Convert Word Documents to PDF using Android Library'
seoTitle: ""
description: ""
date: Mon, 03 Aug 2020 15:26:42 +0000
draft: false
url: /2020/08/03/build-android-word-to-pdf-converter-app/
author: Usman Aziz
summary: ''
tags: ['android word to pdf converter app', 'docx to pdf in android', 'word to pdf in android']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Word-to-PDF-Converter-in-Android.jpg" alt="Word to PDF Converter in Android">}}


The **Word to PDF** is one of the widely practiced document conversions and this is the reason [MS Word][1] provides a built-in feature to save Word documents as PDF. Since PDF is a preferred format for sharing the documents or keeping them online, the need for Word to PDF conversion occurs in various scenarios. On the other hand, Android-powered smartphones have made humans' life easier by putting a multitude of functionality within the phones via apps. Keeping an eye on these trends, in this article, I'll show you how to convert Word documents to PDF within an Android app. For demonstration, we'll build a simple **Word to PDF Converter app for Android** within a few steps having the following features.

*   Convert a Word document to PDF
*   Save PDF in phone's storage
*   View PDF within the app

## Word to PDF Converter Library for Android

For converting MS Word documents into PDF format, we'll use [Aspose.Words for Android via Java][2] that lets you convert DOC/DOCX documents to PDF files seamlessly using a couple of lines of code. You can either [download][3] the API or install it using the [Maven configuration][4].

## Steps to Convert Word to PDF in Android

The following are the steps to create a simple Word to PDF Converter app in Android using _Aspose.Words for Android via Java_:

*   Create a new project in Android Studio (or Eclipse) and select the "Empty Activity" template.



{{< figure align=center src="images/Create-a-New-Android-App.jpg" alt="create new project in android studio">}}


*   Configure your project.



{{< figure align=center src="images/Configure-Project.jpg" alt="Configure Android Project">}}


*   Open the **build.gradle** file.



{{< figure align=center src="images/Open-Build.Gradle-File.jpg" alt="update build.gradle in android studio">}}


*   Add the following repositories section in **build.gradle**.

```
repositories {
    mavenCentral()
    maven { url "https://repository.aspose.com/repo/" }
}
```

*   Add the following entries in the dependencies section of **build.gradle**.

```
implementation 'com.google.android.material:material:1.1.0'
implementation 'com.android.support:multidex:2.0.0'
implementation 'com.github.barteksc:android-pdf-viewer:2.8.2'
compile (group: 'com.aspose', name: 'aspose-words', version: '20.6', classifier: 'android.via.java')
```

*   Enable multidex by adding the following entry under the **defaultConfig** section in **build.gradle**.

```
// enable multiDex
multiDexEnabled true
```

*   The complete **build.gradle** file will look like the following:

{{< gist aspose-com-gists e3f39fb44100eb30caf6ff9af7172a29 "build.gradle" >}}

*   Open **activity\_main.xml** file.



{{< figure align=center src="images/Open-Layout.jpg" alt="update layout xml">}}


*   Paste the following script for the layout of the main activity.

{{< gist aspose-com-gists e3f39fb44100eb30caf6ff9af7172a29 "activity_main.xml" >}}

*   Open **MainActivity.java** file.



{{< figure align=center src="images/Open-MainActivity.jpg" alt="add word to pdf converter code">}}


*   Paste the following Java code in **MainActivity.java**.

{{< gist aspose-com-gists e3f39fb44100eb30caf6ff9af7172a29 "MainActivity.java" >}}

*   Build the app and run it within your Android smartphone or a virtual device.
*   Allow this app to access the storage by going to **Settings->Apps->Permissions->Permission manager->Storage**.



{{< figure align=center src="images/Android-Word-to-PDF-Converter.jpg" alt="Android Word to PDF Converter">}}


## Word to PDF Converter Android App - Demo

The following is the demonstration of how to convert a Word DOCX document to PDF using Word to PDF Converter app we have just created.

<figure class="wp-block-embed is-type-video is-provider-youtube wp-block-embed-youtube wp-embed-aspect-16-9 wp-has-aspect-ratio"><div class="wp-block-embed__wrapper">https://youtu.be/aEY96lOI6nI</div></figure>

## Word to PDF Convetrer - Source Code

Download the complete source code of Word to PDF Converter app from [GitHub][5].

## Conclusion

In this article, you have learned how to convert Word to PDF within Android apps. You can integrate similar functionality within your own app or enhance this converter up to your desired level. You may learn more about _Aspose.Words for Android via Java_ from the [documentation][6].

## See Also

*   [Convert Word to PDF using Java][7]




[1]: https://en.wikipedia.org/wiki/Microsoft_Word
[2]: https://products.aspose.com/words/android-java
[3]: https://downloads.aspose.com/words/androidjava
[4]: https://docs.aspose.com/display/wordsjava/Install+Aspose.Words+for+Android+via+Java#InstallAspose.WordsforAndroidviaJava-InstallAspose.WordsforAndroidviaJavafromMavenRepository
[5]: https://github.com/usman-aziz/Word-to-PDF-Converter-Android-App
[6]: https://docs.aspose.com/display/wordsjava/Supported+Document+Formats
[7]: https://blog.aspose.com/2020/02/20/convert-word-doc-docx-to-pdf-in-java-programmatically/





