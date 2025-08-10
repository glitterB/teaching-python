Imagine you would like to create tables of 2 in Python. We will type each number corresponding to tables of two.

```python
>>> 2
>>> 4
>>> 6
>>> ...
>>> 10
```
In python, data types include integer (`int`, ex. **2**), string (`str`, ex. **'2'** or **"2"**) and real number (**float**, ex. **2.0**).

>In `Python`, we can interchange one data type with another using in built function
>`int()`→ Converting to Integer <br>
>`float()` → Converting to floating point i.e. real number <br>
>`str()` → Converting to string or text


`Python` has in-built function `print()` to output these data types.

```python
print(2)
>>> 2
print(4)
>>> 4
```

But, why should we type each and every number every time using `print` function?. Instead we can use loops for repeative tasks.
Let's use `for` loop. For loop requires mainly 3 things, **starting number**, **ending number** and **increment**. By default, **increment** value is set to 1.
>Ending number should be 1 more than the desired, since `Python` excludes the actual ending number.

```python
for i in range(2,21,2):
    print(i)
```
✅ Output
```python
>>> 2
>>> 4
>>> 6
>>> 8
>>> 10
...
>>> 20
```
In above case, starting number is 2, ending number is 21 (since we want to end on 20) and increment is 2.

This prints tables of 2, and we didn't type `print()` every time.

But now if anyone wants to make tables of 5 or 6 or say 10, one needs to create `for` loop each time. 

Instead, we can write a `function` that takes some input and returns an output.
(In our case, it takes number and returns it's table).

```python
def table(n):
    for i in range(1, 11):
        print(f"{n} x {i} = {n*i}")

```
```python
#Let's call our function (calling a function means using it)
table(3)
```
✅ Output
```python
>>> 3 x 1 = 3
>>> 3 x 2 = 6
>>> 3 x 3 = 9
...
>>> 3 x 10 = 30
```
But, how to check correctness of the input? We can use `if` or `if...else` for conditionals, in order to check specific things while writting a program.

```python
def table(n):
    #Converting input 'n' to an Integer
    n = int(n)
    #Checking if n is less than 0
    if n <= 0:
        print("Please enter a positive number.")
        return
    
    for i in range(1, 11):
        print(f"{n} x {i} = {n*i}")
```


This time, let's take input form the user.

```python
n = int(input("Enter a number: "))
#Let's call our function
table(n)
```
✅ Output
```python
>>> Enter a number: 
>>> 3
>>> 3 x 1 = 3
>>> 3 x 2 = 6
>>> 3 x 3 = 9
...
>>> 3 x 10 = 30
```
>In python, user inputs are treated as strings.

We can make our program to run several times using `while` loop.

```python
while True:
    entry = input("Enter a number (or type 'exit' to quit): ")
    if entry.lower() == 'exit':
        break
    if entry.isdigit():
        table(int(entry))
    else:
        print("Please enter a valid number.")
```

Next, we well see data structures in python such as **lists** and **dictionaries**.

[Home