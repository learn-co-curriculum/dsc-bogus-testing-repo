# Creating Functions - Lab


```python
# this is a change
a = 1 + 10 + 3 + 4 + 5 + 6 + 7
b = 0 + 1 + 2 + 3 + 4 + 5 + 6 + 7 + 8 + 9 + 10 - 1
```

## Tracking changes made by the branch splitter via github actions after
* Pull Request Approval



```python
# The contents of this cell are to demonstrate the github actions functionality on the solution branch

this_is_a_list = None
a_dict = None


def afunction():
    pass
```


```python
# __SOLUTION__
# The contents of this cell are to demonstrate the github actions functionality on the solution branch

this_is_a_list = [1, 2, 3, 4, "fun"]
a_dict = {"yes": "llama", "double quotes or single?": "single"}


def afunction():
    return 100**2
```

## Introduction

As you know, we can use functions to name snippets of our code, thus making our code more expressive. We can also use functions to allow us to reuse our code. In this lab we will practice using functions for both of those purposes.

## Objectives

You will be able to:

* Declare and use a basic function

## Instructions: 
### Writing our first functions

Imagine we are creating a list of travel destinations -- which can really turn out to be a full time job if we like to travel. We have our list of `travel_destinations` which we assign below. Write a function called `number_of_destinations()` that returns the number of destinations we have on our list.


```python
travel_destinations = ["argentina", "mexico", "italy", "finland", "canada", "croatia"]
# define function here
```


```python
# __SOLUTION__
travel_destinations = ["argentina", "mexico", "italy", "finland", "canada", "croatia"]


# define function here
def number_of_destinations():
    return len(travel_destinations)
```

> Below, remove the first `#` to uncomment the following line(s) of code and then press `shift` + `enter` to run the cell


```python
# number_of_destinations() # Expected output: 6
```


```python
# __SOLUTION__
number_of_destinations()
```




    6



Now write another function called `next_up()` that returns our first destination (the destination with the lowest index), in the `list_of_destinations` list.


```python
# define function here
```


```python
# __SOLUTION__
# define function hed
def next_up():
    return list_of_destinations[0]
```

Next, run your new function


```python
list_of_destinations = ["argentina", "canada", "croatia"]
# Your code here
# Expected output:'argentina'
```


```python
# __SOLUTION__
list_of_destinations = ["argentina", "canada", "croatia"]
next_up()
```




    'argentina'



Ok, now write a function called `favorite_destination()` that returns the string `'madagascar'`.


```python
# define function here
```


```python
# __SOLUTION__
# define function here
def favorite_destination():
    return "madagascar"
```

Next, run your new function


```python
# Your code here
# Expected output:'madagascar'
```


```python
# __SOLUTION__
favorite_destination()
```




    'madagascar'



Again, let's declare a list called `favorite_destinations`. Write a new function called `add_favorite_destination()` that adds the string `'madagascar'` to the end of `favorite_destinations` and also returns the string `'madagascar'`.


```python
# define function here
```


```python
# __SOLUTION__
# define function here
def add_favorite_destination():
    favorite_destinations.append(favorite_destination())
    return favorite_destination()
```

Next, run your new function


```python
favorite_destinations = ["argentina", "mexico", "italy", "finland", "canada", "croatia"]

# Your code here

favorite_destinations[-1]
```


```python
# __SOLUTION__
favorite_destinations = ["argentina", "mexico", "italy", "finland", "canada", "croatia"]

add_favorite_destination()

favorite_destinations[-1]  # 'madagascar'
```




    'madagascar'



Now let's write another function called `capitalize_countries()` which iterates through the list of `capitalized_destinations` and capitalizes the first letter of each word. It should return a list of capitalized destinations.


```python
capitalized_destinations = [
    "argentina",
    "mexico",
    "italy",
    "finland",
    "canada",
    "croatia",
]
# define function here
```


```python
# __SOLUTION__
capitalized_destinations = [
    "argentina",
    "mexico",
    "italy",
    "finland",
    "canada",
    "croatia",
]


# define function here
def capitalize_countries():
    new_list = []
    for country in capitalized_destinations:
        new_list.append(country.capitalize())
    return new_list
```

Next, run your new function


```python
# Your code here # ['Argentina', 'Mexico', 'Italy', 'Finland', 'Canada', 'Croatia']
```


```python
# __SOLUTION__
capitalize_countries()
```




    ['Argentina', 'Mexico', 'Italy', 'Finland', 'Canada', 'Croatia']



Great! Now if someone adds a country that is lowercased to our list of destinations, we can simply call our function again to capitalize each of the destinations in the list.

## Summary

Great job! In this lab we were able to get practice both creating and returning values from functions.
