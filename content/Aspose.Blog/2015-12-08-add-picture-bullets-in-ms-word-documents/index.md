---
title: 'Add Picture Bullets in MS Word Documents using C# and Java'
date: Tue, 08 Dec 2015 12:57:20 +0000
draft: false
url: /2015/12/08/add-picture-bullets-in-ms-word-documents/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Aspose.Words 15.11.0 has been released. This month’s release contains over 146 useful new features, enhancements and bug fixes to the Aspose.Words products.

You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 15.11.0][1]
*   [Aspose.Words for Java 15.11.0][2]

Here is a look at just a few of the biggest features and API changes in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the links above.

*   Creation and deletion of picture bullet
*   Introduce public property ImageData in ListLevel
*   Introduce public overload DocumentBuilder.InsertCheckBox method
*   Introduce public property FormField.Default
*   Bookmarks with white-spaces are allowed in PDF, XPS and SWF
*   Introduce document-wide defaults formatting
*   OutlineOptions.CreateMissingOutlineLevels now works for bookmarks
*   Introduce public property UpdateFields in SaveOptions
*   ReportBuildOptions.AllowMissingDataFields is renamed to ReportBuildOptions.AllowMissingMembers

## Public Propery ListLevel.ImageData, Public Methods ListLevel.CreatePictureBullet and ListLevel.DeletePictureBullet Added

We have added DocumentBuilder.CreatePictureBullet and DocumentBuilder.DeletePictureBullet methods to create and delete picture bullets. Using ListLevel.ImageData you can get access to all available ImageData options. Please see the following code example to find out how to work with picture bullets.

```
string imageSrc = "Bullet1.png";

// Create a document and document builder.
Document doc = new Document();

DocumentBuilder builder = new DocumentBuilder(doc);

// Create a list.
List list = doc.Lists.Add(ListTemplate.BulletCircle);

// Configure list if necessary.
ListLevel listLevel0 = list.ListLevels[0];

// You can check HasPictureBullet property and ImageData (currently ImageData is null).
// listLevel0.HasPictureBullet;
// listLevel0.ImageData;

// Create picture bullet with default red cross image for the current list level.
listLevel0.CreatePictureBullet();

// Set your own picture bullet image through the ImageData.
listLevel0.ImageData.SetImage(imageSrc);

// Configure second level.
list.ListLevels[1].NumberStyle = NumberStyle.Arabic;

list.ListLevels[1].NumberFormat = "\u0001.";

// Configure next levels if necessary.

// Apply the list to the current paragraph.
builder.ListFormat.List = list;

builder.Writeln("item 1");

// Increase level.
builder.ListFormat.ListIndent();

builder.Writeln("item 1.1");
builder.Writeln("item 1.2");
builder.Writeln("item 1.3");

// Decrease level.
builder.ListFormat.ListOutdent();

builder.Write("item 2");

// Save output.
doc.Save("out_With_PictureBullet.docx");

// Lets delete picture bullet.
// Default bullet will be shown after deleting.
listLevel0 = doc.Lists[0].ListLevels[0];

// Delete picture bullet.
listLevel0.DeletePictureBullet();

// Save output.
doc.Save("out_Without_PictureBullet.docx"); 
```

## Public Overload of DocumentBuilder.InsertCheckBox Added

The following overload method of InsertCheckBox has been added to the DocumentBuilder class.

```
/// <summary>
/// Inserts a checkbox form field at the current position.
/// </summary>
/// <remarks>
/// If you specify a name for the form field, then a bookmark is automatically created with the same name.
/// </remarks>
/// <param name="name">The name of the form field. Can be an empty string.</param>
/// <param name="defaultValue">Default value of the checkbox form field.</param>
/// <param name="checkedValue">Current checked status of the checkbox form field.</param>
/// <param name="size">Specifies the size of the checkbox in points. Specify 0 for MS Word
/// to calculate the size of the checkbox automatically.</param>
/// <returns>The form field node that was just inserted.</returns>
public FormField InsertCheckBox(string name, bool defaultValue, bool checkedValue, int size) 
```

It allows defining default value and checked state of inserting check box separately. The behavior of the following existing overload is changed.

```
public FormField InsertCheckBox(string name, bool checkedValue, int size)
```

Now checkedValue value is also assigned as default value of check box. Default value had the 'false' value in the previous version. The checkedValue parameter of the overload has been renamed (old name: defaultValue).

## Public Property FormField.Default Added

FormField.Default property is used to get or set the default value of the check box form field. Default value for this property is false.

