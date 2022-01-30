HackerRank
Practice > Python > Introduction > [Python If-Else](https://www.hackerrank.com/challenges/py-if-else/problem)

> Given an integer, _n_, perform the following actions:
> if *n* is odd, print Weird
> if *n* is even and inclusive in the range of 2 to 5, print Not Weird
> if *n* is even and in the inclusive range of 6 to 20, print Weird
> if *n* is even and greater than 20, print Not Weird.

```py
"""
Sample Input: 
3

Sample Output:
Weird

Constraints:
1 <= n <= 100

Base:
#!/bin/python3

import math
import os
import random
import re
import sys
 

if __name__ == '__main__':
	n = int(input().strip())
 """
 ```
 
 Solution:
 ```py
 #7/8 Test cases passed. 8.33 of 10
 
 %%if __name__ == '__main__':
	n = int(input().strip())%%
 
 def if_else_test(n):
	while 1 <= n <= 100:
		if n % 2 == 0:
			if n in range(6,20):
				print("Weird")
			else:
				print("Not Weird")
		else:
			print("Weird")
		break
 ```