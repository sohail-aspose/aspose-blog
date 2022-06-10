---
title: 'Revealing the Killer New Feature in Aspose.Words 13.1.0 for the Start of 2013: Native Access to Page Layout Information'
date: Sat, 09 Feb 2013 13:30:46 +0000
draft: false
url: /2013/02/09/revealing-the-killer-new-feature-in-aspose.words-13.1.0-for-the-start-of-2013-native-access-to-page-layout-information/
author: Adam Skelton
summary: ''
tags: ['.net 1.1', 'Examples', 'Layout', 'extract pages', 'lines', 'net framework', 'page number of node', 'pages', 'rendered document', 'version', 'words']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose.words-logo2.jpg" alt="Aspose.Words Logo">}}


We wish you a warm welcome to 2013 from everyone here at the Aspose.Words team. We are pleased to announce the first release of Aspose.Words for .NET and Java for 2013. This release contains over a hundred improvements to Aspose.Words including several big additions and changes.

As always you can immediately download our latest Aspose.Words release from the following links:

*   [Aspose.Words for .NET 13.1.0][1]
*   [Aspose.Words for Java 13.1.0][2]

# Access to Page Layout Information

This month’s release provides access to the layout engine in the Aspose.Words API. This has been a long awaited feature and allows you to complete the following tasks that were hotly requested by more than a hundred of our users.

With this feature it is now possible to:

*   Find the page number where a particular node is located.
*   Find the X, Y location and size of a node as rendered on the page.
*   Split and extract individual pages from a document.
*   Enumerate the individual elements on a page, e.g pages, lines, spans.
*   Add a different image to each page of a document (without using the header or footer).

## Examples

The following C# examples provide a sneak peak of how to achieve the above tasks in this release of Aspose.Words. The full source code of these examples along with Visual Basic and Java versions are packaged in our offline example pack and is available from the downloads section:

*   [Aspose.Words for .NET Examples][3]
*   [Aspose.Words for Java Examples][4]

## Find the Page Number of a Node

The **PageNumbersOfNodes** sample demonstrates how to display the start and end page number of each node in the document body to the console:

```
Document doc = new Document(dataDir + "TestFile.docx");

// Create and attach collector before the document before page layout is built.
LayoutCollector layoutCollector = new LayoutCollector(doc);

// Print the details of each document node including the page numbers.
foreach (Node node in doc.FirstSection.Body.GetChildNodes(NodeType.Any, true))
{
    Console.WriteLine(" --------- ");
    Console.WriteLine("NodeType:   " + Node.NodeTypeToString(node.NodeType));
    Console.WriteLine("Text:       \"" + node.ToString(SaveFormat.Text).Trim() + "\"");
    Console.WriteLine("Page Start: " + layoutCollector.GetStartPageIndex(node));
    Console.WriteLine("Page End:   " + layoutCollector.GetEndPageIndex(node));
    Console.WriteLine(" --------- ");
    Console.WriteLine();
}
```



{{< figure align=center src="images/PageNumbersOfNodes.jpg" alt="The page numbers of each node in a document">}}


## Extract Individual Pages from a Document

The **PageSplitter** sample demonstrates how to extract the nodes belonging to an individual page or page range and return a new **Document** object from them. Using this feature you can work with the nodes on individual pages and save particular pages from a document back to flow formats such as DOCX or HTML – something which was not possible until now.

_Note: The **DocumentPageSplitter** is a class provided along with the sample and must be downloaded from the offline sample pack in order to use the code above._

```
Document doc = new Document(docName);

// Create and attach collector before the document before page layout is built.
LayoutCollector layoutCollector = new LayoutCollector(doc);

// This will build layout model and collect necessary information.
doc.UpdatePageLayout();

// Split nodes in the document into separate pages.
DocumentPageSplitter splitter = new DocumentPageSplitter(layoutCollector);

// Save each page to disk as separate documents.
for (int page = 1; page <= doc.PageCount; page++)
{
    Document pageDoc = splitter.GetDocumentOfPage(page);
    pageDoc.Save(Path.Combine(outFolder, string.Format("{0} -page{1} Out{2}", fileName, page, extensionName)));
}
```

**The input word documents and the output documents, each a page is saved from the original in separate output documents.**



{{< figure align=center src="images/PageSplitterInputAndOutput.jpg" alt="Word documents split into separate pages">}}


## Enumerate the Individual Elements on a Page

The **EnumerateLayoutElements** sample demonstrates how to use the **LayoutEnumerator** class which is now included in the Aspose.Words API. This class allows you to “walk” through the layout elements on each page of the document once it’s rendered in memory.

```
// Enumerates forward through each layout element in the document 
// and prints out details of each element.
private static void DisplayLayoutElements(LayoutEnumerator it, string padding)
{
    do
    {
        DisplayEntityInfo(it, padding);

        if (it.MoveFirstChild())
        {
            // Recurse into this child element.
            DisplayLayoutElements(it, padding + "    ");
            it.MoveParent();
        }
    } while (it.MoveNext());
}

private static void DisplayEntityInfo(LayoutEnumerator it, string padding)
{
    Console.Write(padding + it.Type + " - " + it.Kind);

    if (it.Type == LayoutEntityType.Span)
        Console.Write(" - " + it.Text);

    Console.WriteLine();
}
```



