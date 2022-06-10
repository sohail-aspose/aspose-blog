---
title: 'Add Animation Effects and Reset Slide Content in PowerPoint Presentations'
date: Fri, 25 Nov 2016 19:24:07 +0000
draft: false
url: /2016/11/25/support-for-new-animation-effects-and-resetting-slide-content-has-been-included-in-aspose.slides-for-.net-16.10.0/
author: Adnan Ahmad
summary: ''
tags: []
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/aspose-Slides-for-net_100.png" alt="">}}


We like to share the release announcement for Aspose.Slides for .NET 16.10.0. We have resolved many issues incurring in the product along with the inclusion of some new features in API as well.

## New Features

We have included some new animation effects for shape in this version. Now, you can also use EffectType.Disapper in animation setting to add disappear shape effect. We have also included support for resetting the slide by adding new property in Slide class by including Reset() method which will reset the position, size and formatting of every shape on slide. We have also included ShowMasterShapes property in IBaseSlide class. It specifies if shapes on the master slide should be shown on slides (ISlide, ILayoutSlide or INotesLides) or not. For master slide itself this property always returns 'false' and doesn't allow to set 'true'.

## Resolved Issues

We have addressed several issues related to charts processing which include improper chart backgrounds, chart border area rendering and improper chart labels. We have also resolved slide cloning issues which include missing content inside cloned presentation as well.

We have rectified several issues related to presentation rendering and it’s exporting to PDF and HTML. The issues related to an improper background color, text rendering and chart element rendering have been rectified as well. We have also addressed several presentation access and saving issues as well in this release that earlier resulted in a different exception when working upon them,

We have made several enhancements to the new API. Please refer to [Aspose.Slides for .NET 16.10.0 Release Notes][1] for further reference.

To download Aspose.Slides for .NET 16.10.0, [please visit the download page][2].




[1]: https://docs.aspose.com/display/slidesnet/Aspose.Slides+for+.NET+16.10.0+Release+Notes
[2]: https://downloads.aspose.com/slides/net/




