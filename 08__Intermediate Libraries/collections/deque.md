# deque
Deque supports adding and removing items from both ends of arrays.
In contrast to lists, which use contiguous memory blocks with elements that are stored next to each other, **deques** are stored in their own memory blocks.

> _deque_: Pronounced 'deck'; short for 'double-ended queue'

```py
import sys, time
from collections import deque

a_deque = deque([3, 4, 5, 6])
a_list = [3, 4, 5, 6]

print(sys.getsizeof(a_deque))  
print(sys.getsizeof(a_list))start_time = time.time()  

for item in range(100000000):  
	a_list.append(item)  
end_time = time.time()  
print("**Append time for LIST:** ", end_time - start_time)start_time = time.time()  


for item in range(100000000):  
	a_deque.append(item)  
end_time = time.time()
print("**Append time for DEQUE:** ", end_time - start_time)start_time = time.time()  

for item in a_list:  
	aa = a_list[200]  
end_time = time.time()  
print("**Lookup time for LIST:** ", end_time - start_time)start_time = time.time()  

for item in a_deque:  
	aa = a_deque[200]  
end_time = time.time()  
print("**Lookup time for DEQUE:** ", end_time - start_time)

# **Output:**
632 (size of deque object in bytes)  
88 (size of deque object in bytes)Append time for LIST:  13.975143671035767   

Append time for DEQUE:  11.940298795700073   
Lookup time for LIST:  8.094613075256348   
Lookup time for DEQUE:  8.974030017852783
```


https://docs.python.org/3/library/collections.html#collections.deque
[Python Deques: Learn What Deques Are Designed For](https://towardsdatascience.com/python-deques-learn-what-deques-are-designed-for-7b345a7adb80)