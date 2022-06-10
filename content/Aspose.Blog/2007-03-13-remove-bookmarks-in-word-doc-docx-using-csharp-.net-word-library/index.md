---
title: 'Remove Bookmarks in Word Document using C#'
date: Tue, 13 Mar 2007 09:11:00 +0000
draft: false
url: /2007/03/13/remove-bookmarks-in-word-doc-docx-using-csharp-.net-word-library/
author: Miklovan
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

What to do if you need to remove bookmark and its entire content from the document altogether. The only method existing in API for that is setting **Bookmark.Text** to an empty string. But that will work only for the simplest of bookmarks. For bookmark spanning multiple nodes with mixed content, like paragraph, tables, it will fail with a dreaded **"Start and end node should have the same grand parent"** exception. It will also fail when bookmark spans several sections and bookmark content is crossing the section border.  

Taking into account this and the fact that lots of users are requesting the robust bookmark removal capability we have decided to provide a sample code to achieve this functionality. We have already tested this code on several 'problem' documents and it works fine as far as I can see. However, it is up to you to try it for yourself and find out if it works for your documents. Please report all encountered problems in the forum. We will try to fix them as soon as they will be reported. Then, after some time and community testing we are going to include this method into Aspose.Words API.

## C# Code to Remove Bookmarks in Word Document```
private void RemoveBookmarkWithContent(Bookmark bookmark)
{
        // We need to store other bookmark nodes here, to move them away from the removed area.
        Hashtable bookmarkNames = new Hashtable();
        Hashtable bookmarkStarts = new Hashtable();
        Hashtable bookmarkEnds = new Hashtable();

        ArrayList nodesToRemove = new ArrayList();
        
        BookmarkStart bookmarkStart = bookmark.BookmarkStart;
        BookmarkEnd bookmarkEnd = bookmark.BookmarkEnd;
        Document doc = bookmarkStart.Document;
        Paragraph lastParagraph = doc.LastSection.Body.LastParagraph;

        Node node = SeekFirstNodeOfBookmarkRange(bookmarkStart);

        Paragraph endPara = FindParagraphNextAfterBookmark(bookmarkEnd);

        // Iterate over all nodes that contain or are between bookmark start and end nodes.
        while(node != bookmarkEnd)
        {
                node = node.NextPreOrder(doc);

                // BookmarkStart/BookmarkEnd are saved to be handled separately later.
                // All other nodes are collected as candidates for removal.
                if (!StoreIfBookmark(bookmarkNames, bookmarkStarts, bookmarkEnds, node))
                        nodesToRemove.Add(node);
        }

        foreach (string name in bookmarkNames.Keys)
        {
                if ((bookmarkStarts.ContainsKey(name)) && (bookmarkEnds.ContainsKey(name)))
                {
                        // If bookmark is nested, remove it altogether.
                        RemoveBookmarkNode(name, bookmarkStarts);
                        RemoveBookmarkNode(name, bookmarkEnds);
                }
                else
                {
                        // If bookmark is overlapping, move the contained start/end node to the next paragraph after removed range.
                        if (bookmarkStarts.ContainsKey(name))
                                MoveBookmarkNode(name, bookmarkStarts, endPara);
                        else
                                MoveBookmarkNode(name, bookmarkEnds, endPara);
                }
        }

        bool hasNodesToRemove = true;
        
        while(hasNodesToRemove)
        {
                hasNodesToRemove = false;

                for (int i = 0; i < nodesToRemove.Count; i++)
                {
                        Node nodeToRemove = (Node)nodesToRemove\[i\];

                        // Skip already removed nodes.
                        if (nodeToRemove.ParentNode == null)
                                continue;

                        // Skip nodes that have child nodes.
                        if (nodeToRemove.IsComposite && (nodeToRemove as CompositeNode).HasChildNodes)
                                continue;

                        // Do not remove node if it is the last paragraph in the document.
                        if (nodeToRemove == lastParagraph)
                                continue;

                        // Remove node.
                        nodeToRemove.Remove();

                        // If at least one node was removed in loop, then the loop will be repeated.
                        hasNodesToRemove = true;
                }
        }
}

