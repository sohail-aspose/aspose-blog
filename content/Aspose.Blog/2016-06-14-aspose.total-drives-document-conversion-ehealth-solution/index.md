---
title: 'Maincare Solutions utilized Aspose.Total Powers for  Document Conversion in an eHealth Solution'
date: Wed, 04 Dec 2019 15:32:27 +0000
draft: false
url: /2016/06/14/aspose.total-drives-document-conversion-ehealth-solution/
author: Pascale Lucas
summary: ''
tags: ['Aspose.Cells for Java supports Excel files to PDF conversion', 'Aspose.Total', 'Aspose.Total for Java for MS Office and PDF files manipulation', 'Aspose.Words for Java to convert DOC DOCX to PDF format', 'Convert PDF to PDF/A-1 format using Aspose.PDF for Java', 'RTF and ODT to PDF and PDF/A-1 Conversion', 'Success Stories']
categories: ['Aspose.Total Product Family']
---

## About Agence eSanté Luxembourg



{{< figure align=center src="images/logoMaincare.png" alt="Maincare solutions logo">}}


[IDO-in][1] has been the leading French eHealth regional platform provider, creating innovative solutions for the exchange and sharing of medical data and for telemedicine. IDO-in becomes Maincare Solutions and its integrated digital agency is now called Digital Initiative. The Security, interoperability and usability are our main concerns to create successful software and services for health professionals and patients.

In 2013, IDO-in was selected by [Agence eSanté Luxembourg][2] to build its national eHealth platform using many IDO-in software ranging from directory, SSO and secured mail system to EHR (_Electronic Health Record_), PHR (_Personal Health Record_) and EMR (_Electronic Medical Record_). In February 2016, Maincare Solutions acquired IDO-in to boost their development in Europe.

## About Agence eSanté Luxembourg

