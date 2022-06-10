---
title: 'Workaround for form field text loose formatting when updated from code.'
date: Tue, 13 Mar 2007 09:04:00 +0000
draft: false
url: /2007/03/13/70190/
author: Miklovan
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

There is a known issue of loss of formatting when setting form field text input value using **Result** property or **SetTextInputValue** method. For example, you have formatted your text form field as bold and it comes up as normal text when updated. For a workaround you can use the following wrapper method instead of using **SetTextInputValue** method directly:

**Example**

```
\[C#\]

private void SetFormFieldText(FormField formField, object value)
{
        if ((value == null) || (value is string) && ((string)value == ""))
        {
                formField.Result = "";
                return;
        }

        Node node = formField.PreviousSibling;
        Node separator = null;
        Run resultRun = null;

        while (node != null && node.NodeType != NodeType.FieldSeparator)
        {
                // Take a run with formatting from form field code.
                if (node is Run)
                        resultRun = (Run)node.Clone(true);

                node = node.NextSibling;
        }

        separator = node;

        while (node != null && node.NodeType != NodeType.FieldEnd)
        {
                // If form field value contains run then it is better to take it from here.
                if (node is Run)
                        resultRun = (Run)node.Clone(true);

                node = node.NextSibling;
        }

        formField.SetTextInputValue(value);

        if (separator != null && resultRun != null)
        {
                resultRun.Text = separator.NextSibling.GetText();
                separator.ParentNode.InsertAfter(resultRun, separator);
                resultRun.NextSibling.Remove();
        }
}

```
```
\[VB .NET\]

Private Sub SetFormFieldText(ByVal formField As FormField, ByVal value As Object)
        If (value Is Nothing) OrElse (TypeOf value Is String) AndAlso (CStr(value) = "") Then
                formField.Result = ""
                Return
        End If

        Dim node As Node = formField.PreviousSibling
        Dim separator As Node = Nothing
        Dim resultRun As Run = Nothing

        Do While Not node Is Nothing AndAlso node.NodeType <> NodeType.FieldSeparator
                ' Take a run with formatting from form field code.
                If TypeOf node Is Run Then
                        resultRun = CType(node.Clone(True), Run)
                End If

                node = node.NextSibling
        Loop

        separator = node

        Do While Not node Is Nothing AndAlso node.NodeType <> NodeType.FieldEnd
                ' If form field value contains run then it is better to take it from here.
                If TypeOf node Is Run Then
                        resultRun = CType(node.Clone(True), Run)
                End If

                node = node.NextSibling
        Loop

        formField.SetTextInputValue(value)

        If Not separator Is Nothing AndAlso Not resultRun Is Nothing Then
                resultRun.Text = separator.NextSibling.GetText()
                separator.ParentNode.InsertAfter(resultRun, separator)
                resultRun.NextSibling.Remove()
        End If
End Sub

```








