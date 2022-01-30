HackerRank
Practice > Python > Introduction > [Write a Function](https://www.hackerrank.com/challenges/write-a-function/problem)

```py
"""
Given a year, determine whether it is a leap year. Return boolean `True`, otherwise return `False`.

Sample Input:
1990

Sample Output:
`False`

Base:

def is_leap(year):
	leap = False

# Write your logic here

	return leap

  

#base - do not modify
year = int(input())
print(is_leap(year))
"""
```

>Notes:
>An extra day is added to the calendar almost every four years as February 29, and the day is called a _leap day_. It corrects the calendar for the fact that our planet takes approximately 365.25 days to orbit the sun. A leap year contains a leap day.
>
>In the Gregorian calendar, three conditions are used to identify leap years:
>
>-   The year can be evenly divided by 4, is a leap year, unless:
>    -   The year can be evenly divided by 100, it is NOT a leap year, unless:
>        -   The year is also evenly divisible by 400. Then it is a leap year.
>
>This means that in the Gregorian calendar, the years 2000 and 2400 are leap years, while 1800, 1900, 2100, 2200, 2300 and 2500 are NOT leap years.

Solution (8/10):
```py
def is_leap(year):
    leap = False

# Write your logic here
    if year % 4 == 0:
        if year % 100 == 0:
            if year % 400 == 0:
                leap = True
                            
    return leap

  

#base - do not modify
year = int(input())
print(is_leap(year))
```