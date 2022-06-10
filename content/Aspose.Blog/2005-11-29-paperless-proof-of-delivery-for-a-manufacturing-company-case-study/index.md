---
title: 'Paperless Proof-of-Delivery for a Manufacturing Company made possible using Aspose.Words for .NET'
date: Tue, 29 Nov 2005 12:02:00 +0000
draft: false
url: /2005/11/29/paperless-proof-of-delivery-for-a-manufacturing-company-case-study/
author: Graham Plumb
summary: ''
tags: ['.NET API to process MS Word documents on the Go', 'Aspose.Words', 'Create and update DOC/DOCX files programatically', 'Dynamically process MS Word document', 'Managed Code based .NET API for MS Word files processing', 'Manipulate MS Word documents without Office Automation', 'No License cost for MS Office', 'Success Stories']
categories: ['Aspose.Words Product Family']
---

I am a software developer currently working for a company in the Midlands (UK) that specializes in Manufacturing Software Solutions. Our flagship product is a fully traceable MRP system that can be applied to almost any business situation and tailored (both by the user as well as by us) to fit any level of a company’s day to day operations. Whether it is entering new customer details or tracing were a batch of material originated on the shop floor, our software provides complete transparency and traceability during the manufacturing process.

## Scenario

One of our clients had a requirement for a proof-of-delivery system to tie in with our core product. The process was simple enough i.e. use a PDA to collect a user’s signature at the time of delivery (_in a similar fashion to the bigger distribution companies_) and then merge them into a Word Document template for subsequent storage. In effect, the solution was to harness a paperless method of storing delivery acknowledgments.



{{< figure align=center src="images/paperless-proof-case-study-aspose-words.png" alt="Preview of BluPOD server solution" caption="Image 1:- Preview of BluPOD solution">}}


## Solution

The solution was to be coded using version 1.1 of the .NET framework and C#. Therefore to actually perform the merge of the signature bitmap with a template Word Document, there was a choice. Use the Microsoft Office Primary Interop Assemblies (PIA) or use [Aspose.Words for .NET][1].

## Pros and Cons

The PIA initially seemed like a good approach as it was free, made by Microsoft, and was almost guaranteed to work as they wrote the software which actually creates .DOC files. How could an outside company like Aspose (_which charges for its components_) contend with that?

Well, as it turned out, quite easily!

One of the biggest advantages has been that [Aspose.Words for .NET][2] component was entirely managed code (_written in C#)_ from the ground up. Unlike the Office PIA (_which is just a generated wrapper_), it comes with complete [documentation][3] and has all the benefits of garbage collection, removing the complexities of pointers, memory allocation and correctly casting objects (_unlike the PIA!_). For ease of use alone, this component is streets ahead of the Office PIAs.

However, the crucial factor for any component is performance. In our scenario, several users were synchronizing data concurrently and so the merge had to be performed quickly so that users were not waiting around before obtaining their delivery schedules.

To test this, I wrote 2 programs (_one using the PIAs and one using_ [_Aspose.Words_ for .NET][4] that performed the merge based on a particular bookmark being available in the document template. The resultant document was then saved to a new location. The programs were run 50 times each and the average times for the merge were taken.

**Bookmark Find and Image Insertion Test Results**



{{< figure align=center src="images/paperless-proof-case-study-aspose-words-1.png" alt="">}}


This works out to be just over 8 times faster! The resultant documents were opened in Microsoft Office (2003) and looked visually identical, but there was another significant difference. The document produced by [Aspose.Words for .NET][5] was actually smaller than the original template file (_created in Word 2003_)!

Comparison of the generated .DOC file sizes



{{< figure align=center src="images/paperless-proof-case-study-aspose-words-2.png" alt="">}}


What’s even more impressive is that the code only took 10 lines of code to create using [Aspose.Words for .NET][6] as opposed to 17 using the Office PIAs.

Since the [Aspose.Words for .NET][7] component is written from scratch for .NET, it brings memory savings as the garbage collector can transparently amalgamate related structures in memory, thus using less of it. This is more secure than the Microsoft approach (_which actually loads an entire instance of Word in the background when the constructor is called_) and more suitable for web servers. The security features of the .NET runtime also help to ensure that the [Aspose.Words for .NET][8] component is a more secure approach to use in both desktop and server environments.

Another advantage is that the component is entirely independent of the Microsoft Office suite. This means that documents can be created without having Microsoft Word (_or any of the Office components_) installed. This is a bigger coo than it first seems as corporate licensing for Microsoft products can be very expensive – especially if it is just to run a small program on a computer. By removing this dependency, the license cost can be circumvented for systems that just need to produce .DOC files without any direct user interaction.

## Conclusion

In the original scenario, there were potentially lots of drivers requiring a responsive mechanism of sending signatures to be merged into a word document.

This would simply not have been possible using the Office PIAs as each user would have to either synchronize their data sequentially or the company would have had to buy a supercomputer’s amount of memory to contain multiple instances of Microsoft Word (_not to mention the licensing cost of Word itself!_).

Because of the [Aspose.Words for .NET][9] API, we were able to offer our client a license-free solution that operated in a fast and effective manner. The end result was that the end-user only has to wait seconds for a days’ worth of deliveries to be synchronized with our MRP system. This happened concurrently, reducing the number of times drivers have to wait before making deliveries. This in itself has to lead to further savings as the drivers were freed from the red-tape that used to plague their delivery schedules and can just focus on getting goods to their destination on time.

[Aspose.Words for .NET][10] has enabled the paperless office to become a reality for our client. This product comes highly recommended and is a must-have for any developer’s toolbox. There simply is no real alternative.




[1]: https://products.aspose.com/words/net
[2]: https://products.aspose.com/words/net
[3]: https://docs.aspose.com/display/wordsnet/Home
[4]: https://products.aspose.com/words/net)
[5]: https://products.aspose.com/words/net
[6]: https://products.aspose.com/words/net
[7]: https://products.aspose.com/words/net
[8]: https://products.aspose.com/words/net
[9]: https://products.aspose.com/words/net
[10]: https://products.aspose.com/words/net




