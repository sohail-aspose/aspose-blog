---
title: 'Support of Ancient Legacy Binary DOC, Introduced New InsertSignatureLine methods and Configuration of Document Hyphenation Options, Added Feature to Get Mail Merge Regions Hierarchy in Aspose.Words 16.1.0'
date: Wed, 17 Feb 2016 15:49:31 +0000
draft: false
url: /2016/02/17/support-of-ancient-legacy-binary-doc-introduced-new-insertsignatureline-methods-and-configuration-of-document-hyphenation-options-added-feature-to-get-mail-merge-regions-hierarchy/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

[](http://www.aspose.com/.net/word-component.aspx)Aspose.Words 16.1.0 has been released. This month’s release contains over 139 useful new features, enhancements and bug fixes to the Aspose.Words products.

You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 16.1.0][1]
*   [Aspose.Words for Java 16.1.0][2]

Here is a look at just a few of the biggest features and API changes in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the links above.

*   Support of Ancient Legacy Binary DOC files
*   Support of Configuration of Document Hyphenation Options
*   Support of Controlling Global Mail Merge Events
*   Support of Getting Mail Merge Regions Hierarchy
*   Support of Working without Static Font Cache and Use Per-document Font Settings
*   Introduced Public Fields API v2.0 - Building Arbitrary Field Using FieldBuilder
*   Introduced HtmlSaveOptions.ExportPageMargins Property
*   Introduced ImageSaveOptions.UseGdiEmfRenderer Property
*   Introduced HtmlFixedSaveOptions.ExportFormFields Property
*   Introduced MailMerge.PreserveUnusedTags Property
*   Introduced Shape.SignatureLine Property
*   Introduced FormField.RemoveField Method
*   Introduced DocumentBuilder.InsertSignatureLine Method
*   Improved Font Substitution Warnings

## Support of Ancient Legacy Binary DOC files

We have added support for older binary DOC format for Word6.0/Word95 documents import. We have renamed Public enumeration LoadFormat.DocPreWord97 to DocPreWord60 to avoid confusion.

## Support of Configuration of Document Hyphenation Options

We introduced new HyphenationOptions class in Aspose.Words. HyphenationOptions instance is available as a read only property on the Document class and contains the following properties to configure document hyphenation options:

```
/// <summary>
/// Gets or sets value determining whether automatic hyphenation is turned on for the document.
/// Default value for this property is <b>false</b>.
/// </summary>
public bool AutoHyphenation {get;set;}

/// <summary>
/// Gets or sets the maximum number of consecutive lines that can end with hyphens.
/// Default value for this property is 0.
/// </summary>
/// <remarks>
/// If value of this property is set to 0, any number of consecutive lines can end with hyphens.
/// The property does not have effect when saving to fixed page formats e.g. PDF.
/// </remarks>
public int ConsecutiveHyphenLimit {get;set;}

/// <summary>
/// Gets or sets the distance in 1/20 of a point from the right margin within which you do not want
/// to hyphenate words.
/// Default value for this property is 360 (0.25 inch).
/// </summary>
public int HyphenationZone {get;set;}

/// <summary>
/// Gets or sets value determining whether words written in all capital letters are hyphenated.
/// Default value for this property is <b>true</b>.
/// </summary>
public bool HyphenateCaps {get;set;} 
```

Following code example shows how to use HyphenationOptions's properties.

```
Document doc = new Document();
doc.HyphenationOptions.AutoHyphenation = true;
doc.HyphenationOptions.ConsecutiveHyphenLimit = 2;
doc.HyphenationOptions.HyphenationZone = 720; // 0.5 inch
doc.HyphenationOptions.HyphenateCaps = false; 
```

## Support of Controling Global Mail Merge Events

We have added the IMailMergeCallback interface to receive notifications while mail merge is performed and MailMerge.MailMergeCallback property to handle particular events during mail merge. This allows to respond to different global mail merge events. Currently it supports a single event, TagsReplaced, which is fired when mustache fields are replaced with merge fields but not yet merged.

```
/// <summary>
/// Allows to handle particular events during mail merge.
/// </summary>
public IMailMergeCallback MailMergeCallback

/// <summary>
/// Implement this interface if you want to receive notifications while mail merge is performed.
/// </summary>
public interface IMailMergeCallback
{
    /// <summary>
    /// Called when "mustache" text tags are replaced with MERGEFIELD fields.
    /// </summary>
    /// <seealso cref="MailMerge.UseNonMergeFields"/>
    void TagsReplaced();
} 
```

## Support of Geting Mail Merge Regions Hierarchy

