---
title: 'Extract Word Document Content Separated by Page Breaks using C#'
date: Mon, 16 Apr 2007 18:26:00 +0000
draft: false
url: /2007/04/16/extract-word-document-content-separated-by-page-breaks-using-csharp/
author: Miklovan
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

In [Aspose.Words][1], it is pretty easy to extract document content separated by section breaks, as this content is effectively put in separate **Section** nodes in Aspose.Words object model.

But what if we need to extract content separated by page breaks?

Here is a small and relatively simple code that can help you in solving this task:

**Example** **\[C#\]**

```
/// <summary>
/// Extracts pages from the specified document as a number of separate documents.
/// The pages must be separated with page breaks.
/// We assume that the initial document has only one section.
/// </summary>
private void ExtractPages()
{
      Document doc = new Document(MyPath + “PageSetup.PageBreaks.doc”);
      Node startNode = doc.FirstSection.Body.FirstParagraph;

      int pageNumber = 1;
      while (startNode != null)
      {
            Document page = ExtractPage(doc, ref startNode);
            page.Document.Save(string.Format(MyPath + “PageSetup.PageBreaks.Page{0} Out.doc”, pageNumber++));
      }
}
/// <summary>

/// Extracts the part of the document starting from specified node and ending with an end of the document or a page break.
/// Starting node reference is updated after extraction to point on the node next to page break,
/// If the extracted page is the last page of the document, then it is set to null.
/// </summary>

private Document ExtractPage(Document doc, ref Node startNode)
{
      // Only top-level paragraphs/tables can be used as a starting node of a page.

    if (startNode.ParentNode.NodeType != NodeType.Body)

            throw new System.ApplicationException(“Starting node must be a paragraph or a table in the main story of the document.”);
      Document page = new Document();
      Body pageBody = page.FirstSection.Body;
      pageBody.FirstChild.Remove();
      NodeImporter importer = new NodeImporter(doc, page, ImportFormatMode.KeepSourceFormatting);

      Node node;
      for (node = startNode; node != null; node = node.NextSibling)

      {
            page.FirstSection.Body.AppendChild(importer.ImportNode(node, true));
            if (node.NodeType == NodeType.Paragraph)

            {
                  Paragraph para = (Paragraph)node;

                  if (para.GetText().IndexOf(ControlChar.PageBreakChar) >=0)
                  {
                        node = node.NextSibling;
                        break;
                  }

            }

      }

      startNode = node;

      Node lastPageNode = pageBody.LastParagraph.LastChild; 

      if (lastPageNode != null)

            lastPageNode.Remove();

      return page;

}
```




[1]: https://products.aspose.com/words