private Node SeekFirstNodeOfBookmarkRange(BookmarkStart bookmarkStart)
{
        Node node = bookmarkStart;

        Document doc = node.Document;

        // Bookmark nodes located immediately before start of our bookmark should also be included in the removal process.
        do
        {
                node = node.PreviousPreOrder(doc);
        }
        while(IsBookmarkNode(node));

        // Look back from the bookmark start node to include containing nodes into removal process.
        while(node.IsComposite)
        {
                Node prevNode = node.PreviousPreOrder(doc);

                if (prevNode == null)
                        break;
                else
                        node = prevNode;
        }

        return node;
}

private Paragraph FindParagraphNextAfterBookmark(BookmarkEnd bookmarkEnd)
{
        // Find the paragraph that is next to removed bookmark range.
        // It will be used to move all bookmark start/end nodes belonging to bookmarks overlapping our bookmark,
        // so that they will be preserved after this bookmark removal.
        Paragraph para;

        Node node = bookmarkEnd;
        Document doc = node.Document;

        // It can be that the paragraph containing bookmark end node if the last paragraph in the bookmark range 
        // contains other nodes beside BookmarkEnd or is the last unremovable paragraph in the document.
        if (node.NextSibling != null || node.ParentNode == doc.LastSection.Body.LastParagraph)
        {
                para = (Paragraph)bookmarkEnd.ParentNode;
        }
                // Or it can be the paragraph next to it.
        else
        {
                while(node.NodeType != NodeType.Paragraph)
                {
                        node = node.NextPreOrder(doc);
                }

                para = (Paragraph)node;
        }

        return para;
}

private bool IsBookmarkNode(Node node)
{
        return (node.NodeType == NodeType.BookmarkStart) || (node.NodeType == NodeType.BookmarkEnd);
}

private bool StoreIfBookmark(Hashtable bookmarkNames, Hashtable bookmarkStarts, Hashtable bookmarkEnds, Node node)
{
        if (node.NodeType == NodeType.BookmarkStart)
        {
                BookmarkStart bookmarkStart = (BookmarkStart)node;
                bookmarkNames\[bookmarkStart.Name\] = null;
                bookmarkStarts.Add(bookmarkStart.Name, bookmarkStart);
                return true;
        }
        else if (node.NodeType == NodeType.BookmarkEnd)
        {
                BookmarkEnd bookmarkEnd = (BookmarkEnd)node;
                bookmarkNames\[bookmarkEnd.Name\] = null;
                bookmarkEnds.Add(bookmarkEnd.Name, bookmarkEnd);
                return true;
        }

        return false;
}

private Node RemoveBookmarkNode(string name, Hashtable bookmarkNodes)
{
        Node node = (Node)bookmarkNodes\[name\];
        node.Remove();
        bookmarkNodes.Remove(name);
        return node;
}

private void MoveBookmarkNode(string name, Hashtable bookmarkNodes, Paragraph para)
{
        para.PrependChild(RemoveBookmarkNode(name, bookmarkNodes));
}
\[VB .NET\] 

