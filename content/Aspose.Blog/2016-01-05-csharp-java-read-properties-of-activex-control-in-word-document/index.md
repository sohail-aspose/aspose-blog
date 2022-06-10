---
title: 'Read Properties of ActiveX Control in Java using Aspose.Words 15.12.0'
date: Tue, 05 Jan 2016 12:52:55 +0000
draft: false
url: /2016/01/05/csharp-java-read-properties-of-activex-control-in-word-document/
author: Tahir Manzoor
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Aspose.Words 15.12.0 has been released. This month’s release contains over 89 useful new features, enhancements and bug fixes to the Aspose.Words products. You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 15.12.0][1]
*   [Aspose.Words for Java 15.12.0][2]

Here is a look at just a few of the biggest features and API changes in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the links above.

*   Support of Read-only access to ActiveX Control properties
*   Support of Default page margins, header, and footer distance, column spacing depends on current culture
*   Introduced Overloaded method InsertOleObject in DocumentBuilder class
*   Introduced SuggestedFileName Property in OleFormat class
*   Introduced TrimWhitespaces Property in MailMerge class
*   Avoid Populating Merge Fields Inside the false Part of IF Field
*   Support of Ruby Tags in HTML Import
*   Support of Applying styles from the template during HTML insertion

## Support of Read-only Access to ActiveX Control Properties

[OleControl][3] is a new public class and represents ActiveX control. OleControl class is base class for all ActiveX objects. You can check whether the control is a Forms 2.0 OLE control by OleControl.IsForms2OleControl property. Type of Forms2OleControl is exposed in Forms2OleControlType.Type property. OleControl.IsForms2OleControl property will return true when the control type is Forms 2.0 OLE control.

Forms2OleControl has few properties exposed for reading:

```
public string Caption
public string Value
public bool Enabled
public Forms2OleControlCollection ChildNodes
public Forms2OleControlType Type
```
```
Document doc = new Document(filename);
Shape shape = (Shape)doc.GetChild(NodeType.Shape, 0, true);
OleControl oleControl = shape.OleFormat.OleControl;

if (oleControl.IsForms2OleControl)
{
  Forms2OleControl checkBox = (Forms2OleControl)oleControl;
  Console.WriteLine("Caption: " + checkBox.Caption);
  Console.WriteLine("Value: " + checkBox.Value);
  Console.WriteLine("Enabled: " + checkBox.Enabled);
  Console.WriteLine("Type: " + checkBox.Type);
  Console.WriteLine("ChildNodes: " + checkBox.ChildNodes);
}
```

## Support of Default Page Margins

Now default page margins, header/footer distance and column spacing depend on current culture to mimic MS Word behavior.

For example, now all page margins are 1 for English (United States) and English (United Kingdom). Left, right, top margins are 2.5 cm; bottom margin is 2 cm for German. The new defaults are used for a new document and for a loaded document if an explicit value is not set for the mention parameters.

The following code can be used to restore the previous behavior.

```
Document doc = new Document();
Section section = doc.Sections[0];

section.PageSetup.LeftMargin = 90;            // 3.17 cm
section.PageSetup.RightMargin = 90;           // 3.17 cm
section.PageSetup.TopMargin = 72;             // 2.54 cm
section.PageSetup.BottomMargin = 72;          // 2.54 cm
section.PageSetup.HeaderDistance = 35.4;      // 1.25 cm
section.PageSetup.FooterDistance = 35.4;      // 1.25 cm
section.PageSetup.TextColumns.Spacing = 35.4; // 1.25 cm
```

It is possible to change culture for current thread that will cause changing default page margins, header/footer distance and column spacing.

```
Thread.CurrentThread.CurrentCulture = new CultureInfo("de-de");
Document doc = new Document();

Section section = doc.Sections[0];
Debug.Assert(section.PageSetup.LeftMargin == 70.85);         // 2.5 cm
Debug.Assert(section.PageSetup.RightMargin == 70.85);        // 2.5 cm
Debug.Assert(section.PageSetup.TopMargin == 70.85);          // 2.5 cm
Debug.Assert(section.PageSetup.BottomMargin == 56.7);        // 2 cm
Debug.Assert(section.PageSetup.HeaderDistance == 35.4);      // 1.25 cm
Debug.Assert(section.PageSetup.FooterDistance == 35.4);      // 1.25 cm
Debug.Assert(section.PageSetup.TextColumns.Spacing == 35.4); // 1.25 cm
```

## Overloaded method InsertOleObject in DocumentBuilder class

The previous implementation of InsertOleObject expects full file name to linked object and chooses ProgId and ClsId depending on the file extension. Passing the internet URL reveals a new use case. We can't extract file type from URL directly, URL can refer to the page in a very different way. It can be www.aspose.com, www.aspose.com\\index.aspx?id=1 and so on. So Aspose.Words decided to make new method which allows customer to pass ProgId explicitly.

```
/// <summary>
/// Inserts an embedded or linked OLE object from a file into the document. 
/// Detects OLE object type using given progID parameter. 
/// </summary>
/// <param name="fileName">Full path to the file.</param>
/// <param name="progId">ProgId of OLE object.</param>
/// <param name="isLinked">If true then linked OLE object is inserted otherwise 
/// embedded OLE object is inserted.</param>
/// <param name="asIcon">Specifies either Iconic or Normal mode of OLE object
/// being inserted.</param>
/// <param name="presentation">Image presentation of OLE object. 
/// If value is null Aspose.Words will use one of the predefined images.</param>
/// <returns>The form field node that was just inserted.</returns>
public Shape InsertOleObject(string fileName, string progId, bool isLinked, 
bool asIcon, System.Drawing.Image presentation)
```
```
Document doc = new Document();
DocumentBuilder builder = new DocumentBuilder(doc);
builder.InsertOleObject("http://www.aspose.com", "htmlfile", true, true, null);
```

## Introduced SuggestedFileName Property in OleFormat class

Microsoft Word is smart enough to extract the file name of the embedded OLE object if it is an OutlookAttach OLE object. So Aspose.Words mimics the same behavior. If the file name can not be extracted, an empty string is returned.

```
Shape oleShape = doc.FirstSection.Body.GetChild(NodeType.Shape, 0, true);
Console.WriteLinel(oleShape.OleFormat.SuggestedFileName);
```

## Introduced TrimWhitespaces Property in MailMerge class

We have added an option that allows trimming trailing and leading whitespaces mail merge values.

```
Document.MailMerge.TrimWhitespaces = false;
```

## Avoid Populating Merge Fields Inside the false Part of IF Field

Originally, this issue was about introducing the option to control whether to populate the merge field inside a false part of IF field or not. However, we eventually decided that the suggested option was too specific. Thus we decided to simply make Aspose.Words avoid populating merge fields inside the false part of the field. The cleanup options are not applied too. So, the false part of the IF field remains unchanged, like in MS Word mail merge preview.

## Support of Applying styles from the template during HTML insertion

'class' attribute can be used to apply a specific MS Word style to an inserted HTML element.

 class='MyWordStyle'>This para should have MyWordStyle style.  

```
Document doc = new Document(MyDir + "in.docx");
               
DocumentBuilder builder = new DocumentBuilder(doc);
builder.MoveToDocumentEnd();
builder.InsertHtml(" class='MyWordStyle'>This para should have MyWordStyle style.");
 
doc.Save(MyDir + "Out.docx");
```




[1]: https://downloads.aspose.com/words/net
[2]: https://downloads.aspose.com/words/java
[3]: https://apireference.aspose.com/words/net/aspose.words.drawing.ole/olecontrol




