# Creating Functions - Lab

## Added action version

Added extended version number for the action

> # Remote Action Testing again!! (wrong script name before)

## added updated version for the remote action
> This cell is put here to track and test tooling changes.

## added the "on: workflow_call arg

This update to this cell is for testing if the remote action works when pushed from your local machine.

## Testing remote action change of path

## Introduction

As you know, we can use functions to name snippets of our code, thus making our code more expressive. We can also use functions to allow us to reuse our code. In this lab we will practice using functions for both of those purposes.

## Objectives

You will be able to:

* Declare and use a basic function

# Testing Github Actions
This cell is to track changes automatically synced with github actions

After many tests, I have the action working beautifully!

Testing changes

More changes

splitter moved.

## Instructions: 
### Writing our first functions

Imagine we are creating a list of travel destinations -- which can really turn out to be a full time job if we like to travel. We have our list of `travel_destinations` which we assign below. Write a function called `number_of_destinations()` that returns the number of destinations we have on our list.


```python
travel_destinations = ['argentina', 'mexico', 'italy', 'finland', 'canada', 'croatia']
# define function here
```

> Below, remove the first `#` to uncomment the following line(s) of code and then press `shift` + `enter` to run the cell


```python
# number_of_destinations() # Expected output: 6
```

Now write another function called `next_up()` that returns our first destination (the destination with the lowest index), in the `list_of_destinations` list.


```python
# define function here
```

Next, run your new function


```python
list_of_destinations = ['argentina', 'canada', 'croatia']
# Your code here 
# Expected output:'argentina'
```

Ok, now write a function called `favorite_destination()` that returns the string `'madagascar'`.


```python
# define function here
```

Next, run your new function


```python
# Your code here 
# Expected output:'madagascar'
```

Again, let's declare a list called `favorite_destinations`. Write a new function called `add_favorite_destination()` that adds the string `'madagascar'` to the end of `favorite_destinations` and also returns the string `'madagascar'`.


```python
# define function here
```

Next, run your new function


```python
favorite_destinations = ['argentina', 'mexico', 'italy', 'finland', 'canada', 'croatia']

# Your code here 

favorite_destinations[-1] 
```

Now let's write another function called `capitalize_countries()` which iterates through the list of `capitalized_destinations` and capitalizes the first letter of each word. It should return a list of capitalized destinations.


```python
capitalized_destinations = ['argentina', 'mexico', 'italy', 'finland', 'canada', 'croatia']
# define function here
```

Next, run your new function


```python
# Your code here # ['Argentina', 'Mexico', 'Italy', 'Finland', 'Canada', 'Croatia']
```

Great! Now if someone adds a country that is lowercased to our list of destinations, we can simply call our function again to capitalize each of the destinations in the list.

## Summary

Great job! In this lab we were able to get practice both creating and returning values from functions.
