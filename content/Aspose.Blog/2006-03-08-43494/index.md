---
title: 'Aspose.ASPXpand 2.0.2.0 released!'
date: Wed, 08 Mar 2006 00:32:00 +0000
draft: false
url: /2006/03/08/43494/
author: Iret
summary: ''
tags: ['Kyle Huang']
---

Dear Customers,

We have released Aspose.ASPXpand 2.0.2.0!  

What's included in this release:

*    Added a new function named SetupMaxLength  
    This function can be used to limite the maximum number of characters in the multi-line TextBox,and the overload list is :  
         **SetupMaxLength(TextBox textBox,int maxLength)  
         SetupMaxLength(TextBox textBox,int maxLength,string alertMessage)  
    ** The second function will alert the specified alertMessage if the number of characters have reached the maxLength.  
      
    
*    Added new overloading to SetMask() functions  
        **SetMask(Page page,TextBox textBox,string mask,bool alwaysSet,string regx,string alertMessage)  
    **It allow you to use regular expression to restrict the input and will alert the specified message if the user input text did not match the regx when the textbox onBlur.  
      
    
*    Added new overloading to SetupWordCount() function to allow displaying customize message.  
       **  SetupWordCount(TextBox targetTextBox, TextBox displayTextBox, bool showWords, bool showChars,string customizeMessage)  
    ** For example,speicified string "WordCount={w},CharacterCount={c}."  to customizeMessage parameter, the text in the displayTextbox will be something like "WordCount=3,CharacterCount=12.", as you can imagine, the "{w}" in the customizeMessage will be replace with the count of  words while {c} will be replace with the count of characters. 

Thanks very much!







