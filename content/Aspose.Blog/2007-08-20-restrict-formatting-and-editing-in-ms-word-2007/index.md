---
title: 'Funny: How the new powerful cryptography implemented in Word 2007 turns it into a perfect tool for document password removal.'
date: Mon, 20 Aug 2007 16:19:00 +0000
draft: false
url: /2007/08/20/restrict-formatting-and-editing-in-ms-word-2007/
author: Miklovan
summary: ''
tags: ['Vladimir Averkin']
---

Today I will talk a bit about Word 2007, its new document format DOCX, and its not very clever implementation of an old MS Word feature called _Document Protection_.

So what is document protection essentially? Called by _Review | Protect Documents | Restrict Formatting and Editing_ in MS Word 2007, it allows you to set different types of protection, including _Readonly_, _Tracked changes_, _Comments_ and _Filling in forms_. Very convenient to prevent undesired changes to the document template, it allows users to edit only certain things in the document or, in read-only mode, disallows editing at all.  It comes as a feature of _DOCX_ format. In _\\word\\settings.xml_ package part it will look like this.

```
<w:documentProtection w:edit=“forms“ w:enforcement=“1“ w:cryptProviderType=“rsaFull“ w:cryptAlgorithmClass=“hash“ w:cryptAlgorithmType=“typeAny“ w:cryptAlgorithmSid=“4“ w:cryptSpinCount=“50000“ w:hash=“0AMSgIVdSif6F5unNC/Lk3rBvr4=“ w:salt=“m3sJnUyPgf0hUjz+U1Sdxg==“/>
```

Of course, this type of document protection can be easily stripped away by removing the line above from the Settings package part. So it is just fool-proof protection, to prevent unintended, accidental change to the documents. That is in fact explicitly stated in Office Open XML spec:

_Document protection is a set of restrictions used to prevent unintentional changes to all or part of a WordprocessingML document - since this protection does not encrypt the document, malicious applications may circumvent its use. **This protection is not intended as a security feature and may be ignored**._

This document protection can be enforced with a password, but again, that is just a foolproof. As the password setting line is exposed in plain text in WordML and RTF you can easily remove the protection if you only know what and where to search.

And now let's look at DOCX implementation. Have you noticed these impressive cryptography attributes? They offer 11 built-in hashing algorithms with the possibility of extending them to an infinite number, using the voluntary number of spins (hashing rounds) and salt (extra line added to password initially) to make it even more secure. Just look what they write about the need for extending of hashing algorithms set:

_This extensibility affords the fact that with exponentially increasing computing power, **documents created in the future will likely need to utilize as yet undefined hashing algorithms in order to remain secure**._

Isn't it (mmm, how to say it mildly) not very clever to use this cryptographical mumbo jumbo to protect things that essentially could not be protected? But the funniest thing is still ahead.

In MS Word 2003 they used a simple hashing algorithm for it and everything was fine. In Word 2003 XML it looked like this:

```
<w:documentProtection w:edit=“forms“ w:enforcement=“on“ w:unprotectPassword=“64CEED7E“ />
```

Of course, you could still go on and remove that line to strip away the protection. But who cares? And that at least required some special knowledge from the person who decided to do this.

In Word 2007 it was decided that the hashing algorithm was not secure enough. (Bwahaha! As if it was ever meant to be secure.) So all these fearful cryptography stuff has appeared. But to maintain compatibility with the previous version old hash stayed. New hashing is put **above** the old hash. So that old hash, calculated and represented as hex string like "7EEDCE64" is used as a source for a secondary, very cryptographical and very secure, hashing.

But what hashing means? Based on hash you can never discover the source string, because the hash is an incomplete reflection of the initial information, like the checksum or CRC code. It cannot be used to restore the hashed string. So storing only secondary hash in the DOCX document you will never be able to find out the primary hash, which is stored in Word 2003 formats. And that means that password hash stored in Word 2007 format can never be reversed to its original form and will inevitably be lost when the document is saved to the old format.

So with all these wise and clever cryptography implemented you no longer need to use any 3rd party editors or tools to remove passwords from the document. **With MS Word 2007 you can remove the document password in seconds just by saving the document to DOC format, closing the word and then opening the saved DOC file again.** You can also use Word 2007 to remove the password from old DOC format. For this, you need to open the DOC file in Word 2007, save it in DOCX, close Word, open file again and repeat the steps described above.

How all that makes sense and why all this stuff was developed and implemented is unclear. Maybe it was intended to be used later, with _Information Rights Management_ software. I have not played with this technology yet but on the first look, it does not seem a very convenient option as all verification is done server-side.







