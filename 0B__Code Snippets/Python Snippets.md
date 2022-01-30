### Basic Algo:

Factorial:
```python
import math

fact_5 = math.factorial(5)
print(fact_5)	# 120
```

Fibonacci Series:
```python
# Option 1
fib = [0, 1]
[fib.append(fib[-2] + fib [-1]) for i in range(8)]
print(fib)	#[0, 1, 1, 2, 3, 5, 8, 13, 21, 34]

# Option 2

```


### Lists:
Access index and values in a list:
```python
numbers = [45, 22, 14, 65, 97, 72]

for i, num enumerate(numbers):
	print(f"index is {i}, value is {num}" )
	
# Result:
index is 0, value is 45
index is 1, value is 22
index is 2, value is 14
index is 3, value is 65
index is 4, value is 97
index is 5, value is 72
```

Check for duplicates in a list:
```python
def dupe_check(x):
    return len(x) != len(set(x))


lst_one = [1, 2, 3, 4, 5]
lst_two = [1, 2, 3, 4, 4, 5, 6]

print(dupe_check(lst_one))  # False (no duplicates)
print(dupe_check(lst_two))  # True - has duplicates
```

Find differences between two lists:
```python
my_set1 = [1, 2, 3, 4, 5]  
my_set2 = [3, 4, 5, 6, 7]  
  
print(list(set(my_set1) - set(my_set2) ))
# {1, 2}
```

Sum a list of integers:
```python
from functools import reduce

def sum_func(arr):
    list_sum = reduce(lambda x, y: x + y, arr)
    return list_sum


arr = [1, 2, 3, 4]
print(sum_funct(arr))
```

### Strings
Check if a string is only letters:
```python
text = "Apple"
print(text.isalpha())	# True

text_num = "Apple100"
print(text_num.isalpha())
```

Check if a string is only numbers:
```python
text = "87946238462"
print(text.isnumeric())	# True

text_alpha = "Apple87946238462"
print(text_alpha.isnumeric())	# False
```

Reverse a String:
```python
string = 'python'

rev_string = string[::-1]
print(rev_string)	#nohtyp
```

### Testing:
Create a Test Array:
```python
arr = []
for i in range(-15, 23, 3):
	arr.append(i)
```

Create a Test String:
```python 
import string
abc = string.ascii_lowercaseprint(abc)  
# 'abcdefghijklmnopqrstuvwxyz'
```


Find most common element(s) in an iterable:
```python
# collections.Counter lets you find the most common
# elements in an iterable:

import collections
>>> c = collections.Counter('helloworld')

>>> c
Counter({'l': 3, 'o': 2, 'e': 1, 'd': 1, 'h': 1, 'r': 1, 'w': 1})

>>> c.most_common(3
[('l', 3), ('o', 2), ('e', 1)]
```

Multiple Input:
```python
a, b, c = input("Enter three inputs ").split()
```

Multiple Input to List:
```python
# runs an infinite loop that accepts user input, appends to a list, and stops when user is finished

input_list = []

def get_input():
	user_input = ''
	while True:
		user_input = input(''' Type your item here and press ENTER (Press Enter if finished):     ''')
		
		if not user_input:
			break
		else:
			input_list.append(user_input)


get_input()
print(input_list)
```

Multiple Variable Assignment:
```python
a, b, c = 10, 3.14, 'python'

print(a, b, c)
# 10 3.14 python
```
```python
a, b, *c = 1, 2, 3, 4, 5	# 1 2 [3, 4, 5]
print(a, b, c)

a, *b, c = 1, 2, 3, 4, 5	# 1 [2, 3, 4] 5
print(a, b, c)

*a, b, c = 1, 2, 3, 4, 5	# [1, 2, 3] 4 5
print(a, b, c)
```

Anagram:
```python
# Anagram Checker
# An anagram is a word or phrase formed by rearranging the letters of another.
# e.g. - 'cinema' can be formed by using the letters in 'iceman'

from collections import Counter

# Option 1
word1 = "below"
word2 = "elbow"

print('anagram') if Counter(word1) == Counter(word2) else print('not an anagram')

# Option 2
def anagram_checker(str1, str2):
	return True if Counter(str1) == Counter(str2) else False

print(anagram_checker('window', 'glass'))
```

Prime Number:
```python
primes = list(filter(lambda x: all(x % y != 0 for y in range(2, x)), range(2, 10)))

print(primes)	# [2, 3, 5, 7]
```


Palindrome:
```python

# Option 1:
string = 'level'
palindrome = string == string[::-1]

print(palindrome)	# True

# Option 2:
phrase.find(phrase[::-1])

# Option 3:
def palindrome_check(str):
	a = str.lower()
	return a == a[::-1]

# Option 4:
def check_palindrome(inputString):
	check_string = inputString.lower()
	return True if check_string == check_string[::-1] else False
```



### Working with files
Add Files to a New .zip file:
```python
def zip_all(path_to_files, zip_file_path):
	"""zip_all:
	Takes a zip filepath name and path to individual files and adds all.
	Function performs doc zip and also returns a list of documents that were added.
	"""
	import os, zipfile
	
	zipped_files = []
	o_dir = os.getcwd()
	with zipfile.ZipFile(zip_file_path, 'a') as zf:
		os.chdir(path_to_files)
		for file in os.listdir(path_to_files):
			zf.write(file, compress_type=zipfile.ZIP_DEFLATED())
			zipped_files.append(file)
	os.chdir(o_dir)
	return zipped_files

# Edit function call to zip files
zipped_files = zip_all(r'<PATH TO FOLDER WITH FILES>', r'C://Users/12345/Desktop/My_New_ZipFile.zip')
```

Read File and Input to a List:
```python
lis = [line.strip() for line in open('gfg.txt', 'r')]
```
