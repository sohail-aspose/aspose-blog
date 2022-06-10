---
title: 'Add and Remove Embedded Fonts, Save Document Page to GIF Format, and many more with Aspose.Words 16.7.0'
date: Fri, 12 Aug 2016 14:57:00 +0000
draft: false
url: /2016/08/12/support-of-add-and-remove-embedded-fonts-export-mathml-to-image-and-text-support-of-skipif-field-improved-font-substitution-rules-in-aspose.words-16.7.0/
author: Tahir Manzoor
summary: ''
tags: ['add embedded fonts', 'embed font word document', 'embed fonts in word', 'embed fonts to documents', 'embedded fonts in documents', 'font substitution in document', 'remove embedded fonts', 'word embed font', 'word embed fonts', 'word to gif']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose-Words-for-net-e1378287014402.png" alt="Aspose.Words for .NET logo">}}


Aspose.Words 16.7.0 has been released. This month’s release contains over 132 useful new features, enhancements and bug fixes to the Aspose.Words product.

You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 16.7.0][1]
*   [Aspose.Words for Java 16.7.0][2]

Here is a look at just a few of the biggest features and API changes in this month’s release.

*   Save Document Page in GIF Format.
*   Exposed more String and Number Formats for Expression Results in LINQ Reporting Engine.
*   SKIPIF field supported.
*   Support for MathML in HTML Export.
*   Support of Add and Remove Embedded Fonts.
*   Improved Font Substitution Rules.
*   MsWordVersion Enum Moved to Aspose.Words.Settings.
*   ReplaceAction, IReplacingCallback and ReplacingArgs Moved to Aspose.Words.Replacing.
*   Added Advanced Range.Replace methods.
*   Added Overload of DigitalSignatureUtil.Sign to Specify a Password for Decrypting Document.

## Save Document Page in GIF Format.

We have introduced new feature in Aspose.Words 16.7.0 to save a Document page to GIF format. A new 'Gif' member is added into 'SaveFormat' enum. Aspose.Words for .Net uses standard GIF codec provided by GDI+. Aspose.Words for Java uses standard GIF codec provided by ImageIO.

```
// Open some document.
Document doc = new Document("mydocument.docx");

// Save the second page as GIF image.
ImageSaveOptions saveOptions = new ImageSaveOptions(SaveFormat.Gif);
saveOptions.PageIndex = 1;
doc.Save("mydocument.gif", saveOptions);
```

## Exposed more String and Number Formats for Expression Results in LINQ Reporting Engine.

More String and Number formats for expression results are introduced in LINQ Reporting Engine. Please check "Outputting Expression Results".

## SKIPIF field supported.

We have introduced new feature in Aspose.Words 16.7.0 to support SKIPIF field. This field is now updated during mail merge.

## Support for MathML in HTML Export.

We have added the HtmlSaveOptions.OfficeMathOutputMode property in Aspose.Wrods v16.7.0 to control how OfficeMath objects are exported to HTML, MHTML or EPUB.

```
/// <summary>
/// Controls how OfficeMath objects are exported to HTML, MHTML or EPUB.
/// Default value is <c>HtmlOfficeMathOutputMode.Image</c>.
/// </summary>
public HtmlOfficeMathOutputMode OfficeMathOutputMode
{
    get { return mOfficeMathOutputMode; }
    set { mOfficeMathOutputMode = value; }
} 
```

HtmlOfficeMathOutputMode enumeration

```
/// <summary>
/// Specifies how Aspose.Words exports OfficeMath to HTML, MHTML and EPUB.
/// </summary>
public enum HtmlOfficeMathOutputMode
{
    /// <summary>
    /// OfficeMath is converted to HTML as image specified by <img> tag.
    /// </summary>
    Image,
    /// <summary>
    /// OfficeMath is converted to HTML using MathML.
    /// </summary>
    MathML,
    /// <summary>
    /// OfficeMath is converted to HTML as sequence of runs specified by <span> tags.
    /// </summary>
    Text
}
```

Sample output for simple OfficeMath equation exported using HtmlOfficeMathOutputMode.Image value:

```
<img src="Test Out.001.png" width="49" height="21" alt="" />
```

Sample output for simple OfficeMath equation exported using HtmlOfficeMathOutputMode.MathML value:

```
<math xmlns="http://www.w3.org/1998/Math/MathML">
	<mi>A</mi>
	<mo>=</mo>
	<mi>π</mi>
	<msup>
		<mrow>
			<mi>r</mi>
		</mrow>
		<mrow>
			<mn>2</mn>
		</mrow>
	</msup>
</math>
```

Sample output for simple OfficeMath equation exported using HtmlOfficeMathOutputMode.Text value:

```
<span style="font-family:'Cambria Math'">A=π</span><span style="font-family:'Cambria Math'">r</span><span style="font-family:'Cambria Math'">2</span>
```

## Support of Add and Remove Embedded Fonts.

