---
title: 'How to Create a Wrapper to Assist in calling Aspose.Words Methods from Classic ASP.'
date: Fri, 18 May 2007 19:16:00 +0000
draft: false
url: /2007/05/18/how-to-create-a-wrapper-to-assist-in-calling-aspose-words-methods-from-classic-asp/
author: Miklovan
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

As you probably know, it is quite possible to use Aspose.Words in classic ASP applications. Aspose.Words assembly gets registered for COM Interop during setup and it is then possible to use it from classic ASP.  

The following articles provide an interesting example of how to create Aspose.Words powered ASP application without even having Visual Studio installed.

*   [Utilize Aspose.Words from COM Clients (ASP, VB, VBScript][1]
*   [ASP/ASP.NET without Visual Studio - an Instant Primer][2]

However, recently one of our customers reported a problem with calling some of the Aspose.Words API functions from ASP. We have found that some methods, returning type arrays cannot be used from ASP applications because VBScript, as well as javascript, only deal with variant type arrays. In other words, if the method is returning an array of variants then returned value can be assigned and further used in the application code. Otherwise, if the array contains other types of variables, e.g. strings or doubles, then any assignment attempt in ASP fails with 'Type mismatch' error.

After some research, I have found that passing typed arrays to VBScript/javascript callers is impossible. So we had to search for a workaround.

First, I tried to find a suitable way of passing the necessary data, instead of using typed arrays.

For this, I have constructed a make-shift research suite. Here is a sequence of actions that need to be taken to be able to research and debug COM interop with ASP.

Create an ASP application dir. The easiest way is creating a directory in C:\\Inetpub\\wwwroot\\. For example let us create directory C:\\Inetpub\\wwwroot\\dir1.

The next step is creating an ASP file. It is a simple text file with the .asp extension. Here is the content for a simple ASP template:

```
<%@ LANGUAGE=”VBSCRIPT” %>
<%

Option Explicit

‘vbscript code is inserted here

%>
    <HTML>
    <HEAD>
    <META HTTP-EQUIV=”Content-Type” content=”text/html; charset=iso-8859-1“>
    </HEAD>
    <BODY TopMargin=”0” Leftmargin=”0“>
    This is a test.
    </BODY>
    </HTML>
```

Now we are ready to create a simple COM Interop application.

Run Visual Studio. Create new class library project. Let's name the project 'AsposeComWrapper'. Then, let's rename the single existing class in it to 'Methods'.

After this add the reference to aspose.Words library to this project and paste the following content into  'Methods' class: using Aspose.Words;

```
using Aspose.Words;
namespace AsposeComWrapper
{
    public class Methods
    {
        public Methods() {}
        public object GetSomeObject()
        {
            return new object();
        }
    }
}
```

To test the wrapper library you need to compile it, then copy to aSP application directory and register running the following commands from Visual Studio 2003 command prompt:

cd C:\\Inetpub\\wwwroot\\dir1  
regasm AsposeComWrapper.dll /codebase

Then the method can be tested from our test.asp app.

For example we can put the following code into it:

\[VBScript\]

Dim methodWrapper  
Set methodWrapper = CreateObject("AsposeComWrapper.Methods")

Dim x  
x = methodWrapper.GetSomeObject

To test it the following URL should be typed in IE:

<figure class="wp-block-embed"><div class="wp-block-embed__wrapper">http://localhost/dir1/test.asp</div></figure>

The resulting page should show a simple test text: "This is a test."

Otherwise, if some of the method calls in our vbscript will fail we will get a page stating the error together with the number of the line where it happened.

When you need to change wrapper code and run the test app with a new version do the following:  

*   Make necessary changes to the project.
*   Compile it.
*   Restart IIS to release the previous version of DLL, which is currently in use.
*   Copy the resulting DLL to our test ASP dir, overwriting the previous version.
*   Refresh IE with test app's URL in address window.

After making this test suite and spending some time on a lengthy and sometimes frustrating research I have finally found that the only way to pass the array from COM Interop assembly to ASP caller is using an array of variants. In our case with **Document.MailMerge.GetFieldNames** method, the following wrapper can be used: \[C#\]  
using Aspose.Words;

namespace AsposeComWrapper  
{

    public class Methods  
    {

        public Methods() {}

        /// <summary>  
        /// COM Wrapper for Document.MailMerge.GetFieldNames method.  
        /// </summary>  
        public object\[\] GetFieldNames(object doc)  
        {  
            // Get string array from GetFieldNames method.  
            string\[\] names = ((Document)doc).MailMerge.GetFieldNames();  
  
            // Copy string array to an object array.  
            object\[\] array = new object\[names.Length\];  
            names.CopyTo(array, 0);

            // Return the array of objects.  
            return array;  
        }

    }

}  

and to test it in ASP we can use the following code:  

\[VBScript\]  

Dim helper  
Set helper = CreateObject("Aspose.Words.ComHelper")  

Dim doc  
Set doc = helper.Open("C:\\Inetpub\\wwwroot\\dir1\\test.doc")  

Dim methods  
Set methods = CreateObject("AsposeComWrapper.Methods")  

Dim BR  
BR = "<br>"  

Dim element  
For Each element in methods.GetFieldNames(doc)  
  Response.Write(element + BR)  
Next  

As VBScript lacks the possibility of declaring dimensionless array, the only way to use an array of variable length is employing For Each iterator.  

And one more thing that I should not forget to do. You need to set 'read' and 'read and execution' permission for IUSR\_\[ACCOUNTNAME\] account for the file AsposeComWrapper.dll, because ASP uses this account to run. Otherwise, you can encounter 0x800A0046 error when creating the AsposeComWrapper.Methods object.  

That is basically all that you should know to write your own Aspose.Words wrapper for ASP to call Aspose.words methods which cannot be called directly from ASP.




[1]: http://www.aspose.com/Products/Aspose.Words/Api/index.html?url=Utilize_Aspose_Words_from_COM_Clients_ASP_VB_VBScript.html
[2]: http://www.aspose.com/Products/Aspose.Words/Api/index.html?url=ASPASP_NET_without_Visual_Studio_an_Instant_Primer.html




