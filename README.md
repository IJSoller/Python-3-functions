# Python-3-functions

print("") or print()
print(dict[keys]) #prints keys 

type(x) #returns the type of variable/data

print(type(x)) #gives more info

type(type(x)) #gives type

"x" + "y" gives "xy". "x " + "y" gives "x y".

max(1, 2, 3, 4) #gives largest number. This one would give 4. 

min(x, y, z)

abs(x) #gives the absolute value

list[0] #accesses the first item in a list.
list[0:2] #slices the list, accessing the 0 and 1 items.

x= "string"
x[0] #accesses the first character in a string.
x[0:2] #accesses the 0 and 1 character in the string.


list.append("y") #adds y to the end of a list

list.index(x) #finds x in the list

list.insert(2, x) #inserts x at index 2, and pushes everything down.

list.sort() #sorts a list alphabetically or numerically

dict = {}
dict[key] = 20 #adds key:20 to the dictionary, so it looks like dict={key:20}

del dict[key] #deletes the key in the dictionary

list.remove["item"] #removes item from a list. does NOT take index NUMBER as input- use the actual name of the item.

dict[list_in_dict].list_function() #this is the general layout for using a list command on a list nested in a dictionary

list[index number] = x #replaces the object at index number with x.

n.pop(index number) #deletes the index and returns it

del(list[index number]) #deletes the index 

range(6) #creates a list from 0 to 5
range(1,6) #creates a list from 1 to 5
range( 1, 10, 3) #creates a list of 1, 4, and 10. 

print list_containing_lists[list][item number in that list] #allows you to access an item in a list when that list is in a list

print(something), #prints stuff on the same line

for index, item in enumerate(list):
  print index + 1, item
  # prints numbers along side list items
  
#the zip function will create pairs of elements when passed two or more lists, and will stop at the end of the shorter list
list_a = [1, 2, 3]
list_b = [4, 5, 6]
for a, b in zip(list_a, list_b):
  
list.split() #converts list="rando text to split" into list="rando", "text", "to", "split". When you use a loop to iterate through the list after splitting it, it iterates through the strings as a whole, not the individual letters.

dict.items() #prints the dictionary
dict.keys() #prints the keys
dict.values() #prints the 

doubles_by_3 = [x*2 for x in range(1,6) if (x*2) % 3 == 0] #returns doubles_by_3 = [6]

list = range(16)
print(filter(lambda x: x% 3 == 0, list)) #reads def lambda(x) - > if x%3==0 with list as input. prints[0, 3, 6, 9, 12, 15

