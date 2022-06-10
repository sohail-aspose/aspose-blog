---
title: 'What Will Come When Windows Get Closed?'
date: Wed, 22 Feb 2006 10:35:00 +0000
draft: false
url: /2006/02/22/42272/
author: DmitryV
summary: ''
tags: ['Dmitry Vorobyev']
---

The history of Microsoft Windows counts more than 20 years. Every new version of this operating system provides us with new features, new level of security, nicer interface. We currently have Windows XP which is extremely popular (maybe the most popular OS ever). We are looking forward to the mighty, stylish, and shining Vista. The enigmatic successor to Vista, code-named Blackcomb, was recently renamed to Vienna…

It is obvious that Windows is flourishing. It is also obvious that the recession is inevitable. So what will succeed to the throne when Windows becomes history?

Nobody knows exactly :) However, there is something looking very similar to a candidate for being the OS of the future. This is the **Singularity** project being researched in Microsoft Research Labs.

**Singularity** is a new software platform designed from scratch. It breaks most of the Windows crucial concepts. It provides new system architecture, new technologies, and several revolutionary innovations that allow designing a superb operating system.

Of course, it is unlikely that **Singularity** as is will become the successor to Windows. But it apparently might become a base for developing a next generation OS by Microsoft. At the moment it is the only project of the Operating Systems group at the Microsoft Research website!

Here is a very brief listing of the **Singularity** innovations and interesting decisions:

*   **Singularity** is written from scratch in a C# extension named _Sing#_.
*   **Singularity** processes have no isolated address spaces. Instead, **Singularity** processes (called _Software-Isolated Processes_, or _SIPs_) are closed _object_ spaces. Two SIPs cannot access the same object simultaneously. Sing# supports message-passing communications and it is just impossible to damage another process programmatically since the messaging API is built into the language. So a **Singularity** system lives in a single virtual address space providing hard boundaries between processes at the same time.
*   **Singularity** supports heterogeneous execution environments. Each process has its own runtime system, with its own memory layout, garbage collection algorithm, and libraries. For example, a process' garbage collector can be selected for its algorithm and data structure layout, without awareness of or coordination with its counterparts in other processes.
*   In **Singularity**, an application consists of a manifest and a collection of resources. To be run, a piece of code must be added to the system by the **Singularity** installer.
*   **Singularity** does not support JIT compilation. Code is compiled before execution including all referenced libraries! The compiler optimizes a code by getting rid of unused classes and applying other smart techniques.
*   **Singularity** does not support run-time reflection services. It is incompatible with the conception of SIPs. A code cannot dynamically load and run another code. Only compile-time reflection (_CTR_) used when compiling an application is supported. For example, applications and device drivers declaratively describe their resource requirements, such as I/O ranges. These descriptions are used to produce safe startup code.

These are only a tiny part of the **Singularity** features. If you are interested, welcome to Microsoft Research:

[http://research.microsoft.com/os/singularity/][1]




[1]: http://research.microsoft.com/os/singularity/