We have added the MailMergeRegionInfo public class and the MailMerge.GetRegionsHierachy public method. These allow to obtain mail merge hierarchy including child regions and fields.

```
public class MailMergeRegionInfo
{

    /// <summary>
    /// Returns a list of child regions.
    /// </summary>
    public ArrayList Regions { get; }

    /// <summary>
    /// Returns a list of child merge fields.
    /// </summary>
    public ArrayList Fields { get; }

    /// <summary>
    /// Returns the name of region.
    /// </summary>
    public string Name { get; }

    /// <summary>
    /// Returns a start field for the region.
    /// </summary>
    public FieldMergeField StartField { get; }

    /// <summary>
    /// Returns an end field for the region.
    /// </summary>
    public FieldMergeField EndField { get; set; }
} 
```

## Support of Working Without Static Font Cache and Use Per-document Font Settings

We have made all methods of FontSettings class as instance methods. Static methods are replaced with static DefaultInstance property. **This is a breaking change.**

```
/// <summary>
/// Specifies font settings for a document.
/// </summary>
/// <remarks>
/// <para>Aspose.Words uses font settings to resolve the fonts in the document. Fonts are resolved mostly when building document layout
/// or rendering to fixed page formats. But when loading some formats, Aspose.Words also may require to resolve the fonts. For example, when
/// loading HTML documents Aspose.Words may resolve the fonts to perform font fallback. So it is recommended that you set the font settings in
/// <see cref="LoadOptions"/> when loading the document. Or at least before building the layout or rendering the document to the fixed-page format.</para>
///
/// <para>By default all documents uses single static font settings instance. It could be accessed by
/// <see cref="DefaultInstance"/> property.</para>
///
/// <para>Changing font settings is safe at any time from any thread. But it is recommended that you do not change the font settings while
/// processing some documents which uses this settings. This can lead to the fact that the same font will be resolved differently
/// in different parts of the document.</para>
/// </remarks>
public class FontSettings
{
    public void SetFontsFolder(string fontFolder, bool recursive);
    public void SetFontsFolders(string[] fontsFolders, bool recursive);
    public void SetFontsSources(FontSourceBase[] sources);
    public FontSourceBase[] GetFontsSources();
    public void ResetFontSources();
    public string DefaultFontName;
    public string[] GetFontSubstitutes(string originalFontName);
    public void SetFontSubstitutes(string originalFontName, params string[] substituteFontNames);
    public void AddFontSubstitutes(string originalFontName, params string[] substituteFontNames);

    /// <summary>
    /// Static default font settings.
    /// </summary>
    /// <remarks>
    /// This instance is used by default in a document unless <see cref="Document.FontSettings"/> is specified.
    /// </remarks>
    public static FontSettings DefaultInstance
    {
        get { return gDefaultInstance; }
    }
} 
```

## Introduced Public Fields API v2.0 - Building Arbitrary Field Using FieldBuilder

We have now provided typed access to all Microsoft Word fields, it is a good time to allow users build an arbitrary field code. We can insert a complete field code via DocumentBuilder, or we can insert a field of a certain type and access its code using the typed properties of a FieldXXX class.

Below are skeletons of proposed classes responsible for building a field. They support nested fields and arbitrary document nodes. They also expose a bunch of methods for convenient insertion of field argument and switches.