{{< figure align=center src="images/EnumerateLayoutEntities.jpg" alt="Lists details about the visual entities of a word document">}}


This sample also demonstrates this visually by rendering each page to a **Graphics** object and drawing outlines around each of the elements. Each layout entity type is drawn with a different colour line and the output is saved to disk in JPEG format.

**This is what the first page looks like in the input document:**



{{< figure align=center src="images/Input-Document.jpg" alt="Input Document">}}


**and this is the output with all layout entities outlined (click to zoom).**



{{< figure align=center src="images/TestFile-Page-1-Out.png" alt="Word document layout entities outlined">}}


## Find the Location and Size of a Node on a Page

The **DocumentLayoutHelper** sample provides a “wrapper” around the **LayoutEnumerator** class to allow easy access to layout elements through an object model in the same way nodes are accessed using the **Document** class.

It also provides backward access to find the line elements rendered on a page from a given **Paragraph** node.

```
// Creates a new RenderedDocument from the Aspose.Words Document object.
RenderedDocument layoutDoc = new RenderedDocument(doc);

// The following example demonstrates how to use the wrapper API.
// This snippet returns a class representing the third line of the first page and 
// contains properties that return the layout information of the element.
RenderedLine line = layoutDoc.Pages[0].Columns[0].Lines[2];

// This method provides a reverse lookup of lines for a given paragraph.
Console.WriteLine("The lines of the second paragraph:");

foreach (RenderedLine paragraphLine in layoutDoc.GetLinesOfParagraph(doc.FirstSection.Body.Paragraphs[1]))
{
    Console.WriteLine(string.Format("\"{0}\"", paragraphLine.Text.Trim()));
    Console.WriteLine(paragraphLine.Rectangle.ToString());
    Console.WriteLine();
}
```



{{< figure align=center src="images/LinesOfParagraph.jpg" alt="Lines of a word paragraph">}}


_Download the samples pack and check out the full code for further examples._

## Add an Image to Each Page of a Document without using Header or Footer

The **AddImageToEachPage** sample demonstrates how to add an image and a textbox containing different text to each page in the document:

```
LayoutCollector layoutCollector = new LayoutCollector(doc);

// Images in a document are added to paragraphs, so to add an image 
// to every page we need to find at any paragraph belonging to each page.
IEnumerator enumerator = doc.SelectNodes("//Body/Paragraph").GetEnumerator();

// Loop through each document page.
for (int page = 1; page <= doc.PageCount; page++)
{
    while (enumerator.MoveNext())
    {
        // Check if the current paragraph belongs to the target page.
        Paragraph paragraph = (Paragraph)enumerator.Current;
        if (layoutCollector.GetStartPageIndex(paragraph) == page)
        {
            AddImageToPage(paragraph, page); // Method provided in the full sample.
            break;
        }
    }
}

doc.Save(gDataDir + "TestFile Out.docx");
```



{{< figure align=center src="images/ImageTextboxAddedToPage.jpg" alt="An image added to every page of a Microsoft Word document">}}


# Aspose.Words has Switched to “Date-based” Version Numbering

The first version of Aspose.Words was released in late 2003 and since then everyone on the Aspose.Words team has been working hard, releasing new versions every month or so packed full with features and improvements. As a result we have a great product with many releases under our belt.

However we have noticed that from that versioning scheme it is hard to know what version belongs to what release date, which when dealing with subscriptions can make for some confusion. Therefore starting with this month’s release we are making it easier to track both Aspose.Words for .NET and Aspose.Words for Java versions by using the following scheme instead:

*   **<Year>.<Month>.<Hotfix>**

Because this month's release is for January 2013, this month's version of Aspose.Words is 13.1.0. Next month it will be 13.2.0 and so forth.

# Discontinued Support for .NET Framework 1.1

To make things better and easier for both our developers and the users of Aspose.Words, we have decided to dismiss support for the .NET Framework 1.1 from the Aspose.Words for .NET product. This means starting from this release we no longer ship the special DLLs targeting the .NET Framework 1.1 with Aspose.Words for .NET.

The NET Framework 1.1 is outdated and we expect very few users to develop applications that exclusively rely on this version of .NET. However we do hope this doesn’t provide any interruption to users. This was no easy decision, and hopefully one that is seen as a step forward and not backward. This is for several reasons:

*   There are features that we need to implement which are incompatible or difficult to get working with the 1.1 version of the .NET Framework. Without support for 1.1 we can more easily stream line new features into our component.
*   We can begin using features exclusively found in the .NET Framework 2.0 and above in the Aspose.Words code. This means useful features such as generics that we previously off limits to enable continued support of .NET 1.1 can now be used in our code. The benefits of this get passed onto you as these features will improve performance in the Aspose.Words component even further. Expect to see these improvements in the next few versions of Aspose.Words.
*   Since Aspose.Words for .NET is auto-ported to Java many performance benefits will extend to Aspose.Words for Java as well.

As always we value our customer feedback, if you have anything to ask us let us know on our [dedicated forum][5].




[1]: https://downloads.aspose.com/words/net
[2]: https://downloads.aspose.com/words/java
[3]: https://github.com/aspose-words/Aspose.Words-for-.NET
[4]: https://github.com/aspose-words/Aspose.Words-for-Java
[5]: https://forum.aspose.com/c/words