We have implemented APIs to add embedded fonts in a document when it is saved. Similarly, embedded fonts can be removed from the document when it is saved. We have added EmbedTrueTypeFonts, EmbedSystemFonts, and SaveSubsetFonts properties in FontInfoCollection class.

```
/// <summary>
/// Specifies whether or not to embed TrueType fonts in a document when it is saved.
/// Default value for this property is <b>false</b>.
/// </summary>
/// <remarks>
/// <para>Embedding TrueType fonts allows others to view the document with the same
///  fonts that were used to create it, but may substantially increase the 
///  document size.</para>
/// <para>This option works for DOC, DOCX and RTF formats only.</para>
/// </remarks>
public bool EmbedTrueTypeFonts 
```
```
/// <summary>
/// <para>Specifies whether or not to embed System fonts into the document.
/// Default value for this property is <b>false</b>.</para>
/// <para>This option works only when <see cref="EmbedTrueTypeFonts"/> option is set to <b>true</b>.</para>
/// </summary>
/// <remarks>
/// <para>
/// Setting this property to <c>True</c> is useful if the user is on an East Asian system
/// and wants to create a document that is readable by others who do not have fonts for that
/// language on their system. For example, a user on a Japanese system could choose to embed the
/// fonts in a document so that the Japanese document would be readable on all systems.
/// </para>
/// <para>This option works for DOC, DOCX and RTF formats only.</para>
/// </remarks>
public bool EmbedSystemFonts 
```
```
/// <summary>
/// <para>Specifies whether or not to save a subset of the embedded TrueType fonts with the document.
/// Default value for this property is <b>false</b>.</para>
/// <para>This option works only when <see cref="EmbedTrueTypeFonts"/> property is set to <b>true</b>.</para>
/// </summary>
/// <remarks>
/// This option works for DOC, DOCX and RTF formats only.
/// </remarks>
public bool SaveSubsetFonts 
```

**Use Case 1** - Save document with embedded TrueType fonts. System fonts are not included. Saves full versions of embedding fonts.

```
Document doc = new Document("fileName");
FontInfoCollection fontInfos = doc.FontInfos;

fontInfos.EmbedTrueTypeFonts = true;
fontInfos.EmbedSystemFonts = false;
fontInfos.SaveSubsetFonts = false;
doc.Save("DocWithEmbeddedFonts"); 
```

**Use Case 2** - Save document with embedded TrueType fonts. System fonts are included. Saves full versions of embedding fonts.

```
Document doc = new Document("fileName");
FontInfoCollection fontInfos = doc.FontInfos;

fontInfos.EmbedTrueTypeFonts = true;
fontInfos.EmbedSystemFonts = true;
fontInfos.SaveSubsetFonts = false;
doc.Save("DocWithEmbeddedFonts"); 
```

**Use Case 3** - Save document with embedded TrueType fonts. System fonts are included. Saves subset of embedding fonts.

```
Document doc = new Document("fileName");
FontInfoCollection fontInfos = doc.FontInfos;

fontInfos.EmbedTrueTypeFonts = true;
fontInfos.EmbedSystemFonts = true;
fontInfos.SaveSubsetFonts = true;
doc.Save("DocWithEmbeddedFonts"); 
```

**Use Case 4** - Save document with embedded TrueType fonts. System fonts are not included. Saves subset of embedding fonts.

```
Document doc = new Document("fileName");
FontInfoCollection fontInfos = doc.FontInfos;

fontInfos.EmbedTrueTypeFonts = true;
fontInfos.EmbedSystemFonts = false;
fontInfos.SaveSubsetFonts = true;
doc.Save("DocWithEmbeddedFonts"); 
```

**Use Case 5** - Remove embedded fonts from the saved document.

```
Document doc = new Document("fileName");
FontInfoCollection fontInfos = doc.FontInfos;

fontInfos.EmbedTrueTypeFonts = false;
doc.Save("DocWithoutEmbeddedFonts"); 
```

### Improved Font Substitution Rules

We have improved font substitution rules in Aspose.Words 16.7.0. When specific font is not installed but is embedded into the document and a substitute for this font is assigned. In this case, Aspose.Words will use the fonts embedded in the document. Please check "Font Availability and Substitution".

## MsWordVersion Enum Moved to Aspose.Words.Settings.

MsWordVersion Enum has moved to Aspose.Words.Settings in Aspose.Wrods v16.7.0. This, however, should not be a breaking change as presently CompatibilityOptions.OptimizeFor is the only method that uses MsWordVersion enum and is already a member of Aspose.Words.Settings namespace.

## ReplaceAction, IReplacingCallback and ReplacingArgs Moved to Aspose.Words.Replacing.

ReplaceAction, IReplacingCallback and ReplacingArgs have moved to Aspose.Words.Replacing namespace in Aspose.Wrods v16.7.0.

## Added Advanced Range.Replace methods.

We have added following methods in Range class in Aspose.Words v16.7.0 to support advanced find/replace operations.