```
namespace Aspose.Words.Fields
{
    /// <summary>
    /// Builds a field from field code tokens(arguments and switches).
    /// </summary>
    public class FieldBuilder
    {
        /// <summary>
        /// Initializes an instance of the <see cref="FieldBuilder"/> class.
        /// </summary>
        /// <param name="fieldType"></param>
        public FieldBuilder(FieldType fieldType)
        {
            throw new NotImplementedException();
        }

        /// <summary>
        /// Adds a field's argument.
        /// </summary>
        /// <remarks>
        /// Unlike <see cref="AddText"/>, separates the text with spaces and encloses it into double quotes if needed.
        /// </remarks>
        /// <param name="argument"></param>
        public FieldBuilder AddArgument(string argument)
        {
            throw new NotImplementedException();
        }

        /// <summary>
        /// Adds a field's argument.
        /// </summary>
        /// <param name="argument"></param>
        public FieldBuilder AddArgument(int argument)
        {
            throw new NotImplementedException();
        }

        /// <summary>
        /// Adds a field's argument.
        /// </summary>
        /// <param name="argument"></param>
        public FieldBuilder AddArgument(double argument)
        {
            throw new NotImplementedException();
        }

        /// <summary>
        /// Adds a child field represented by another <see cref="FieldBuilder"/> to the field's code.
        /// </summary>
        /// <remarks>
        /// This overload is used when the argument consists of a single child field.
        /// </remarks>
        /// <param name="childField"></param>
        /// <returns></returns>
        public FieldBuilder AddArgument(FieldBuilder argument)
        {
            throw new NotImplementedException();
        }

        /// <summary>
        /// Adds a child field represented by another <see cref="FieldBuilder"/> to the field's code.
        /// </summary>
        /// <remarks>
        /// This overload is used when the argument consists of a mixture of different parts such as child fields, nodes, and plain text.
        /// </remarks>
        /// <param name="argument"></param>
        /// <returns></returns>
        public FieldBuilder AddArgument(FieldArgumentBuilder argument)
        {
            throw new NotImplementedException();
        }

        /// <summary>
        /// Adds a field's switch.
        /// </summary>
        /// <remarks>
        /// This overload adds a flag (switch without argument).
        /// </remarks>
        /// <param name="switchName"></param>
        public FieldBuilder AddSwitch(string switchName)
        {
            throw new NotImplementedException();
        }

        /// <summary>
        /// Adds a field's switch.
        /// </summary>
        /// <param name="switchName"></param>
        /// <param name="switchArgument"></param>
        public FieldBuilder AddSwitch(string switchName, string switchArgument)
        {
            throw new NotImplementedException();
        }

        /// <summary>
        /// Adds a field's switch.
        /// </summary>
        /// <param name="switchName"></param>
        /// <param name="switchArgument"></param>
        public FieldBuilder AddSwitch(string switchName, int switchArgument)
        {
            throw new NotImplementedException();
        }

        /// <summary>
        /// Adds a field's switch.
        /// </summary>
        /// <param name="switchName"></param>
        /// <param name="switchArgument"></param>
        public FieldBuilder AddSwitch(string switchName, double switchArgument)
        {
            throw new NotImplementedException();
        }

        /// <summary>
        /// Builds and inserts a field into the document.
        /// </summary>
        /// <param name="refNode"></param>
        /// <param name="isAfter"></param>
        /// <returns></returns>
        public Field BuildAndInsert(Node refNode, bool isAfter)
        {
            throw new NotImplementedException();
        }
    }

    /// <summary>
    /// Builds a complex field argument consisting of fields, nodes, and plain text.
    /// </summary>
    public class FieldArgumentBuilder
    {
        /// <summary>
        /// Adds a plain text to the argument.
        /// </summary>
        /// <param name="text"></param>
        /// <returns></returns>
        public FieldArgumentBuilder AddText(string text)
        {
            throw new NotImplementedException();
        }

        /// <summary>
        /// Adds an arbitrary node to the argument.
        /// </summary>
        /// <param name="node"></param>
        /// <returns></returns>
        public FieldArgumentBuilder AddNode(Node node)
        {
            throw new NotImplementedException();
        }

        /// <summary>
        /// Adds a field represented by a <see cref="FieldBuilder"/> to the argument.
        /// </summary>
        /// <param name="fieldBuilder"></param>
        /// <returns></returns>
        public FieldArgumentBuilder AddField(FieldBuilder fieldBuilder)
        {
            throw new NotImplementedException();
        }
    }
} 
```

Following code snippet shows how to use FieldBuilder.

```
 FieldBuilder builder = new FieldBuilder(FieldType.FieldIf);

builder
    .AddArgument(new FieldBuilder(FieldType.FieldMergeField).AddArgument("CustomerName"))
    .AddArgument("=")
    .AddArgument("John Smith")
    .AddArgument(10)
    .AddArgument(20)
    .BuildAndInsert(refNode, true); 
```

## Introduced HtmlSaveOptions.ExportPageMargins Property

We have now added a new public property to HtmlSaveOptions class to specify whether page margins is exported to HTML, MHTML or EPUB.

```
/// <summary>
/// Specifies whether page margins is exported to HTML, MHTML or EPUB.
/// Default is <c<false</c<.
/// </summary>
/// <remarks>
/// Aspose.Words does not show area of page margins by default.
/// If any elements are completely or partially clipped by the document edge the displayed area can be extended with this option.
/// </remarks>
public bool ExportPageMargins
{
   get { return mExportPageMargins; }
   set { mExportPageMargins = value; }
} 
```

## Introduced ImageSaveOptions.UseGdiEmfRenderer Property

Now Aspose.Words could save metafiles directly without using GDI+. For now only saving to EmfPlusOnly format is supported. In Aspose.Words for .NET version this is controlled by the flag in ImageSaveOptions.

