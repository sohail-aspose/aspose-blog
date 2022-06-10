---
title: 'Metronik Uses Aspose.Words to Generate Templates Quickly without MS Word'
date: Mon, 13 May 2019 13:42:19 +0000
draft: false
url: /2019/05/13/generate-templates-without-reliance-on-ms-word/
author: Marjan Kaligaro
summary: ''
tags: ['Aspose.Words', 'Success Stories']
categories: ['Aspose.Words Product Family']
---

## About Metronik



{{< figure align=center src="images/Metronik.png" alt="">}}


Metronik has been close to the EU GP industry since its incorporation nearly three decades ago and is a trusted partner of leading GP companies (e.g. Novartis, Teva, Stada, Krka). By combining our extensive knowledge of their manufacturing processes with state-of-the-art automation and digitalization technology, we have been helping our GP clients improve management and control of their processes, identify cost-saving opportunities and develop optimization initiatives. The ability to incorporate new technological developments into our solutions has brought Metronik to where it is today – we are the leading high-tech company in CEE in the field of Industry 4.0 solutions with 115 employees and 16.1 million EUR in revenue.

## Problem

In the Pharmaceutical industry, documentation is the key to GMP compliance and ensures traceability of all development, manufacturing, and testing activities. Documentation provides the route for auditors to assess the overall quality of operations within a company and the final product.

## Solution

Based on the objectives above we evaluated multiple possibilities that were rejected due to various reasons (long generation times of over 20 seconds/document, dependence on Word Interop components, …). In the end, we tried [Aspose.Words][1] which proved perfect for our needs. During the POC phase, we confirmed the main objective of generating templates quickly without reliance on MS Word on the server-side plus we performed a stress-test (12 hours of document generation with 5+ concurrent requests to our server) which [Aspose.Words][2] survived without any problems.



{{< figure align=center src="images/metronic-aspose-words-case-study-762x1024.png" alt="" caption="An example of a generated template.">}}


## Experience

**Finding a solution**: the need for such a solution arose when we migrated an old Windows Form based application to a Web-based one. We evaluated a couple of possible solutions that we found through previous experience and “Google searches”. All of these took more than a couple of months before we found Aspose.Words.

**Implementation**: For the initial Proof of Concept we used the free trial license that proved exceptional and due to great documentation we needed only a couple of days to implement the component and test it. As the documentation and examples are self-explanatory we didn’t need any specific support input from Aspose. The actual component was wrapped as a separate task which is being run by our scheduling service on a server.

**Outcome**: The implementation was a success and our customers confirmed the POC. Based on that we are currently finishing the production version of the implementation and are already planning an updated version of our templating service as [Aspose.Words][3] provides a lot of features that were not present in previous providers.

## Next Steps

In the next step, we are planning to implement the Aspose component(s) into all the products that we offer. The first next thing that we are planning to implement is Aspose.Words’ feature of converting Word documents to HTML which will enable “online preview” functionality to our users so they will be able to see what will be printed upfront. Alongside we are reviewing the possibility of using additional Aspose components from the [Aspose.Total][4].

## Summary

Overall we are extremely satisfied with the feature set of Aspose components and with the documentation that is available as this is crucial for a fast and stable implementation. The product met and even exceeded our initial expectations and we are looking forward to using further features in the upcoming versions of our software.

**Marjan Kaligaro  
**Assistant Director VPI  
Metronik d.o.o.




[1]: https://products.aspose.com/words
[2]: https://products.aspose.com/words
[3]: https://products.aspose.com/words
[4]: https://products.aspose.com/total