```
public int Replace(string pattern, string replacement, FindReplaceOptions options)
public int Replace(Regex pattern, string replacement, FindReplaceOptions options)
```

These methods support breaks in both search pattern and replacement string. Special meta-characters are used to specify breaks: &p for paragraph break, &b for section break, &m for page break and &l for manual line break. New FindReplaceOptions class was also introduced to hold all find/replace options. Most notable member of this class is ApplyFont/ApplyParagraphFormat. It allow to specify text/paragraph formatting to be applied to replacement text.

**Use Case 1**

Demonstrate how breaks support works. In this example we replace certain paragraph breaks with new paragraph breaks + some underline while make it centered. Additionally we replace custom text tag with section break.

```
Document doc = new Document();
DocumentBuilder builder = new DocumentBuilder(doc);

builder.Font.Name = "Arial";
builder.Writeln("First section");
builder.Writeln("  1st paragraph");
builder.Writeln("  2nd paragraph");
builder.Writeln("{insert-section}");
builder.Writeln("Second section");
builder.Writeln("  1st paragraph");

FindReplaceOptions options = new FindReplaceOptions();
options.ApplyParagraphFormat.Alignment = ParagraphAlignment.Center;

// Double each paragraph break after word "section", add kind of underline and make it centered.
int count = doc.Range.Replace("section&p", "section&p----------------------&p", options);

// Insert section break instead of custom text tag.
count = doc.Range.Replace("{insert-section}", "&b", options);
```

**Use Case 2**

Demonstrates usage of apply formatting and customer callback. In this example we replace numbers with their hexadecimal representations while make them highlighted with color.

```
Document doc = new Document();
DocumentBuilder builder = new DocumentBuilder(doc);

builder.Font.Name = "Arial";
builder.Write("There are few numbers that should be converted to HEX and highlighted: 123, 456, 789 and 17379.");

FindReplaceOptions options = new FindReplaceOptions();

// Highlight newly inserted content.
options.ApplyFont.HighlightColor = Color.DarkOrange;
options.ReplacingCallback = new NumberHexer();

int count = doc.Range.Replace(new Regex("[0-9]+"), "", options);

// Customer defined callback.
private class NumberHexer : IReplacingCallback
{
    public ReplaceAction Replacing(ReplacingArgs args)
    {
        // Parse numbers.
        int number = Convert.ToInt32(args.Match.Value);

        // And write it as HEX.
        args.Replacement = string.Format("0x{0:X}", number);

        return ReplaceAction.Replace;
    }
} 
```

**Deprecated methods:**

Old Replace methods are left for backward compatibility but marked as obsolete. We going to remove following methods in this year:

```
public int Replace(string oldValue, string newValue, bool isMatchCase, bool isMatchWholeWord)
public int Replace(Regex pattern, IReplacingCallback handler, bool isForward)
```

One old method

```
public int Replace(Regex pattern, string replacement)
```

continues to work with old code and will be switched to new code eventually.

## Added Overload of DigitalSignatureUtil.Sign to Specify a Password for Decrypting Document.

We have added following static methods for signing encrypted documents in Aspose.Words v16.7.0.

```
public static void Sign(string srcFileName, string dstFileName, CertificateHolder certHolder, string comments, DateTime signTime, string srcPassword);
public static void Sign(Stream srcStream, Stream dstStream, CertificateHolder certHolder, string comments, DateTime signTime, string srcPassword);
```

In the last parameter of these methods, specify a password for decrypting source document. Also, this is meaningful only if source document has DOCX format.

**Use Case 1 (working with file)**

```
// Create certificate holder from a file.
CertificateHolder cert = CertificateHolder.Create("certFileName", "certPassword");

// Digitally sign encrypted with "docPassword" document in the specified path.
DigitalSignatureUtil.Sign("srcDocFileName", "signedDocFileName", cert, "Comment", DateTime.Now, "docPassword");

// Open encrypted document from a file.
Document signedDoc = new Document("signedDocFileName", new LoadOptions("docPassword"));

// Check that encrypted document was successfully signed.
DigitalSignatureCollection signatures = doc.DigitalSignatures;
if (signatures.IsValid && (signatures.Count > 0))
  Console.WriteLine("The document was signed successfully.")
```

**Use Case 2 (working with stream)**

```
// Create certificate holder from a file.
CertificateHolder cert = CertificateHolder.Create("certFileName", "certPassword");

// Digitally sign encrypted with "docPassword" document in the specified stream.
DigitalSignatureUtil.Sign(srcDocStream, signedDocStream, cert, "Comment", DateTime.Now, "docPassword");

// Open encrypted document from a stream.
Document signedDoc = new Document("signedDocStream", new LoadOptions("docPassword"));

// Check that encrypted document was successfully signed.
DigitalSignatureCollection signatures = doc.DigitalSignatures;
if (signatures.IsValid && (signatures.Count > 0))
  Console.WriteLine("The document was signed successfully.")
```




[1]: https://downloads.aspose.com/words/net
[2]: https://downloads.aspose.com/words/java




