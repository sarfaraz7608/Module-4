# Classes and Objects in Python: Calculate the Area of a Circle

## 🎯 Aim
To write a Python program that calculates the **area of a circle** based on the radius provided by the user. This program uses a class named `cse` and a method `mech` to perform the calculation.

## 🧠 Algorithm
1. **Get user input**: Take the radius of the circle as input from the user.
2. **Define the class**: Create a class named `cse`.
3. **Define the method**: Inside the class, define the method `mech` to calculate the area of the circle using the formula:  
   Area = pi *r^2 
4. **Execute the program**: Create an object of the class and call the method with the radius value.

## 🧾 Program
```
class cse:
    def mech(self, radius):
        pi = 3.14159
        area = pi * radius ** 2
        return area

radius = int(input("Enter the radius of the circle: "))
circle = cse()
area = circle.mech(radius)
print("Area of the circle:", area)
```

## Output
<img width="1920" height="1080" alt="Screenshot 2025-10-19 162150" src="https://github.com/user-attachments/assets/f9a74b45-343e-45d2-9443-9cffea136944" />

## Result
Thus To write a Python program that calculates the **area of a circle** based on the radius provided by the user. This program uses a class named `cse` and a method `mech` to perform the calculation has been executed sucessfully.


## Dictionary Operations in Python: Merging Two Dictionaries

## 🎯 Aim
To write a Python program that merges **two dictionaries** and combines their key-value pairs.

## 🧠 Algorithm
1. Define two dictionaries `dict1` and `dict2` with some key-value pairs.
2. Define a function `merge()` that merges the two dictionaries using the `**` unpacking operator.
   - The merged result will combine keys from both dictionaries. If a key exists in both, the value from `dict2` will overwrite that from `dict1`.
3. Call the `merge()` function and print the merged dictionary.

## 🧾 Program
```
def merge(dict1, dict2):
    return {**dict1, **dict2}

dict1 = {'a': 1, 'b': 2, 'c': 3}
dict2 = {'b': 4, 'd': 5}

merged_dict = merge(dict1, dict2)
print("Merged dictionary:", merged_dict)
```

## Output
<img width="1920" height="1080" alt="Screenshot 2025-10-19 162506" src="https://github.com/user-attachments/assets/127e1161-eee4-437b-bad8-bd7b1b6fe010" />

## Result
Thus To write a Python program that merges **two dictionaries** and combines their key-value pairs has been executed sucessfully.


# 🔤 Dictionary-Python Program to Sort a Dictionary by Keys and Values

This Python program demonstrates how to sort a dictionary:
- Alphabetically by keys
- Alphabetically by values

---

## 🎯 Aim

To write a Python program that sorts a dictionary's:
- Keys in alphabetical order
- Values in alphabetical order

---

## 🧠 Algorithm

1. **Start the program.**
2. **Define** a dictionary with key-value pairs.
3. **Sort by Keys**:
   - Use `sorted(dictionary.items())`
   - Convert the result to a dictionary using `dict()`
4. **Sort by Values**:
   - Use `sorted(dictionary.items(), key=lambda item: item[1])`
   - Convert the result to a dictionary using `dict()`
5. **Display** the original and sorted dictionaries.
6. **End the program.**

---

## 🧪Program
```
original_dict = {'apple': 'fruit', 'carrot': 'vegetable', 'banana': 'fruit', 'date': 'dry fruit'}

# Sort dictionary by keys
sorted_by_keys = dict(sorted(original_dict.items()))

# Sort dictionary by values
sorted_by_values = dict(sorted(original_dict.items(), key=lambda item: item[1]))

print("Original dictionary:", original_dict)
print("Sorted by keys:", sorted_by_keys)
print("Sorted by values:", sorted_by_values)
```

## Sample Output
<img width="1920" height="1080" alt="Screenshot 2025-10-19 162807" src="https://github.com/user-attachments/assets/757183f6-9fc9-49df-aab6-077711f6ec41" />

## Result
Thus To write a Python program that sorts a dictionary's:
- Keys in alphabetical order
- Values in alphabetical order
has been executed sucessfully

# Exception Handling in Python: Avoiding Index Errors

## 🎯 Aim
To write a Python program that handles an **IndexError** when trying to access an element beyond the available range of a list.

## 🧠 Algorithm
1. Define a list `list1` with some integer elements.
2. Use a **try-except** block:
   - In the `try` block, attempt to access an index that is out of range (e.g., `list1[5]`).
   - In the `except` block, catch the error and print a custom message `"You're out of list range"`.
3. Print the result based on whether the index access succeeds or fails.

## 🧾 Program
```
list1 = [10, 20, 30, 40]

try:
    # Attempt to access an out-of-range index
    value = list1[5]
    print("Accessed value:", value)
except IndexError:
    print("You're out of list range")
```

## Output
<img width="1920" height="1080" alt="Screenshot 2025-10-19 163022" src="https://github.com/user-attachments/assets/14266f4e-9065-40ca-afc2-270d047b0d6b" />

## Result
Thus To write a Python program that handles an **IndexError** when trying to access an element beyond the available range of a list hass been executed sucessfully.


# File Handling in Python: Count Lines Not Starting with 'T'

## 🎯 Aim
To write a Python program that counts the number of lines in a text file `story.txt` that do **not** start with the alphabet `'T'`.

## 🧠 Algorithm
1. Open the file `story.txt` in **read mode**.
2. Initialize a counter `count` to zero.
3. Iterate through each line of the file:
   - Check if the first character of the line is **not** `'T'`.
   - If the line does not start with `'T'`, increment the `count` by 1.
4. After processing all lines, print the `count` value, which represents the number of lines that do not start with `'T'`.

## 🧾 Program
```
count = 0

with open('story.txt', 'r') as file:
    for line in file:
        if not line.startswith('T'):
            count += 1

print("Number of lines not starting with 'T':", count)
```

## Output
```
Number of lines not starting with "T": 3
```
## Result
Thus To write a Python program that counts the number of lines in a text file `story.txt` that do **not** start with the alphabet `'T'` has been exeuted succesfully.
