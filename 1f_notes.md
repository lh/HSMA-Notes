# Python: handling errors

There is a common pattern on e.g. user input:
```python

    try: 
        age = int(float(input("How old are you? "))) # always runs
        break # only gets here if no error - goes to "finally:"
    except ValueError: # only if there is an error
# this is what to do if there is an error
        print(
            f"I'm sorry, that was not a valid answer. Please enter your", 
            f"age in years as a number: "
            )
        continue # this says can go back to the "while" but first do:
    finally: # this code always runs before restarting the "while"
        print("This is a great little app!")

```

# Numpy

All the routines for handling arrays quickly live here. 

Some examples of array creation:
### Create a 1D array from a list
```python
list1 = [1, 2, 3, 4, 5]
array1 = np.array(list1)
print(array1)
```
### Create a 2D array from a list of lists
```python
list2 = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
array2 = np.array(list2)
print(array2)
array6 = np.linspace(0, 1, 5)
print(array6)
```
### Create an array with values from 0 to 9
```python
array3 = np.arange(10)
print(array3)
```
### Create a 1D array of zeros
```python
array4 = np.zeros(5)
print(array4)
```
### Create a 2D array of ones
```python
array5 = np.ones((3, 3))
print(array5)
```

### Create an array with 5 values evenly spaced between 0 and 1
```python
array6 = np.linspace(0, 1, 5)
print(array6)
```

### Create a 3x3 identity matrix
```python
array7 = np.eye(3)
print(array7)
```

### Create a 1D array with 5 random values from a uniform distribution
```python
array8 = np.random.rand(5)
print(array8)
```
### Create a 2D array with random values from the standard normal distribution
```python
array9 = np.random.randn(3, 3)
print(array9)
```
### Create odd or even arrays
```python
evens = np.arange(2, 31, 2)
odds = np.arange(1, 31, 2)
print(evens)
print(odds)
```