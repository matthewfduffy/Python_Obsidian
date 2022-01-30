HackerRank
Practice > Python > Introduction > [Arithmetic Operators](https://www.hackerrank.com/challenges/python-arithmetic-operators/problem)

```py
"""
Given two integers, provide a solution where:
1. the first line contains the sum of the two numbers
2. the second line contains the difference of the two numbers (fist - second)
3. the third line contains the product of the two numbers

Sample Input:
3
2

Sample Output:
5	# 3 + 2 = 5
1	# 3 - 2 = 1
6	# 3 * 2 = 6

Constraints:
1 <= a <= 10^10
1 <= b <= 10^10

Base Code:
if __name__ == '__main__':

 a = int(input())

 b = int(input())
"""
```

Solution:
```py
if __name__ == '__main__':
    a = int(input())
    b = int(input())
    #begin solution
    if (a >= 1 and b >= 1) and (a <= 10**10 and b <= 10**10):
        print(a + b)
        print(a - b)
        print(a * b)

```