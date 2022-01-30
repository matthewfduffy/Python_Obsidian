HackerRank
Practice > Python > Introduction > Print Function

![[Pasted image 20210421063434.png]]

```py
"""
Given an integer n, print all integers from 1 to n as a string without spaces.

Constraints:
+ Without using string methods
+ 1<= n <= 150

Sample Input:
> 3

Sample Output:
> 123

Base:

#Python 2
from __future__ import print_function

if __name__ == '__main__':
    n = int(raw_input())

#Python 3
if __name__ == '__main__':
    n = int(input())
"""
```


Solution:
```py
if __name__ == '__main__':
	n = int(input())
	#begin solution
 	new_string = ""

   	if n >= 1 and n <= 150:
		for i in range(1, n +1):
			new_string += str(i)

 	print(new_string)
```