```
/// <summary>
/// Gets or sets the default value of the check box form field.
/// Default value for this property is <b>false</b>.
/// </summary>
/// <remarks>
/// Applicable for a check box form field only.
/// </remarks>
public bool Default
```

## Bookmarks With White Spaces are Allowed in PDF, XPS and SWF

WORDSNET-12531 is now resolved. In the previous versions of Aspose.Words it was not allowed to use bookmarks with white spaces in all document formats. All white spaces in the bookmarks were replaced with underscores. This restriction came from MS Word formats, since bookmarks in MS Word formats, like DOCX or DOC cannot have white spaces. However, PDF allows such bookmarks.

So now, if you need to use bookmarks in PDF, XPS or SWF outlines, you can use them with white spaces.

```
Document doc = new Document();
DocumentBuilder builder = new DocumentBuilder(doc);

builder.StartBookmark("My Bookmark");
builder.Writeln("Text inside a bookmark.");

builder.StartBookmark("Nested Bookmark");
builder.Writeln("Text inside a NestedBookmark.");
builder.EndBookmark("Nested Bookmark");

builder.Writeln("Text after Nested Bookmark.");
builder.EndBookmark("My Bookmark");

PdfSaveOptions options = new PdfSaveOptions();
options.OutlineOptions.BookmarksOutlineLevels.Add("My Bookmark", 1);
options.OutlineOptions.BookmarksOutlineLevels.Add("Nested Bookmark", 2);

doc.Save(MyDir + "Out.pdf", options);
```

In the document generated such way bookmarks in outlines will have white-spaces, that make it more convenient to read. Also if you have existing bookmarks and would like to use them in PDF outlines, you can replace underscores in bookmarks with white spaces.

```
foreach (Bookmark bookmark in doc.Range.Bookmarks)
{
    bookmark.Name = bookmark.Name.Replace("_", " ");
}
```

Note: behavior for all other formats was not changed. White spaces in bookmarks are replaced with underscores upon saving to all flow formats.

## Public Properties DefaultParagraphFormat and DefaultFont Added to StyleCollection

WORDSNET-4079 is now resolved. We have added new public properties DefaultParagraphFormat and DefaultFont to StyleCollection class.

```
Font Document.Styles.DefaultFont;
ParagraphFormat Document.Styles.DefaultParagraphFormat;
```

**Use Case**

```
Document doc = new Document();
doc.Styles.DefaultFont.NameFarEast = "PMingLiU";
```

**Use Case**

```
Document doc = new Document();
doc.Styles.DefaultParagraphFormat.SpaceAfter = 20;
```

Note that document-wide defaults were introduced in Microsoft Word 2007 and are fully supported in OOXML formats only. Earlier document formats have limited support for default text formatting (only font names can be stored) and have no support for default paragraph formatting (default paragraph formatting is copied to all top level styles when it is not supported in target document format).

## OutlineOptions.CreateMissingOutlineLevels Now Works for Bookmarks

In the previous versions of Aspose.Words with this option enabled missing outline levels was created only for headings. Now missing outline levels are created both for headings and bookmarks.

```
/// <summary>
/// <para>Gets or sets a value determining whether or not to create missing outline levels when the document is
/// exported.</para>
/// <para>Default value for this property is <b>false</b></para>
/// </summary>
public bool CreateMissingOutlineLevels { get; set; }
```

## Public Property SaveOptions.UpdateFields Added

We have added new public property UpdateFields to SaveOptions class. This property gets or sets a value determining if fields should be updated before saving the document to a fixed page format. Default value for this property is true.

```
/// <summary>
/// Gets or sets a value determining if fields should be updated before saving the document to a fixed page format.
/// Default value for this property is <b>true</b>
/// </summary>
public bool UpdateFields {get;set;}
```

## ReportBuildOptions.AllowMissingDataFields is Renamed to ReportBuildOptions.AllowMissingMembers

ReportBuildOptions.AllowMissingDataFields affected only fields of DataRow and IDataRecord instances. In previous versions of Aspose.Words this enumeration does not work for master-detail relationships. That is why, the option was renamed.

```
/// <summary>
/// Specifies that missing object members should be treated as null literals by the engine. This option
/// affects only access to instance (that is, non-static) object members and extension methods. If this
/// option is not set, the engine throws an exception when encounters a missing object member.
/// </summary>
AllowMissingMembers = 1
```




[1]: https://products.aspose.com/words/net
[2]: https://products.aspose.com/words/java




