---
title: 'Surgical Notes Inc. Uses Aspose.Words to Write and Print Data to Documents without Microsoft Word'
date: Fri, 29 May 2009 17:15:47 +0000
draft: false
url: /2009/05/29/write-and-print-data-to-documents-without-opening-microsoft-word/
author: Stenson
summary: ''
tags: ['Aspose.Words', 'Success Stories']
categories: ['Aspose.Words Product Family']
---

## About Surgical Notes Inc.



{{< figure align=center src="images/Surgical-Notes.png" alt="">}}


Surgical Notes, Inc., based in Dallas, Texas, is a leading innovator in administrative medical technology. The company’s flagship product, SN Chart, revolutionized medical transcription and is currently used by more than 14,500 physicians at over 400 facilities nationwide.

Managing the administrative cost of medicine is important to all stakeholders –doctors, administrators, insurance companies and patients. Unfortunately, upwards of 25% of all medical costs currently relate to the administrative components, not patient care. To help the ASC market contain cost and realize operational efficiencies, Surgical Notes developed an electronic medical records product VMR Express.

VMR Express allows medical offices to electronically prepare medical charts at the time of the patient encounter. All of the forms are created as templates in Microsoft Word and the program automatically generates a barcode on the documents and pre-fills patient data. This saves the medical facilities from using preprinted forms, allows the forms to be scanned for electronic retrieval and eliminates costly sticky labels commonly used to “place” patient data on charts.

## Requirements Scenario

The developers of VMR Express were presented with several challenges. Medical facilities are immediately moving to electronic records and the target was to quickly deliver a product to market without sacrificing quality. As Brian Meredith, Senior Vice President for Development stated:

“Our customers have known Surgical Notes as a strong partner. They have consistently received a high-quality product and top-notch customer service. Although the goal was to bring a product to market quickly, under no circumstances would the company sacrifice any of its quality standards and we did not want one shortcoming to undermine the project as an entirety.”

The company first attempted automation through the Microsoft Word VBA interop, freely available from Microsoft. This was unsuccessful. In addition to completing the forms, printing each form has its own settings for the printer, paper tray, simplex or duplex, rotation, et cetera. The automation through the freely available Microsoft Office SDK simply could not handle the constant setting changes and forms that were designed to print on plain paper, for example, printing on expensive label sheets. The company needed a solution.

“A typical chart might be consist of more than 20 different Word documents. When printing through the standard word automation, it just didn’t work. It was time-consuming and prone to failure. We needed a reliable solution”, continued Meredith.

In addition, the company’s test product not only had to open Microsoft Word and each document to send the form to the printer, but Microsoft Word and each form file had to be opened to write the patient data to the various fields. A typical chart could take several minutes to prepare.  
Meredith was quick to address this challenge. “In addition to wanting to solve the printing issues, we also wanted a mechanism to write data to Microsoft Word document fields without opening the document or Microsoft Word. We found the solution in [Aspose][1].”

## Solution

Utilizing VB.NET 2008, the programming team created a straight forward application to control printer properties and write data to the various Word document form fields. The programmers then made a COM-accessible object and implemented the solution into the existing VB6-based electronic medical records product.

“Testing and debugging of the product were relatively easy” explained Meredith. “After we configured our application, we tested several test packets. Our project is complex, so it took a few hours to debug code and apply all settings properly. We were very pleased with the results and level of support from ASPOSE.”

## Benefits

Surgical Notes is confident that both it and its customers are the true winners with [Aspose.Words][2]. Using the product, Surgical Notes was able to:

*   Solve a technical task of continually changing printers
*   Solve a technical task of setting complex printer settings, including paper trays, duplex mode, number of copies and destination printer.
*   Print a Microsoft Word document without opening Microsoft Word
*   Write data to a Microsoft Word document without opening Microsoft Word.

Not only was Surgical Notes able to quickly address a growing concern over document printing, but the company was also able to provide a faster product for its clients. When the developers used the ASPOSE.WORDS component instead of the Microsoft automation SDK, an added benefit was that documents could be prepared and printed without opening Microsoft Word. This provided a time savings of approximately 3 minutes per / forms package.

## Conclusion

A major differentiation in any software product is quality. In this case, the quality of the [Aspose.Words][3] component has helped Surgical Notes achieve its quality standards for its new electronic medical records component and provided significant savings in development time and document preparation time.

Developers often look to components to achieve complex tasks, yet sometimes the objectives are as simple as programmatically completing forms and printing documents. While SDK tools and components from Microsoft were able to complete much of this, the office SDK available from Microsoft could not compare with the stability, rich features, and “code only” solution offered by [Aspose.Words][4].



{{< figure align=center src="images/surgical-notes-case-study-aspose-words.png" alt="">}}




{{< figure align=center src="images/surgical-notes-case-study-aspose-words-1.png" alt="">}}




{{< figure align=center src="images/surgical-notes-case-study-aspose-words-2-1024x640.png" alt="">}}




{{< figure align=center src="images/surgical-notes-case-study-aspose-words-3-1024x640.png" alt="">}}




{{< figure align=center src="images/surgical-notes-case-study-aspose-words-4-1024x640.png" alt="">}}




{{< figure align=center src="images/surgical-notes-case-study-aspose-words-5-1024x640.png" alt="">}}


**Stenson, Eric J  
**Virtual Medical Records  
Surgical Notes, Inc.




[1]: https://www.aspose.com/
[2]: https://products.aspose.com/words
[3]: https://products.aspose.com/words
[4]: https://products.aspose.com/words/family




