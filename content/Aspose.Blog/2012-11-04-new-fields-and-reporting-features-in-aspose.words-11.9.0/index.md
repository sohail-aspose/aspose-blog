---
title: 'New Fields and Reporting Features in Aspose.Words 11.9.0'
date: Sun, 04 Nov 2012 09:30:19 +0000
draft: false
url: /2012/11/04/new-fields-and-reporting-features-in-aspose.words-11.9.0/
author: DmitryV
summary: ''
tags: ['ASK', 'Image', 'fields', 'fillin', 'lock fields in word document', 'locked fields', 'mail merge', 'reporting', 'set image merge field in word', 'template']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose.words-logo2.jpg" alt="">}}


We have just released this month’s improvements to Aspose.Words for .NET and Java. This month’s release includes numerous improvements to many areas of our components as well as many new exciting features.

You can immediately download our latest Aspose.Words release from the following links:

*   [Aspose.Words for .NET 11.9.0][1]
*   [Aspose.Words for Java 11.9.0][2]

Throughout October we have added a number of interesting features to the fields and reporting area which are explained in detail below.

## ASK and FILLIN Fields

ASK and FILLIN fields, when updated, prompt the user to enter information and store it in the document. In the past, users had to implement a workaround to handle these fields and obtain a response. Starting with Aspose.Words 11.9 the support for these fields is built in.

To enable interaction between these fields and the user, you should implement the **IFieldUserPromptRespondent** interface and assign a respondent object to the **Document.FieldOptions.UserPromptRespondent** property.

The **IFieldUserPromptRespondent** interface contains a single method named **Respond** which can be implemented in various ways. For example, it could simply show the prompting window and return user's response in case of desktop application (like in Microsoft Word). The following example is simple but provides the basic idea of how this system works:

```
string IFieldUserPromptRespondent.Respond(string promptText, string defaultResponse)
{
    return (promptText == "Please enter your age" ? "32" : null);
}
```

For more information please see the **IFieldUserPromptRespondent** interface and its members.

## Image Size for Image Merge Fields

It is well known that Aspose.Words has a very useful feature which allows you to easily insert images into the document during mail merge. To insert an image, you should designate a placeholder using a merge field whose name looks like _Image:FieldName_.

In Aspose.Words 11.9, we have added the ability of the specifying image size for such fields. It can be accomplished using one of the two approaches described below.

### Specifying Image Size in Document

The first approach is specifying image size directly in the field’s name:



{{< figure align=center src="images/MailMergeImageSizeSet.png" alt="">}}


The format of the image merge field's name with image size specified is as follows:

_Image(width\[pt|%\];height\[pt|%\]):FieldName_

The format is case-insensitive. The values of the width and the height should represent double constant values using the dot as the decimal separator (i.e. using invariant culture). Negative values should be used to indicate that the original values of the corresponding image dimensions should be used. If no unit is specified, points are used by default. If a unit other than "pt" or "%" is specified, then the image size parsing is considered to be failed and the original values of the corresponding image dimensions are used.

### Specifying Image Size in Code

The second approach is to specify image size via new properties of the **ImageFieldMergingArgs** class: **ImageWidth** and **ImageHeight**. The values of these properties can be initially populated from the merge field in the template by using the image size defined in the field name as discussed in the previous section.

Below are some examples of how to use these properties:

```
void IFieldMergingCallback.ImageFieldMerging(ImageFieldMergingArgs args)
{
    args.ImageFileName = "Image.png";
    args.ImageWidth.Value = 200;
    args.ImageHeight = new MergeFieldImageDimension(200,
        MergeFieldImageDimensionUnit.Percent);
}
```
```
void IFieldMergingCallback.ImageFieldMerging(ImageFieldMergingArgs args)
{
    args.ImageFileName = "Image.png";
    args.ImageWidth = null;
    args.ImageHeight = new MergeFieldImageDimension(-1);
}
```

Note that the code in the second example will lead to the original image size (i.e. both width and height) to be used when merging the field. For more information please see the **ImageFieldMergingArgs** and **MergeFieldImageDimension** classes.

## Locked Fields

Locked fields are any field whose result should not be updated (Ctrl-F11 to lock a field in Word, Ctrl-Shift-F11 to unlock). Starting with Aspose.Words 11.9.0 locked fields are now supported. You can control whether a field is locked through the API by using the following new properties:

*   **Field.IsLocked**
*   **FieldChar.IsLocked** and subsequently **FieldStart.IsLocked**, **FieldSeparator.IsLocked**, and **FieldEnd.IsLocked**

Note that **Field.IsLocked** is currently only useful when a field is just inserted via **DocumentBuilder.InsertField()**:

```
DocumentBuilder builder = new DocumentBuilder();
Field field = builder.InsertField("=2+2", "5");
field.IsLocked = true;
// No update is performed, the incorrect result is preserved.
field.Update();
```

In any other cases, please use **FieldStart.IsLocked**. Although **FieldStart.IsLocked**, **FieldSeparator.IsLocked**, and **FieldEnd.IsLocked** are essentially the same when reading or writing document, it is recommended that you use **FieldStart.IsLocked** in your code because its value is considered by Aspose.Words' field update logic.




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.words-for-.net/category1188.aspx
[2]: http://www.aspose.com/community/files/72/java-components/aspose.words-for-java/category1378.aspx




