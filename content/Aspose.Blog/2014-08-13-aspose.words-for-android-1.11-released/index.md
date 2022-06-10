---
title: 'Aspose.Words for Android 1.11 Released'
date: Wed, 13 Aug 2014 06:29:00 +0000
draft: false
url: /2014/08/13/aspose.words-for-android-1.11-released/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Total Product Family']
---

[![Aspose.Words for Android Logo][1]](http://www.aspose.com/android/word-component.aspx)We are pleased to announce a new release of Aspose.Words for Android. Aspose.Words for Android 1.11 sees the codebase better tweaked and the core functionality closer to Aspose.Words for Java/.NET 14.6.0, which is the product that Aspose.Words for Android is ported from.

You can download the latest release of Aspose.Words for Android from the following link:

*   [Aspose.Words for Android 1.11][2]

This release includes the following most notable improvements/fixes:

*   Support of automatic change tracking on a document.
*   Added vertical text support to HTML, EPUB  and MHT.
*   Footnote and endnote references now can be rendered as hyperlinks in output PDFs.
*   CJK (Chinese, Japanese, Korean) text is now properly rendered in multiline DrawingML textboxes.
*   Default text anti-aliasing on Java is optimized for Chinese, Japanese and Korean fonts.
*   Font substitution feature is added to public API.

## How to Use Aspose.Words for Android from 1.11 Onward

Previously, a single JAR of Aspose.Words for Android contained 47+ thousand methods which made older versions a little impractical to use in huge android applications. Now starting from this release, we have started to reduce the size of Aspose.Words for Android library. Our major concern now is to reduce the number of methods without loss of functionality. We are constantly working on improving the quality and usability of Aspose.Words for Android.

### Aspose.Words for Android Library Divided into Two Parts

We have divided the library into following two archives:

*   aspose-words-1.11-android-jdk15.jar: The first one includes public API and its auxiliary methods. Currently it has 32395 methods.
*   aspose-words-1.11-libs-android-jdk15.apk: The second one includes 3rd party jars, basic classes and resources. Currently, it has 18296 methods.

### Using Aspose Words for Android since 1.11

To include Aspose.Words for Android into the project you can use any of the following methods:

1\. To place "aspose-words-1.11-android-jdk15.jar" in the folder "libs" of your project, and the archive "aspose-words-1.11-libs-android-jdk15.apk" into the folder "assets".

Indicate that you are going to use AsposeWords application as the basic one.

[![][3]](https://blog.aspose.com/wp-content/uploads/sites/2/2014/08/Screenshot1.png)  

2\. to initiate the load of .apk file in the onCreate() method and if you do not want to use android:name="com.aspose.words.AsposeWordsApplication" in AndroidManifest.xml

### Using Aspose.Words for Android in Android Test Applications

To use Aspose.Words for Android in test projects, the same approach can be applied:

1\. Indicate AsposeWordsTestRunner in AndroidManifest.xml of the test project.

In IDE it might be necessary to indicate AsposeWordsTestRunner in the configuration window as follows:

2\. Or to initiate the load of .apk using the getTargetContext() method.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/09/aspose-Words-for-Android-e1401783855548.png "Aspose.Words for Android Logo"
[2]: http://www.aspose.com/community/files/74/android-components/aspose.words-for-android/default.aspx
[3]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/08/Screenshot1-300x161.png "Screenshot1"




