---
title: Tutorial 6
updated: 2021-09-22T17:33:48.0000000+12:00
created: 2021-09-22T17:32:49.0000000+12:00
---

Tutorial 6
Wednesday, 22 September, 2021
1:32 PM

![image1](../../../../resources/20a6bbafa15340f6af1feb10a9eee5e6.png)
But yes, roughly speaking the runtime will be n^2. The most important thing is the growth rate. It grows as fast as n^2.
The exact value does not matter so much (but it’s good to be able to calculate it if you need to)

Well, maybe n-1 comparisons, because you need to compare each element to at most all of the others.

The comparison and move is the same in worst case, to the last element it's n - 1, so it should be 1 + 2 + ... + (n -1).

which is something like (n-1)\*n/2
But you also need to compare the pointer to see if you’ve reached the end of the list
