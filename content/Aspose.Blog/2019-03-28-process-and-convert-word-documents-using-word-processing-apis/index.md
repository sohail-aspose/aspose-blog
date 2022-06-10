---
title: 'IntelAgree Uses Aspose.Words to Process and Convert Word Documents'
date: Thu, 28 Mar 2019 14:24:06 +0000
draft: false
url: /2019/03/28/process-and-convert-word-documents-using-word-processing-apis/
author: Colabs Holdings
summary: ''
tags: ['Aspose.Words', 'Success Stories']
categories: ['Aspose.Words Product Family']
---

## About IntelAgree



{{< figure align=center src="images/IntelAgree.jpg" alt="">}}


IntelAgree is a contract management platform powered by machine learning. We make contracts easier by speeding up the contract process, offering free electronic signatures, and providing a centralized, searchable contract repository.

Many parts of the contract process (create, upload, negotiate) involve the conversion of large and in-depth documents from one file type to another. At times, we are converting from Word to a PDF, and at other times we are converting from Word to HTML. We needed a tool that could do this quickly and securely while maintaining the integrity of each document.

## Problem

Aside from the high-level task of document conversion, we had a list of additional requirements when we set out to find a tool that could work with our platform. As referenced above, high fidelity conversions were paramount. We needed to maintain the integrity of very robust documents when they were converted—to include everything from formatting to pagination to images, pages, and headers and footers.

We also needed to be able to convert back and forth in a way that could track the use of Word for contract negotiation. For example, we needed to consider redlining and the insertion of comments.

Finally, the API was extremely important to us. Because of our customers’ heavy use of track changes and high expectations for the fidelity of documents coming out of our platform, we needed to be confident the API was robust enough to meet our needs.

These issues were all very high priority for us because each and every customer on our platform uses this functionality and would, therefore, be affected by our decision.

## Solution

We chose [Aspose.Words][1] because it met the objectives outlined in the section above, and it met them effectively and continuously performed well. While competitor products had regular conversion errors and issues, Aspose was consistent and fast. (For example, another system we tried took over 30 seconds to convert some documents. Aspose.Words did the same job in just under 5 seconds.) The more we learned about Aspose.Words, the more we realized how important this decision would be as we scale our business. Since hundreds of users (or more!) could be using this functionality on our platform at once, the ability to perform these actions quickly and at a high volume was paramount.



{{< figure align=center src="images/intelagree-case-study-aspose-words.png" alt="">}}




{{< figure align=center src="images/intelagree-case-study-aspose-words-1.png" alt="" caption="An example of a Word document converted to HTML inside IntelAgree">}}


## Experience

**Finding a solution**: When we discovered Aspose.Words, we were actually a year into development using another product. We were not thrilled with that experience and found Aspose.Words after lots of searching for a viable option that would meet all of our requirements and could support .NET Core. We used a free trial to better understand how Aspose.Words could work for us, as well as to perform more robust testing to confirm that the product could hold up to the stress and volume of our platform.

**Implementation**: Implementation and testing took roughly 40 hours in total. We implemented the Aspose.Words library by encapsulating their API and exposing it to our application through our existing interface. This allowed us to quickly switch from the competitor's library to Aspose with no impact on our application. We did not need to use Aspose support—the documentation and examples were excellent and very helpful. Our only challenge was understanding the difference between the “search and replace” functionality in Aspose and our former provider. The approaches were different, and we had to make adjustments in order to have a seamless transition into our platform.

**Outcome**: Our implementation of and experience with Aspose.Words has exceeded our expectations. Based on our research, we were certain it could meet our needs and just needed to make sure it could handle our volume of work. However, we came across two excellent surprises after implementation. First, Aspose.Words offers a very robust way to manipulate properties inside Word documents. This is very helpful for our platform’s integration with Word. Second, we have been extremely pleased with the way Aspose.Words has improved our platform’s ability to extract and understand multi-level lists that originate in Word. Our team feels confident that using Aspose.Words will improve our customer experience drastically.

## Next Steps

Our next focus is to fully leverage Aspose.Words’ conversion of Word documents to HTML throughout our platform to enhance our users’ experience when viewing executed or in-progress contracts.

## Summary

Overall, we have been more than satisfied with [Aspose][2] and Aspose.Words. The product met and exceeded our expectations, checked all the boxes on quite a long list of requirements, and has improved our platform’s speed and functionality. We would gladly recommend Aspose to companies with similar challenges and are open to using other [Aspose products][3] in the future.

**CoLabs Holdings, LLC  
**IntelAgree




[1]: https://products.aspose.com/words
[2]: https://www.aspose.com/
[3]: https://products.aspose.com/




