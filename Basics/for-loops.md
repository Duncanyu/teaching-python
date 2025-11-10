# -- For Loops --
## What Are They?
### Introduction
__For loops__ are similar to Scratch's repeat for x times, where x is an integer > 0

Essentially loops that repeat **for** x times, where x is an integer > 0

**HOWEVER:** One thing to note is that, traditional __for loops__ in Python do not take an integer as a parameter
- Instead, __for loops__ take ```lists```
    - ```lists``` are a new data/variable type
    - Instead of holding one value, like a ```string``` or an ```integer```, ```lists``` instead hold a **list** of values, ranging from ```strings```, to ```integers```, to ```floats```, to a mix of everything (```str``` + ```int``` + ```float``` etc..)
    - We won't be going too much into detail on ```lists``` this week/today, however, just know that they are created like any variable
        - ```variable_name = ["string", 8, 8.0, True, "string2"]```
- __For loops__ iterate through *elements* of a ```list```, where *element* is each item in that **list**.
    - For example, when I create a __for loop__ that takes the **list** ```variable_name``` as defined above:
        - Each iteration, it holds the value of the iteration number's location in the list:
        1. ```"string"```
        2. ```8```
        3. ```8.0```
        4. ```True```
        5. ```"string2"```
- Now comes one of the more useful parts of a __for loop__, the ```iterating variable```.
    - ```iterating variables``` are essentially **temporary variables** that we define when initializing the __for loop__, as shown in the example below:
        ```for x in range(5):```\
               ^ ```x``` is our ```iterating variable```
        - ```range(5)``` produces a list ranging from 0 to 4. **IMPORTANT:** When indexing a ```list```, index being the *location* we are at in the ```list```, the first *element* is considered **number 0**, then moving on, 1, 2, 3, where the last is the **length of the list - 1**
            - What are the indexes for each *element* in this list?\
                [1, 2, "three", 4, "five", True, 7]\
                0, 1, 2, 3, 4, 5, 6
        - ```x``` is the value of the current index. The index will increase by one after each iteration:
            [0, 1, 2, 3, 4]
            1. index = 0, x = list[0] = 0
            2. index = 1, x = list[1] = 1
            3. ... so on
        - With this new knowledge, a new *error type* appears, the ```index error```, which occurs when the index requested/mentioned does not exist within the ```list```.\
            [0, 1, 2, 3, 4, 5]\
            list[5] = 5\
            list[6] returns index error as the 7th element of the ```list``` does not exist; remember, **indexes start from 0 and go up to length - 1***
- Parts of a __for loop__:
    ```for x in range(5):```\
          ```print(x)```
    - Our designator is ```for```, which defines the __for loop__
    - We then follow with the ```iterating variable```, where we can name it anything: ```x```, ```_```, ```iterating_variable```, ```banana``` are all valid ```iterating variables```
    - After the ```iterating variable```, we put ```in```, which points to our ```list```
    - ```range(i)``` is a ```function``` that returns a ```list``` ranging from 0 to i - 1.
    - We then finish the __for loop__ off with a ```:```, and a ```new line``` that is *indented* once to show that we are 'in' the __for loop__
        - In here, we write our code.
        - We can reference the ```iterating variable``` **ONLY INSIDE THE** __for loop__, however, it is not mandatory to do so.
- You try!
    - Create your own ```list``` of daily food objects that you eat.
    - Create a __for loop__ to iterate through and ```print``` each food object that you listed.
    - Create a __for loop__ to ask the user *5 times* for their age.
    - Create a guessing game using __for loops__ and __if statements__, such that the player only gets *3 attempts* each for *5 questions*.
        - **Hint:** the ```break``` statement is used within any __loop__ (__for__, __while__) and *breaks* out of said __loop__. Example:
            - ```for x in range(5):```\
                    ```if x == 3:```\
                        ```break```\
                    ```else:```\
                        ```print(x)```
            - This only prints numbers up to 2, despite the range being up to 4.

## Things Covered:
1. __For loops__
2. ```lists```
3. Indexes
4. ```range(i)```
5. ```break```