```
/// <summary>
/// Gets or sets a value determining whether to use GDI+ or Aspose.Words metafile renderer when saving to EMF.
/// </summary>
/// <remarks>
/// <para<If set to <c<true</c< GDI+ metafile renderer is used. I.e. content is written to GDI+ graphics
/// object and saved to metafile.</para<
/// <para<If set to <c<false</c< Aspose.Words metafile renderer is used. I.e. content is written directly
/// to the metafile format with Aspose.Words.</para<
/// <para<The default value is <c<true</c<.</para<
/// <para<Has effect only when saving to EMF.</para<
/// </remarks>
public bool UseGdiEmfRenderer; 
```

## Introduced HtmlFixedSaveOptions.ExportFormFields Property

We have now added a new public property to HtmlFixedSaveOptions class to get/set indication of whether form fields are exported as interactive items (as 'input' tag) rather than converted to text or graphics.

```
/// <summary>
/// Gets or sets indication of whether form fields are exported as interactive
/// items (as 'input' tag) rather than converted to text or graphics.
/// </summary>
public bool ExportFormFields
{
   get { return mExportFormFields; }
   set { mExportFormFields = value; }
} 
```

## Introduced MailMerge.PreserveUnusedTags Property

We have added a capability to preserve mustache tags that haven't been populated.

```
/// <summary>
/// Gets or sets a value indicating whether the unused "mustache" tags should be preserved.
/// </summary>
/// <remarks>
/// The default value is <b<false</b<.
/// </remarks>
/// <seealso cref="UseNonMergeFields"/<
public bool PreserveUnusedTags 
```

## Introduced DocumentBuilder.InsertSignatureLine Method

We have added following two methods to DocumentBuilder class to insert signature lines.

```
/// <summary>
/// Inserts a signature line at the current position.
/// </summary>
/// <param name="signatureLineOptions"<The object that stores parameters of creating signature line .</param<
/// <returns<The signature line node that was just inserted.</returns<
public Shape InsertSignatureLine(SignatureLineOptions signatureLineOptions);

/// <summary>
/// Inserts a signature line at the specified position.
/// </summary>
/// <param name="signatureLineOptions"<The object that stores parameters of creating signature line.</param<
/// <param name="horzPos"<Specifies where the distance to the signature line is measured from.</param<
/// <param name="left"<Distance in points from the origin to the left side of the signature line.</param<
/// <param name="vertPos"<Specifies where the distance to the signature line measured from.</param<
/// <param name="top"<Distance in points from the origin to the top side of the signature line.</param<
/// <param name="wrapType"<Specifies how to wrap text around the signature line.</param<
/// <returns<The signature line node that was just inserted.</returns<
public Shape InsertSignatureLine(SignatureLineOptions signatureLineOptions, RelativeHorizontalPosition horzPos,
    double left, RelativeVerticalPosition vertPos, double top, WrapType wrapType); 
```

Following code example shows how to insert signature line.

```
 Document doc = new Document();
DocumentBuilder builder = new DocumentBuilder(doc);

SignatureLineOptions options = new SignatureLineOptions();
options.Signer = "John Doe";
options.SignerTitle = "Manager";
options.ShowDate = false;
builder.InsertSignatureLine(options); 
```

## Introduced Shape.SignatureLine Property

We have now added Shape.SignatureLine property to get SignatureLine object if the shape is a signature line. Note! Now it is not possible to sign a signature line by digital signature in Aspose.Words.

```
/// <summary>
/// Gets <see cref="SignatureLine"/< object if the shape is a signature line. Returns <b<null</b< otherwise.
/// </summary>
/// <remarks>You can insert new SignatureLines into the document using <see cref="DocumentBuilder.InsertSignatureLine(SignatureLineOptions)"/< and
/// <seealso cref="DocumentBuilder.InsertSignatureLine(SignatureLineOptions, RelativeHorizontalPosition, double, RelativeVerticalPosition, double, WrapType)"/<</remarks>
public SignatureLine SignatureLine; 
```

## Introduced FormField.RemoveField Method

We have added a capability to remove the whole form field right from the FormField object.

```
/// <summary>
/// Removes the complete form field, not just the form field special character.
/// </summary>
/// <remarks>
/// If there is a bookmark associated with the form field, the bookmark is not removed.
/// </remarks>
public void RemoveField() 
```




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.words-for-.net/default.aspx
[2]: http://www.aspose.com/community/files/72/java-components/aspose.words-for-java/default.aspx




