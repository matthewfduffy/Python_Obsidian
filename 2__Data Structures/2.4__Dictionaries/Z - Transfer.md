Once you have a dictionary, you can access the values in it by providing the key. For example, let’s imagine we have a dictionary that maps buildings to their heights, in meters:

```py
building_heights = {"Burj Khalifa": 828, "Shanghai Tower": 632, "Abraj Al Bait": 601, "Ping An": 599, "Lotte World Tower": 554.5, "One World Trade": 541.3}

# Then we can access the data in it like this:

>>> building_heights["Burj Khalifa"]
828

>>> building_heights["Ping An"]
599
```
  
  

One way to avoid this error is to first check if the key exists in the dictionary:
```py
key_to_check = "Landmark 81"  
  
if key_to_check in building_heights:  
 print(building_heights["Landmark 81"])
```

This will not throw an error, because key_to_check in building_heights will return False, and so we never try to access the key.

# Try/Except to Get a Key

We saw that we can avoid KeyErrors by checking if a key is in a dictionary first. Another method we could use is a try/except:
```py
key_to_check = "Landmark 81"

try:
	print(building_heights[key_to_check])
except KeyError:
	print("That key doesn't exist!")
```
When we try to access a key that doesn’t exist, the program will go into the except block and print "That key doesn't exist!".

# Safely Get a Key

We saw in the last exercise that we had to add a `key:value` pair to a dictionary in order to avoid a KeyError. This solution is not sustainable. 
We can’t predict every key a user may call and add all of those placeholder values to our dictionary!

Dictionaries have a `.get()` method to search for a value instead of the `my_dict[key]` notation we have been using. 
If the key you are trying to `.get()` does not exist, it will return None by default:
```py
building_heights = {"Burj Khalifa": 828, "Shanghai Tower": 632, "Abraj Al Bait": 601, "Ping An": 599, "Lotte World Tower": 554.5, "One World Trade": 541.3}

#this line will return 632:
building_heights.get("Shanghai Tower")

#this line will return None:
building_heights.get("My House")
```
You can also specify a value to return if the key doesn’t exist. For example, we might want to return a building height of 0 if our desired building is not in the dictionary:
```py
>>> building_heights.get('Shanghai Tower', 0)
632

>>> building_heights.get('Mt Olympus', 0)
0

>>> building_heights.get('Kilimanjaro', 'No Value')
'No Value'
```

# Delete a Key

Sometimes we want to get a key and remove it from the dictionary. Imagine we were running a raffle, and we have this dictionary mapping ticket numbers to prizes:
```py
raffle = {223842: "Teddy Bear", 872921: "Concert Tickets", 320291: "Gift Basket", 412123: "Necklace", 298787: "Pasta Maker"}
```
When we get a ticket number, we want to return the prize and also remove that pair from the dictionary, since the prize has been given away. We can use .`pop()` to do this. 
Just like with `.get()`, we can provide a default value to return if the key does not exist in the dictionary:
```py
>>> raffle.pop(320291, "No Prize")
"Gift Basket"

>>> raffle
{223842: "Teddy Bear", 872921: "Concert Tickets", 412123: "Necklace", 298787: "Pasta Maker"}

>>> raffle.pop(100000, "No Prize")
"No Prize"

>>> raffle
{223842: "Teddy Bear", 872921: "Concert Tickets", 412123: "Necklace", 298787: "Pasta Maker"}

>>> raffle.pop(872921, "No Prize")
"Concert Tickets"

>>> raffle
{223842: "Teddy Bear", 412123: "Necklace", 298787: "Pasta Maker"}
```

`.pop()` works to delete items from a dictionary, when you know the key value.

```py
available_items = {"health potion": 10, "cake of the cure": 5, "green elixir": 20, "strength sandwich": 25, "stamina grains": 15, "power stew": 30}

health_points = 20

health_points += available_items.pop("stamina grains", 0)

health_points += available_items.pop("power stew", 0)

health_points += available_items.pop("mystic bread", 0)

print(available_items)

print(health_points)
```



# Get All Keys

Sometimes we want to operate on all of the keys in a dictionary. For example, if we have a dictionary of students in a math class and their grades:
```py
test_scores = {
	"Grace":[80, 72, 90], 
	"Jeffrey":[88, 68, 81], 
	"Sylvia":[80, 82, 84], 
	"Pedro":[98, 96, 95], 
	"Martin":[78, 80, 78], 
	"Dina":[64, 60, 75]
}
```
We want to get a roster of the students in the class, without including their grades. We can do this with the built-in `list()` function:
```py
>>> list(test_scores)
["Grace", "Jeffrey", "Sylvia", "Pedro", "Martin", "Dina"]
```



# Get All Items
You can get both the keys and the values with the `.items()` method. Like `.keys()` and `.values()`, it returns a `dict_list object`. 
Each element of the `dict_list` returned by `.items()` is a tuple consisting of:
	(key, value)

so to iterate through, you can use this syntax:
```py
biggest_brands = {"Apple": 184, "Google": 141.7, "Microsoft": 80, "Coca-Cola": 69.7, "Amazon": 64.8}

for company, value in biggest_brands.items():
	print(company + " has a value of " + str(value) + " billion dollars. ")
```
which would yield this output:
```
Apple has a value of 184 billion dollars.
Google has a value of 141.7 billion dollars.
Microsoft has a value of 80 billion dollars.
Coca-Cola has a value of 69.7 billion dollars.
Amazon has a value of 64.8 billion dollars.
```
  
  
  
```py
pct_women_in_occupation = {
	"CEO": 28, 
	"Engineering Manager": 9, 
	"Pharmacist": 58, 
	"Physician": 40, 
	"Lawyer": 37, 
	"Aerospace Engineer": 9
	}

for key, value in pct_women_in_occupation.items():
	print(f'Women make up {value} percent of {key}s')
```