Private Sub RemoveBookmarkWithContent(ByVal bookmark As Bookmark)
        ‘ We need to store other bookmark nodes here, to move them away from the removed area.
        Dim bookmarkNames As Hashtable = New Hashtable
        Dim bookmarkStarts As Hashtable = New Hashtable
        Dim bookmarkEnds As Hashtable = New Hashtable

        Dim nodesToRemove As ArrayList = New ArrayList

        Dim bookmarkStart As BookmarkStart = bookmark.BookmarkStart
        Dim bookmarkEnd As BookmarkEnd = bookmark.BookmarkEnd
        Dim node As Node = bookmarkStart
        Dim doc As Document = node.Document
        Dim lastParagraph As Paragraph = doc.LastSection.Body.LastParagraph

        ‘ Bookmark nodes located immediately before start of our bookmark should also be included in the removal process.
        Do
                node = node.PreviousPreOrder(doc)
        Loop While IsBookmarkNode(node)

        ‘ Look back from the bookmark start node to include containing nodes into removal process.
        Do While node.IsComposite
                Dim prevNode As Node = node.PreviousPreOrder(doc)

                If prevNode Is Nothing Then
                        Exit Do
                Else
                        node = prevNode
                End If
        Loop

        ‘ Find the paragraph that is next to removed bookmark range.
        ‘ It will be used to move all bookmark start/end nodes belonging to bookmarks overlapping our bookmark,
        ‘ so that they will be preserved after this bookmark removal.
        Dim endPara As Paragraph

        ‘ It can be the paragraph containing bookmark end node if the last paragraph in the bookmark range 
        ‘ contains other nodes beside BookmarkEnd or is the last unremovable paragraph in the document.
        If Not bookmarkEnd.NextSibling Is Nothing OrElse bookmarkEnd.ParentNode Is lastParagraph Then
                endPara = CType(bookmarkEnd.ParentNode, Paragraph)
                ‘ Or it can be the paragraph next to it.
        Else
                Do While node.NodeType <> NodeType.Paragraph
                        node = node.NextPreOrder(doc)
                Loop

                endPara = CType(node, Paragraph)
        End If

        ‘ Iterate over all nodes that contain or are between bookmark start and end nodes.
        Do While Not node Is bookmarkEnd
                node = node.NextPreOrder(doc)

                ‘ BookmarkStart/BookmarkEnd are saved to be handled separately later.
                ‘ All other nodes are collected as candidates for removal.
                If (Not StoreIfBookmark(bookmarkNames, bookmarkStarts, bookmarkEnds, node)) Then
                        nodesToRemove.Add(node)
                End If
        Loop

        For Each name As String In bookmarkNames.Keys
                If (bookmarkStarts.ContainsKey(name)) AndAlso (bookmarkEnds.ContainsKey(name)) Then
                        ‘ If bookmark is nested, remove it altogether.
                        RemoveBookmarkNode(name, bookmarkStarts)
                        RemoveBookmarkNode(name, bookmarkEnds)
                Else
                        ‘ If bookmark is overlapping, move the contained start/end node to the next paragraph after removed range.
                        If bookmarkStarts.ContainsKey(name) Then
                                MoveBookmarkNode(name, bookmarkStarts, endPara)
                        Else
                                MoveBookmarkNode(name, bookmarkEnds, endPara)
                        End If
                End If
        Next name

        Dim hasNodesToRemove As Boolean = True

        Do While hasNodesToRemove

                hasNodesToRemove = False

                Dim i As Integer = 0

                Do While i < nodesToRemove.Count
                        Dim nodeToRemove As Node = CType(nodesToRemove(i), Node)
                        ‘ Skip already removed nodes.
                        ‘ Skip nodes that have child nodes.
                        ‘ Do not remove node if it is the last paragraph in the document.
                        If Not (nodeToRemove.ParentNode Is Nothing) And \_
                                Not (nodeToRemove.IsComposite AndAlso CType(nodeToRemove, CompositeNode).HasChildNodes) And \_
                                Not (nodeToRemove Is lastParagraph) Then
                                ‘ Remove node.
                                nodeToRemove.Remove()
                                ‘ If at least one node was removed in loop, then the loop will be repeated.
                                hasNodesToRemove = True
                        End If
                        i += 1
                Loop
        Loop
End Sub

Private Function IsBookmarkNode(ByVal node As Node) As Boolean
        Return (node.NodeType = NodeType.BookmarkStart) OrElse (node.NodeType = NodeType.BookmarkEnd)
End Function

Private Function StoreIfBookmark(ByVal bookmarkNames As Hashtable, ByVal bookmarkStarts As Hashtable, ByVal bookmarkEnds As Hashtable, ByVal node As Node) As Boolean
        If node.NodeType = NodeType.BookmarkStart Then
                Dim bookmarkStart As BookmarkStart = CType(node, BookmarkStart)
                bookmarkNames(bookmarkStart.Name) = Nothing
                bookmarkStarts.Add(bookmarkStart.Name, bookmarkStart)
                Return True
        ElseIf node.NodeType = NodeType.BookmarkEnd Then
                Dim bookmarkEnd As BookmarkEnd = CType(node, BookmarkEnd)
                bookmarkNames(bookmarkEnd.Name) = Nothing
                bookmarkEnds.Add(bookmarkEnd.Name, bookmarkEnd)
                Return True
        End If

        Return False
End Function

Private Function RemoveBookmarkNode(ByVal name As String, ByVal bookmarkNodes As Hashtable) As Node
        Dim node As Node = CType(bookmarkNodes(name), Node)
        node.Remove()
        bookmarkNodes.Remove(name)
        Return node
End Function

Private Sub MoveBookmarkNode(ByVal name As String, ByVal bookmarkNodes As Hashtable, ByVal para As Paragraph)
        para.PrependChild(RemoveBookmarkNode(name, bookmarkNodes))
End Sub
```

Private Sub MoveBookmarkNode(ByVal name As String, ByVal bookmarkNodes As Hashtable, ByVal para As Paragraph)  
para.PrependChild(RemoveBookmarkNode(name, bookmarkNodes))  
End Sub








