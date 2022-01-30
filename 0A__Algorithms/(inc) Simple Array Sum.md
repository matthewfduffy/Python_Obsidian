HackerRank
Practice > Algorithms > Warmup > [Simple Array Sum](https://www.hackerrank.com/challenges/simple-array-sum/problem)

https://stackoverflow.com/questions/52760487/python-keyerror-output-path
%%solve "OUTPUT_PATH" error%%
> Given an array of integers, find the sum of its elements as an integer

```py
"""Given an array of integers, find the sume of its elements as an integer

Constraints:
0 < n, ar[i] <= 1000

Format:
The first line contains an integer, _n_, denoting the size of the array
The second line contains n space-separated integers representing the array's elements

Sample Input:
6
1 2 3 4 10 11

Sample Output:
31

Base:
#!/bin/python3"""

import os
import sys

# Complete the simpleArraySum function below.

def simpleArraySum(ar):
 #
 # Write your code here.
 #
  

if __name__ == '__main__':
 	fptr = open(os.environ['OUTPUT_PATH'], 'w')
	
	ar_count = int(input())
	ar = list(map(int, input().rstrip().split()))
	result = simpleArraySum(ar)
	fptr.write(str(result) + '\n')
	fptr.close()

```