---
title: 'Tutorial on Aspose.Network latest Outlook dragdrop feature'
date: Tue, 20 Mar 2007 08:31:00 +0000
draft: false
url: /2007/03/20/70798/
author: Iret
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

**Outlook dragdrop** feature is included in the latest **Aspose.Network** release, which enables  
developers to easily create UI elements that respond to Outlook drag drop events.

The following sample shows how to create a panel, on which user can drag a message from  
Outlook and drop it, and the program save that message(s) to .msg file(s).

**Step 1.** Create a windows form application

**Step 2.** Add reference to Aspose.Network

Browse for Aspose.Network.dll and Aspose.Windows.Forms.dll, and click ok

**Step 3.** Create your ui elements, in this sample, we create a panel in this sample. Right click  
your project in the solution panel and choose "Add > new item", create a class called  
MyPanel:

Let MyPanel be a subclass of System.Windows.Form.Panel, and add a  
Aspose.Windows.Forms.FileDropTargetManager property to MyPanel:

\[C#\]

using System;  
using System.Collections.Generic;  
using System.Text;

namespace WindowsApplication1  
{  
    public class MyPanel:System.Windows.Forms.Panel  
    {

        private Aspose.Windows.Forms.FileDropTargetManager m;  
    }  
}

\[VB.NET\]

Public Class MyPanel  
    Inherits System.Windows.Forms.Panel

    Private m As Aspose.Windows.Forms.FileDropTargetManager

End Class

**Step 4.** Override OnHandleCreated and OnHandleDestroyed methods to register MyPanel  
using Aspose.WindowsForms.FileDropTargetManager:

\[C#\]

    public class MyPanel:System.Windows.Forms.Panel  
    {  
        //hook up  
        protected override void OnHandleCreated(EventArgs e)  
        {  
            this.AllowDrop = true;  
            this.m = new Aspose.Windows.Forms.FileDropTargetManager(this);  
            this.m.EnsureRegistered(this);  
            base.OnHandleCreated(e);  
        }  
        //unhook  
        protected override void OnHandleDestroyed(EventArgs e)  
        {  
            this.m.EnsureUnRegistered(this);  
            base.OnHandleDestroyed(e);  
        }

        private Aspose.Windows.Forms.FileDropTargetManager m;  
    }

\[VB.NET\]

Public Class MyPanel  
    Inherits System.Windows.Forms.Panel

    'hook up  
    Protected Overrides Sub OnHandleCreated(ByVal e As System.EventArgs)  
        Me.AllowDrop = True  
        m = New Aspose.Windows.Forms.FileDropTargetManager(Me)  
        m.EnsureRegistered(Me)  
        MyBase.OnHandleCreated(e)  
    End Sub

    'un hook  
    Protected Overrides Sub OnHandleDestroyed(ByVal e As System.EventArgs)  
        m.EnsureUnRegistered(Me)  
        MyBase.OnHandleDestroyed(e)  
    End Sub

    Private m As Aspose.Windows.Forms.FileDropTargetManager

End Class

**Step 5.** Build the project. MyPanel is ready to use now. This panel will be able to accepts  
drag and drop events from Outlook. Open your toolbox panel and drag MyPanel onto your  
windows form:

**Step 6.** Add an event handler to MyPanel's DragDrop event (don't forget to set AllowDrop  
property to true from the properties panel and change MyPanel's BackColor to your favourite  
):

**Step 7:** Implement the DragDrop event handler. we simply save those messages dragged from  
outlook to files as .msg. First we cast DragEventArgs to  
Aspose.Windows.Forms.FileDragEventArgs, which contains an array "Files" property  
standing for user's drag target. If user drag several messages from outlook and drop it onto  
MyPanel, Files.Count will be the number of  messges, and Files\[ i \] ( or VB Files(i) ) stands  
for each message.

\[C#\]

        private void myPanel1\_DragDrop(object sender, DragEventArgs e)  
        {  
            Aspose.Windows.Forms.FileDragEventArgs args;  
            args = (Aspose.Windows.Forms.FileDragEventArgs)e;  
            if (args != null && args.Files.Count > 0)  
            {  
                for (int i = 0; i < args.Files.Count; i++)  
                {  
                    SaveFileDialog dialog = new SaveFileDialog();  
                    dialog.FileName = args.Files\[ i \].FileName;  
                    if (dialog.ShowDialog() == DialogResult.OK)  
                    {  
                        try  
                        {  
                            System.IO.FileStream output;  
                            output = new System.IO.FileStream(dialog.FileName,  
System.IO.FileMode.CreateNew);  
                            args.Files\[ i \].Save(output);  
                            MessageBox.Show("Save success:" + dialog.FileName);  
                        }  
                        catch (Exception ex)  
                        {  
                            MessageBox.Show("Save failed:" + ex.ToString());  
                        }  
                    }  
                }  
            }  
        }

\[VB.NET\]

    Private Sub MyPanel1\_DragDrop(ByVal sender As System.Object, ByVal e As  
System.Windows.Forms.DragEventArgs) Handles MyPanel1.DragDrop  
        Dim args As Aspose.Windows.Forms.FileDragEventArgs  
        args = TryCast(e, Aspose.Windows.Forms.FileDragEventArgs)  
        If (args IsNot Nothing) Then  
            If ((args.Files IsNot Nothing) AndAlso (args.Files.Count > 0)) Then  
                For i As Integer = 0 To args.Files.Count - 1  
                    Dim saveDialog As New SaveFileDialog  
                    saveDialog.FileName = args.Files(i).FileName  
                    saveDialog.ShowDialog(Me)  
                    Try  
                        Dim fs As System.IO.FileStream = New  
System.IO.FileStream(saveDialog.FileName, System.IO.FileMode.CreateNew)  
                        args.Files(i).Save(fs)  
                        fs.Close()  
                        MessageBox.Show("Save Success." & args.Files(i).FileName)  
                    Catch ex As Exception  
                        MessageBox.Show("Save Failed:" & ex.Message)  
                    End Try  
                Next  
            End If  
        End If  
    End Sub

**Step 8.** Run the project and test it! Now you will be able to drag messages from outlook and  
drop it to your application. the application will prompt you to save those messages to .msg  
files:







