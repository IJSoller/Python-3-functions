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
list.sort(reverse = True) #sorts a list opposite of alphabetical
list.sort(key = str.lower) #treats all items in list as if they were lowercase

dict = {}
dict[key] = 20 #adds key:20 to the dictionary, so it looks like dict={key:20}

del dict[key] #deletes the key in the dictionary

list.remove("item") #removes item from a list. does NOT take index NUMBER as input- use the actual name of the item.

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
  
list.split() #converts list= ["rando text to split"] into list= ["rando", "text", "to", "split"]. When you use a loop to iterate through the list after splitting it, it iterates through the strings as a whole, not the individual letters.

dict.items() #prints the dictionary
dict.keys() #prints the keys
dict.values() #prints the 

doubles_by_3 = [x*2 for x in range(1,6) if (x*2) % 3 == 0] #returns doubles_by_3 = [6]

list = range(16)
print(filter(lambda x: x% 3 == 0, list)) #reads def lambda(x) - > if x%3==0 with list as input. prints[0, 3, 6, 9, 12, 15

Class Derived(Base)
  def full_time_wage(self, hours):
    return super(Derived, self).Original_Method(arguments, but self is already taken by super fn) #calls the parent method
   
my_file = open("file.txt", "r+") #Allows us to read and write in file
my_file.write("Data to be written) #Writes data to my_file's file. requires a string fn. You MUST close file by my_file.close()
my_file.close() #required after opening
my_file.read() #reads the entire fille
my_file.readline() #reads individual lines

with open("file", "method") as variable: #Read or write to the file

def rando_fn():
   global variable_name
   variable_name = "x" #reassigns a global variable within a local setting
   
try:
  #code that may be messed up here
except Error_here:
  print("Message that indicates something went wrong")

list = [[a, b], [c, d, e]]
list[0][1] -> b #refers to the first list in the list (lol)

cat = ["fat", "orange", "loud"]
size, color, disposition = cat

print('string', end='') #causes the next print statement to immediately follow
print('something')
yields >>> 'stringsomething'

print('cats', 'dogs', 'mice', sep=',') #causes the spaces to dissapear
>>> catsdogsmice

def spam():
  global eggs  #makes the variable global, even though it is in a function
  eggs = spam  #this is a global function, because of the line above
  
def spam(divideBy):
    try:                        # The try and tries the code and ignores the except error
        return 42/divideBy
    except ZeroDivisionError:
        print('Error: Invalid argument')

list2 = copy.copy(list) #allows you to create a copy of a list with a new reference, so you don't modify the original list
copy.deepcopy # copies inner lists

for x in dictionary.values()
  print(v) #prints out the values in a dictionary
  
for x in dictionary.keys():
  print(x)
  
for x in dictionary.items():
  print(x)
  
for k, v in dictionary.items():
  print('Keys ': + k + 'Values: ' v) 
  
'thing' in dictionary.keys #Gives a Boolean if 'thing' is in dictionary. can be used on values or just the dict. Also works with not in.

dictionary.get(key, fallback) #prints the key's value, or the fallback value you enter.

dictionary.setdefault(key, desired_value) #looks for the key. If it is not present, the key and desired value are added to the dict.

import pprint
pprint.pprint(dictionary) #Prints out a cleaner dictionary list
print(pprint.pformat(dictionary)) #Prints it out in string format

'string'.islower() #returns True or False
'string'.isalpha() #returns True if string consists only of letters and is not blank
'string'.isalnum() #returns True if string consists only of letters and numbers and is not blank
'string'.isdecimal() #returns True if string consists only of numbers and is not blank
'string'.isspace() #returns True if string consists only of spaces, tabs, and new lines and is not blank
'string'.istitle() #returns True if string consists only of words that begin with an uppercase letter followed by lowercase letters

'X Y'.startswith('X') #returns True if string starts with X.
'X Y'.endswith('Y') #returns True if string ends with Y.

', '.join(['item 1', 'item 2', 'item 3']) 
>>> 'item 1, item 2, item 3' #join turns a list of strings into a single string and inserts ', ' inbetween. 

'item 1, item 2, item 3'.split()
>>> ['item', '1', 'item', '2', 'item', '3'] #splits a string into a list at whitespaces. Can add string in split to create a divider.

'string'.rjust(10)
'    string' #pads the string to the right for a total string length of 10 spaces. also usable with ljust.

'string'.rjust(10, '-')
'----string'

'string'.center(10, '-')
'--string--'   #works just like rjust and ljust.

Phone_Number_Regex = re.compile(r'\d\d\d-\d\d\d-\d\d\d\d') #compiles the regex object
mo = Phone_Number_Regex.search('My number is 415-555-4242') #searches a string for the regex object
print('Phone number found: ' +mo.group()) # prints 'Phone number found: 415-555-4242'

Regex functions:
| is or. Finds the first item in the object.
()? matches zero or 1 instance of items in the parentheses. 
()* m*atches zero or more instances of items in the parentheses. 
()+ matches one or more instances of items in the parentheses.
(){3,5} greedily matches 3 to 5 instances of the items in the parentheses
(){3,5}? nongreedily matches 3 to 5 instances of the items in the parentheses

mo = Phone_Number_Regex.findall('Cell: 415-555-9999 Work: 212-555-0000')
 # yields ['415-555-9999', '212-555-0000']. You don't have to type in mo.group()
