---
title: 'How to Create Quality Code Examples for C# and VB.NET'
date: Wed, 27 Sep 2006 11:51:00 +0000
draft: false
url: /2006/09/27/57590/
author: Romank
summary: ''
tags: ['Roman Korchagin']
---

Have a look, most of the public API members of our new Aspose.Editor component have  code examples [http://www.aspose.com/Products/Aspose.Editor/Api/Index.html][1]. You decide whether they are good or not, but we think they are great and hope you like them.

We went through a lot of hurdles trying to find a suitable solution and I thought you might find it useful to know how we produce code examples now.

In my earlier post Authoring API Help for .NET Projects I complained that we cannot find a suitable tool for building API reference the way we want it, including a robust system for building code examples.

To recap quickly:

1.  We want the API documentation to be in XML comments in C#.
2.  We do not want code examples to be embedded in XML comments because they make both the production code and code of examples impossible to read and maintain.
3.  We did not find any commercial tools that helped to work with code examples in a decent way. One of the tools I tried allowed to include a range of lines from an external file as an example, but you had to specify line numbers explicitly. What a briliant feature :) What if the external file changes? The example will include a different set of code lines then and nobody will notice until much later.

Therefore we built our own technology and a tool to maintain code examples and inject them into the API documentation.

The new technology can be summarized as:

1.  Create C# project with code examples. Write examples as unit tests (you will be able to exclude actual unit testing code from the published code example if you want).
2.  Use special comments inside the code example to indicate where the example starts, ends, brief description, public members the example applies to, individual lines to skip and so on.
3.  Convert the C# project with examples to VB.NET using this excellent tool [http://www.tangiblesoftwaresolutions.com/][2]
4.  Compile and run both C# and VB.NET example projects unit test to make sure all examples actually work.
5.  Use our Aspose.ExampleCutter tool that takes two directories (C# and VB.NET source code), a reference to the assembly your are documenting and the XML comments file without examples. The output of the tool is an XML file with examples injected in the right places. The tool also produces a log file which lists all public members that still do not have examples or members that have example in one language only and so on.
6.  Use NDoc or some other tool to compile the documentation into CHM and HTML and you are done.

We use Aspose.ExampleCutter at Aspose internally only. Although if there is a public interest, I think we might be able to release it as a free (or commercial) utility. Please let us know if you are interested.

Here is some code that shows the syntax we use to identify what goes into an example:

```
[Test]
  public void OpenSaveFile()
  {
   //ExStart
   //ExFor:Document
   //ExFor:Document.#ctor(string)
   //ExFor:Document.Save(String)
   //ExFor:Document.IsModified
   //ExFor:Range.Italic
   //ExSummary:Opens, modifies and saves a WordprocessingML document into a file.
   Document doc = new Document(MyPath + “Welcome.xml”);

   // Just test the modified property.
   Assert.AreEqual(false, doc.IsModified);

   // Let’s make all text in the document italic for fun.
   doc.GetRange().Italic = true;

   Assert.AreEqual(true, doc.IsModified);

   doc.Save(MyPath + “ExDocument.OpenSaveFile Out.xml”);
   //ExEnd
  }

—–

  [Test]
  public void BoldItalic()
  {
   editorControl = new Aspose.Editor.EditorControl();
   editorControl.Open(MyPath + “Welcome.xml”);
   FormatBold();
   FormatItalic();
  }

  //ExStart
  //ExFor:Selection.Bold
  //ExFor:Selection.Italic
  //ExSummary:Shows how to use bold and italic properties of the current selection.

  /// <summary>
  /// This method should be called when the user clicks the Bold toolbar button to toggle
  /// current selection bold status.
  /// </summary>
  private void FormatBold()
  {
   Debug.Assert(editorControl.Document != null);

   // This is a bit of roughness, should improve in future versions.
   // To find out whether current place is bold it seems best to use Selection.Range.Bold,
   // but to set bold in the current place (which could be an empty selection, just a cursor),
   // it is best to use Selection.IsBold.
   editorControl.Selection.Bold = !editorControl.Selection.Range.Bold;
  }

  /// <summary>
  /// This method should be called when the user clicks the Italic toolbar button to toggle current
  /// current selection italic status.
  /// </summary>
  private void FormatItalic()
  {
   Debug.Assert(editorControl.Document != null);
   editorControl.Selection.Italic = !editorControl.Selection.Range.Italic;
  }
  //ExEnd

—–
```

As you can see from the above code, a single example can apply to several members of the API. It is also possible for multiple examples to be included for a single member in the API. The //ExStart and //ExEnd tags can be anywhere in your code so you can include "jagged" fragments of the code, for example, 1.5 method, etc.




[1]: /Products/Aspose.Editor/Api/Index.html
[2]: http://www.tangiblesoftwaresolutions.com/



