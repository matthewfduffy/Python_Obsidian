#python-standard-library
# deque
Deque, pronounced 'deck', and short for "double-ended queue(s)", is part of the collections module in Python.
The advantage of deque over lists or other arrays is that it supports adding and removing items from ==both ends== of an array.

You can also mimic FIFO queues with deque. That is, a deque will only hold the number of items you specify -- never any more. If you add a new item to a deque that is at it's maximum defined length, the oldest element in the deque will be popped off in a First in, First out (FIFO) structure.

```python
# Example of FIFO functionality using deque

from collections import deque

my_deck = deque(maxlen = 3)		# create a new deque with 3 (or less) elements

my_deck.append(1)				# adding first three elements
my_deck.append(2)		
my_deck.append(3)				

print(my_deck)					# Note: The deck is now full	 
# deque([1, 2, 3])

my_deck.append('extra')			# adding a new element to a deque at it's max storage
print(my_deck)					
# deque([2, 3, 'extra'])		# the first element has been dropped from the deque
```

Elements in deques can be manipulated in other ways:
```python
...
my_deck = deque(maxlen=3)
my_deck.extend([1, 2, 3])
print(my_deck)
# deque([1, 2, 3])



# Rotate to the right (default)
my_deck.rotate()				#deque([3, 1, 2])

# Rotate to the Left
my_deck.rotate(-1)				# deque([1, 2, 3])
my_deck.rotate(-1)				# deque([2, 3, 1])

# Append to Left
my_deck.appendleft('left')		# deque(['left', 1, 2])

# Extend to Left
my_deck.extendleft(['d', 'd'])	# deque(['d', 'd', 'left'])

# Pop Left
my_deck.popleft()				# deque(['d', 'left'])

# Remove element by name
my_deck.remove('left')			# deque(['d'])

```










```python
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


[Official Python Documentation: Deque](https://docs.python.org/3/library/collections.html#collections.deque)
[Python Deques: Learn What Deques Are Designed For](https://towardsdatascience.com/python-deques-learn-what-deques-are-designed-for-7b345a7adb80)
[Introduction to Python deque()](https://medium.com/gustavorsantos/introduction-to-python-deque-d6402282fe92)


%%In contrast to lists, which use contiguous memory blocks with elements that are stored next to each other, **deques** are stored in their own memory blocks.%%