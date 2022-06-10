---
title: 'Improved Product Versioning Scheme using Year and Month of the Release'
date: Tue, 25 Oct 2016 05:59:33 +0000
draft: false
url: /2016/10/25/improved-product-versioning-scheme-using-year-and-month-of-the-release/
author: Shahzad Latif
summary: ''
tags: ['News Release']
---

We have recently introduced an improvement in the versioning scheme of our APIs. Earlier, we were using squence-based identifiers for major and minor version numbers; however, we have decided to use the version numbers based on the year and the month in which the API is released. This will help our customers easily identify in which year and month a particular version was released. It will also help them know whether they're using a recent version or an older version.

The format will be as Year.Month.Hotfix Number; for example, 16.10.0, if it is the major release, while if a hotfix is released before the next month then we'll increase the last number as well, like 16.10.1.

Most of our products have started using this new versioning scheme, while the rest will be converting to this format with the upcoming releases.

We hope that this announcement will help avoid any confusion. If you still find any questions or concerns, please feel free to get in touch with us via our [support forums][1]. We'll be happy to hear from you.




[1]: http://forum.aspose.com