[![Agence eSanté Luxembourg logo][3]](https://blog.aspose.com/2016/06/14/aspose.total-drives-document-conversion-ehealth-solution/attachment/204/)  
[Agence eSanté Luxembourg][4], the national eHealth Agency in Luxembourg, created in October 2011, is operational since March 2012 and started its main activities in September 2012. One of its main roles is enhancing the patient’s care coordination through a better use of healthcare-related data. Agence eSanté has been given five missions, among them were the specification, creation and maintenance of eHealth services including a national Electronic Health Record system named DSP (_Dossier de Soins Partagé_) and the promotion and improvement of interoperability in the healthcare sector.

The “Dossier de Soins Partagé” or DSP, Luxembourg’s EHR, aims at gathering all documents relevant to the patient’s care coordination (_medical and socio-medical_). It is not a replacement for institutions’ EMR nor contains all patient’s data, but instead facilitates the patient’s global handling by providing the most relevant information to all professionals involved, and also to the patient. Indeed, the patient can view all documents from his DSP and has the freedom to send as well some documentation in his DSP in an area called “personal data”. Only professionals having a therapeutic relationship with the patient can access the DSP and they have to be securely authenticated (_e.g. using a smartcard_) and can either use the web portal or an integrated software. Several mechanisms exist to enhance the usability of the DSP, like a timeline view or tree-structure for documents, the possibility for the patient to be helped by a trusted friend or family member or to designate a trusted health professional with privileged access.

## Business Challenges

As said above, documents can be sent by:

*   Patients and their delegates
*   Health professionals having a therapeutic relationship with the patient

These medical documents are critical and are meant to be stored for a long time. That is why they have to be PDF/A-1 conformant (ISO 19005-1) to ensure their readability by any authorized user using any PDF reader at any time, even several years after their submission, without any loss of content or formatting.

So, every time a patient or a health professional having a therapeutic relationship with this patient provides a document to the DSP, a validation is done and only valid PDF/A-1 documents can be stored in the DSP document repository.

The current major problem the DSP is facing is that it is not easy for users to have their documents in the correct PDF/A-1 format so that they can upload them to the platform. We really need to help users by offering them a functionality that will automatically convert any document regardless of its format to the correct PDF/A-1 format which will then be accepted by the platform.

More than 22.000 DSP have been opened so far in this piloting phase and up to 50.000 are expected in the next coming months, representing 10% of the population and more than 8% of everyday patients (population plus the daily commuters from Great Region).

Later on, when the pilot is going to be extended at a larger scale 850 000 DSPs are expected to be opened. So all these patients and their health professionals will benefit from Aspose efficiency.

## Meeting the Requirements with Aspose.Total

As our projects are built using Maven, it seemed essential to us to give our dev teams a simple and intuitive solution making the conversion of documents easier. Thus, we have decided to create an independent project requiring only an additional maven dependency inside other projects.

Our document converter does not require any instantiation of Java objects, its signature has been simplified as much as possible, its first parameter is the InputStream, the second parameter includes its conversion settings (_override and merging of settings and their solutions_), the last parameter being an OutputStream. To implement this converter, we used [Aspose.Words for Java][5] and [Aspose.PDF for Java][6] functionalities to convert between document formats but also to add the pieces of information required by the PDF/A-1 standard.

![General architecture of the solution.][7]

###### Figure 1: General architecture of the solution.

The new document converter module (green) is integrated into our EHR (red).

The setting of the converter inside our existing application has been unnoticeable for our users. We only extended the list of supported MIME types: this list previously contained PDF/A-1 only and now it contains the most common document types (_DOC, DOCX, RTF, ODT, standard PDF_).

The user can now upload his original document on the web portal without worrying about its format. Then the [converted PDF/A-1 document][8] appears, and finally the user can confirm the document submission. The general workflow is left unchanged.

![Showing the integration of the converter into the Health professionals’ portal.][9]

###### Figure 2: Showing the integration of the converter into the Health professionals’ portal.

After writing its medical report using Word for instance (upper right), the user can upload it into the portal (drag-and-drop), in its original format without converting it in PDF himself.

![Preview of converted document (PDF/A-1)][10]

###### Figure 3: Last step: the converted document (PDF/A-1) is displayed to the user who can then confirm its submission to the document repository of the EHR.

The PDF/A-1 document is now shared with all the authorized users (patient and health professionals).

## Alternative Solutions

At the beginning of this project, we searched across the web for some solutions that could meet our needs (conversion of any type of documents into PDF). We found many products but none of them fully met our requirements (_they were difficult to use, not fully functional product, not supported…_). In many articles, [Aspose][11] has been quoted as the best one and was said to solve many issues. We also quickly experimented some solutions and [Aspose][12] appeared to be simple to use and was most efficient at preserving document formatting. Then we extensively tested it with the help of Documentation and Support Forum.

The most important challenge of using [Aspose][13] was to convert any type of document in PDF/A- 1 in order to store them into our IHE XDS document repository. We successfully used [Aspose's Support][14] on some technical issues when the [documentation][15] was incomplete.

In only two months we achieved a fully satisfying solution. Currently only one team uses [Aspose products][16].

## Future Plans for Aspose

We will continue to use [Aspose][17] in the future: we will enhance our conversion module with new features and we will support new types of documents. We plan to integrate it in other products we created. We also plan to use [Aspose.OCR for Java][18] to allow full-text indexing of scanned documents, and [Aspose.Imaging for Java][19] to automatically resize and recompress images inside documents.

## Overall Experience with Aspose.Total for Java

Our experience with [Aspose][20] was great, thanks to its easy way to convert and manipulate many kind of documents. [Aspose products][21] allowed us to meet our objectives. Now with Aspose, we aren't afraid of converting documents into another format. This issue is not straightforward and your solutions solve it simply.

Without any doubt, [Aspose][22] is a great tool to manipulate documents, and is, in our opinion, the best one.




[1]: https://www.ido-in.com/index.html
[2]: https://www.esante.lu/portal/fr/
[3]: https://blog.aspose.com/wp-content/uploads/sites/2/2020/05/204.png
[4]: https://www.esante.lu/portal/fr/
[5]: https://products.aspose.com/words/java
[6]: https://products.aspose.com/pdf/java
[7]: https://blog.aspose.com/wp-content/uploads/sites/2/2019/12/5de7cba48d124_img.png
[8]: https://docs.aspose.com/display/wordsjava/Specify+Rendering+Options+When+Converting+to+PDF#SpecifyRenderingOptionsWhenConvertingtoPDF-CreatingaPDF/ADocumentwithFillableForms
[9]: https://blog.aspose.com/wp-content/uploads/sites/2/2019/12/5de7cba48d54b_img.png
[10]: https://blog.aspose.com/wp-content/uploads/sites/2/2019/12/5de7cba48d8f8_img.png
[11]: https://www.aspose.com/
[12]: https://www.aspose.com/
[13]: https://www.aspose.com/
[14]: https://forum.aspose.com/
[15]: https://docs.aspose.com/dashboard.action
[16]: https://products.aspose.com/total/java
[17]: https://www.aspose.com/
[18]: https://products.aspose.com/ocr/java
[19]: https://products.aspose.com/imaging/java
[20]: https://www.aspose.com/
[21]: https://products.aspose.com/total/java
[22]: https://www.aspose.com/




