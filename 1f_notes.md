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

