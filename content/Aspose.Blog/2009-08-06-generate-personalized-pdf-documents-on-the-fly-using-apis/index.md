---
title: 'Fairtrade Foundation Uses Aspose.Words to Generate Personalized PDF Documents on the Fly'
date: Thu, 06 Aug 2009 05:13:57 +0000
draft: false
url: /2009/08/06/generate-personalized-pdf-documents-on-the-fly-using-apis/
author: Chris Cranie
summary: ''
tags: ['Aspose.Words', 'Generate Personalized PDF', 'Success Stories']
categories: ['Aspose.Words Product Family']
---

## About Fairtrade Foundation



{{< figure align=center src="images/fairtrade-logo.png" alt="">}}


The Fairtrade Foundation is an independent non-profit organization that licenses the use of FAIRTRADE Mark on products in the UK in accordance with internationally agreed Fairtrade standards.

Our vision is of a world in which justice and sustainable development are at the heart of trade structures and practices so that everyone, through their work, can maintain a decent and dignified livelihood and develop their full potential.

The Fairtrade Foundation has seen significant growth in Fairtrade sales over the last three years which has placed extensive pressure on Fairtrade’s current systems and processes. Furthermore, the Foundation’s ambitious strategy for future expansion will create even more pressure on these systems and processes.

The BPI (Business Process Improvement) project was launched to implement sweeping changes to our internal processes and to enable companies who wish to license products as ‘Fairtrade’ to apply for and manage these products online.

## Requirements Scenario

The Business Processes involved in the project were required to generate personalized PDF documents on the fly which were then printed or sent to the customers. The business users required a facility to update the static content of this document when required with zero development/coding effort.

## Solution

The solution comprises of document templates, web services, Document Generator Engine and associated document generators. The application components instantiate the Document Generator Engine by providing it with a document template type, document template and the keys for obtaining dynamic data. During the instantiation, the Document Generator Engine uses the document template type to get an associated document generator. Finally, the Generate Document method of the document generator is executed to get a PDF document.

During this step, the generator uses the keys and gets the dynamic information from the web services, uses [Aspose.Words][1] to bind it to the merge fields in the document template and then converts it to a PDF document using Aspose.Words.

Microsoft Word documents with static content and merge fields were used as document templates and placed in a central location accessible to both business users and application components.

## Benefits

The project team looked at ways to take dynamic data stored across repositories and create core legal documents. This included various commercial third party products, opensource products, and custom development of a PDF generator.

Binding dynamic data with a Word document and converting it to PDF as well as dynamically generating table rows are hugely complex functionalities and highly time-consuming if developed from scratch. Other tools did not offer the robustness of features to create legal documents in precise formats. Aspose.Words performed these functions out of the box and saved a small IT shop development time and long term costs versus having to maintain a custom solution. Dynamically generating table rows is another feature that was useful to us.

## Future Implementations

The BPI Project consists of two phases, at present we are have had to restrict requirements due to the scale of the project. There is scope for significant expansion in the future; the use of [Aspose products][2] would again be considered given the time saved on development.

## Conclusion

The experience with Aspose.Words has been great so far. It was very intuitive and simple to use and performs most of the functions we required.

**Chris Cranie  
**Fairtrade Foundation




[1]: https://products.aspose.com/words
[2]: https://products.aspose.com/




