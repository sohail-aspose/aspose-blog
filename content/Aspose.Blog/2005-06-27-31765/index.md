---
title: 'XmlNodeList live or dead, or who broke the contract.'
date: Mon, 27 Jun 2005 18:03:00 +0000
draft: false
url: /2005/06/27/31765/
author: Romank
summary: ''
tags: ['Roman Korchagin']
---

**XmlNodeList** is an abstract class that represents an ordered collection of XML nodes and it can be returned by **XmlNode.ChildNodes**, **XmlNode.SelectNodes** and **XmlElement.GetElementsByTagName**. The documentation [here][1] clearly states that **XmlNodeList** is a “live” collection so that changes to the children of the node object that it was created from are immediately reflected in the nodes returned by the **XmlNodeList** properties and methods. The interesting thing is that if you retrieve **XmlNodeList** using **ChildNodes** or **GetElementsByTagName** - it is indeed a live collection. Remove or insert a node and bingo - **XmlNodeList** is up to date automatically. However, when you retrieve **XmlNodelist** from **XmlNode.SelectNodes**, - the collection is “semi-live“. That is the nodes are cached as soon as you access them and if say, you access **Count** or the last node - all the nodes will be cached internally and changes to the document will not show through this **XmlNodeList** because the cache is never reset. So it's a nice example of a not so nice thing: **XmlNodeList** is an interface and therefore a contract that is broken by different XmlNodeList implementations. The point is: This code is NOT supposed to work because the collection is live: XmlNodeList shapes = elem.**GetElementsByTagName**(“Shape“); for (int i = 0; i < shapes.Count; i++)     shapes\[i\].ParentNode.RemoveChild(shapes\[i\]); However, this code coincidentally (nastily) works: XmlNodeList shapes = elem.**SelectNodes**(“.//Shape“); for (int i = 0; i < shapes.Count; i++)     shapes\[i\].ParentNode.RemoveChild(shapes\[i\]); I was looking at XmlNodeList in Rotor source and from what I can guess, .NET probably implements it the same way although I did not bother confirming myself.




[1]: https://docs.microsoft.com/en-us/documentation/



