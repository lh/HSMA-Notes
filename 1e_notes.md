# Python in a day!

Python is not strongly typed. Assiging a new type will change the type of the variable. Yuck. 


## Variables that store Multiple Items

Lists (list) are sequences of items, where the order matters.  Duplicates allowed. 
```python
[a,B,3,"hello"]
```
Sets (set) are unordered sequences of unique items.
```python
{1,11,7,5,9,3} 
```
Tuples (tuple) are ordered sequences (like a list) but are immutable (once created, they cannot be changed)

```python
("Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday", "Sunday")
```
Dictionaries (dict) are unordered collections of key-value pairs

```python
{"Monday": "1", "Tuesday": "2", "Friday": "5"}
```

##  Forcing type

Use a function to cast type, eg
```python
age = int(input("How old are you? : "))

````
But there are gotchas. It will round a float to an int but it won't round a number expressed as a string.

## Operators

Mainly obvious. 

    % is modulus (ie a%b is remainder of a/b)
    ** is power 
    += 1 is increment by 1
    -= 2 is decrement by 2

