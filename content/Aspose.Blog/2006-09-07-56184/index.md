---
title: 'Class Design: Which is the Best?'
date: Thu, 07 Sep 2006 20:27:00 +0000
draft: false
url: /2006/09/07/56184/
author: DmitryV
summary: ''
tags: ['Dmitry Vorobyev']
---

What class design do you prefer? I assume most of you follow Microsoft guidelines, and it's reasonable. However, practice shows that not all the recommendations should be blindly obeyed. I don't imply here fundamental rules like "never make instance fields public" (yet this also might be broken in some rare cases – imagine you have an internal class representing a low-level data structure with several hundred fields!). I'm rather speaking of naming conventions, order of members, and some other stuff related to the appearance of a class. I wanted to share few class design rules that seem different from most popular guidelines but proved to be useful to me and my teammates. I supplied each recommendation with a practical explanation of the reason.

**Naming Conventions**

_Use **m** prefix for instance fields and **g** prefix for static fields + Pascal style name._

**Why?** Despite Microsoft recommendations, including prefixes in field names seems useful due to several reasons:

*   Field identifiers cannot be mixed up with other identifiers, e.g. those of properties or local variables.
*   No need in color highlighting (for example, offered by the ReSharper plug-in) to distinct field identifiers.
*   IntelliSense sorts fields together thanks to the same prefix.
*   Field look more "class level" than say when using camel style

It seems like controls should be the only exception. There is no strict opinion how to name the fields holding controls. I don't like both the popular styles: neither including a prefix (such as **txtCustomerName**) because Hungarian notation is considered obsolete in .NET, nor ending the field name with the control's class name (too long – imagine something like **CompilationResultsRichTextBox3**). So I'm just using Pascal casing (instead of camel casing offered by VS designers) until I find a better rule.

**The Order of Members**

_The order of members inside a class:_

_Ctor  
Methods  
Static ctor  
Properties  
Fields_

**Why?** Methods go first because when you open a source file in an editor, the first thing you want to read is normally what the class DOES rather than what data it works with. The instance constructor is the "initializing" method so it goes very first. The static constructor goes last because it's usually the least "important" of the methods – it normally contains nothing but static field initialization. Properties might be treated as a hybrid of fields and methods so it's logical to place them in the middle; another argument is that most properties are nothing but field accessors, hence they should be placed closely to fields. Fields are last because they are usually the last thing you want to get familiar with when exploring a class.

One can argue that it's reasonable to keep fields and their "wrapping" properties together. Yes, it makes sense because it allows easily remove a field and corresponding property if needed. However, inconsistency is our natural enemy so if we agreed to physically separate the code of the methods and the data they work with, let's stick with this rule.

It's a moot point which is the best place for events (not shown on the list), probably between static ctor and properties.

_The order of members inside each group:_

_Public  
Internal  
Protected  
Private_

(Don't know where to put **protected internal** – have you ever had to create any? )

**Why?** Mostly because less visible methods are normally invoked from more visible ones. There may be exceptions from this ordering for example if a private method is a helper method called from one or more public methods; in this case it's acceptable to place this private method right after the public method(s).

**Other Rules**

_Always explicitly specify the visibility of a class and its members._

**Why?** Just because it makes code more readable.

_If a method does not refer to any of the instance fields, make it static._

**Why?** Because you can easily extract it later for example to a utility class.

_Do not use **#region** blocks._

**Why?** Class shouldn't be so large to demand the use of **#region**. Refactor the class to a couple of smaller classes. Perhaps regions would still be useful say for separating methods and fields but they don't seem to have a decent support in VS (I was amazed when discovered that collapsing regions makes the contents not searchable).

So a "proper" class should look as follows:

    public class ProperClass  
    {  
        public ProperClass(int field1, int field2)  
        {  
            mField1 = field1;  
            mField2 = field2;  
        }  
         
        public void PublicMethod()  
        {  
            InternalMethod();  
             
            // ...  
        }

        internal void InternalMethod()  
        {  
            int result = PrivateMethod(mField1);  
             
            // ...  
        }  
         
        private int PrivateMethod(int inputValue)  
        {  
            // ...  
        }  
         
        private static string PrivateStaticMethod(string value)  
        {  
            return (string)gSomeMap\[value\];  
        }  
         
        static ProperClass()  
        {  
            gSomeMap = new Hashtable();  
              
            gSomeMap.Add("Value1", "MappedValue1");  
            gSomeMap.Add("Value2", "MappedValue2");  
             
            // ...  
        }

        public int Field1  
        {  
            get { return mField1; }  
        }

        internal int Field2  
        {  
            get { return mField2; }  
            set { mField2 = value; }  
        }

        private int mField1;  
        private int mField2;

        private static readonly Hashtable gSomeMap;  
    }







