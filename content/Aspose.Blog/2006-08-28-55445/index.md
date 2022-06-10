---
title: 'Prime Numbers - There is a pattern!'
date: Mon, 28 Aug 2006 23:57:00 +0000
draft: false
url: /2006/08/28/55445/
author: DannyCooper
summary: ''
tags: ['Danny Cooper']
---

Hey everyone,

I know this is a bit off topic; however, I thought it may be of interest to the programming community. A while back I discovered there is a pattern to prime numbers. I was very excited to find the pattern, but despite my best efforts I received little to no interest from the math community (this may very well have been because I was looking in the wrong place, but I really feel like I gave it a good effort). Therefore, in order to share the knowledge I thought that I would post it here in hopes that people could help spread the word.

Current mathematics states that there is not a prime pattern; that primes appear along the number line at random. I believe that conclusion was derived because people are looking at primes in a base 10 number system.  
However, in a base 6 number system you will find that the primes form two straight lines (except for 2 and 3… they are special primes, similar to 1). So from a mathematics standpoint the following two equations make up those lines: (1 + 6x) and (-1 + 6x)

You will notice in the above screenshot that there are “skips” within the two lines (for example 25, 35, 49, 55, etc)… I was able to determine that the “skips” are factors of the primes… but not just any factors of the primes; it’s the factors of the primes times the other primes.

Therefore, if one is to calculate a prime – they have to know the number of “skips” that occur within the lines prior to the prime.  I then found that the space between the factors of the primes is a pattern as well. For example with factors of 5 the skips occur every 7th and then 3rd place (starting at 5)… the factors of 7 occur every 9th and 5th place (starting at 7) and so on…

In the end, the following is a true picture of the pattern (from a positive / negative side)...

I have created two different projects using the information I learned about the pattern. In the first project one can pass a number to a function and the function will then return the correct prime. It does so by determining the number of skips and then plugging the information into a math formula. However, it is quite slow when compared to a sieve (especially on very large numbers).  
  
The second project is an improved version of the Sieve of Eratosthenes. It works in a much different fashion since the prime pattern is known. Based on my test so far it is between 100% and 150% faster than the basic sieve. If anyone would like copies of the projects, please feel free to email me for details.  
  
If you know anyone that is interested in this sort of thing, please pass it along. I would love to get this information into the hands of the public.







