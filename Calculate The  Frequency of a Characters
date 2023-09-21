In this python program, we will be  Calculating the Frequency of a character in a string or how many times a character is present in a string.

The string is a datatype in programing language and is formed when 2 or more characters join or concatenate together. Now it is not necessary for a string to have a distinct character, it can be meaningless or meaningful can have distinct characters or can be a combination of the same characters.

Check Frequency of Characters in Python

-------------------------------------------------------------------------------Method 1-------------------------------------------------------------------------------

This method is the most naive method –

Iterate on the input string
For each character in string count and prints its frequency
Use .count() method to do so.

string = "Yolo Life"

for i in string:
    frequency = string.count(i)
    print(str(i) + ": " + str(frequency), end=", ")
Output

Y: 1, o: 2, l: 1, o: 2, : 1, L: 1, i: 1, f: 1, e: 1, 

-------------------------------------------------------------------------------Method 2-------------------------------------------------------------------------------

This method uses a dictionary in python.

Iterate on the input string
If a character appears for the first time, add key: char and value: 1
If char already exists in the dictionary increment the value counter by 1 against key char
Run
str = "YOLO LIFE"

# create dictionary to store key value pair
dict = {}

for i in str:
    # if i already appears as key in dict, increment the count
    if i in dict:
        dict[i] += 1

    # else i appears for the first time, add to dict
    else:
        dict[i] = 1

# printing result 
print(dict)
Output

{'Y': 1, 'O': 2, 'L': 2, ' ': 1, 'I': 1, 'F': 1, 'E': 1}

-------------------------------------------------------------------------------Method 3 (Using Counter)-------------------------------------------------------------------------------

This method uses a counter from collections


from collections import Counter
string = "Yolo Life"

output = Counter(string)

print(output)
Output

Counter({'o': 2, 'Y': 1, 'l': 1, ' ': 1, 'L': 1, 'i': 1, 'f': 1, 'e': 1})

-------------------------------------------------------------------------------Method 4 Using Set() and Count()-------------------------------------------------------------------------------

This method is better than the previous method that used count as we are converting the string into a set of unique items.

So, Loop will not run for duplicate items and only for unique items in the set()


string = "aabbbccccdddddeeeeee"

# using set() reduces string "YOLO LIFE" with 20 items
# to a set of 5 items : {'a', 'b', 'c', 'd', 'e'}
# now print count each item in set appearing in string
# storing result as dictionary
# for loop runs only 5 times
res = {i: string.count(i) for i in set(string)}

print(res)
Output

{'a': 2, 'c': 4, 'b': 3, 'e': 6, 'd': 5}
Method 5 Using dict.get()
The get() method returns the value of the item with the specified key.

Run
string = "YOLO LIFE"

res = {}

for key in string:
    # if item doesn't exist res.get(key, 0) returns 0 as result
    # we use res.get(key, 0) + 1 so as to initialize value as 1 on first occurrence
    # if item exits then res.get(key, 0) + 1 just increments the previously held value
    res[key] = res.get(key, 0) + 1

# printing result
print (res)
Output

{'Y': 1, 'O': 2, 'L': 2, ' ': 1, 'I': 1, 'F': 1, 'E': 1}
Note
Time Complexity: O(n), where n is the number of characters in the string.
