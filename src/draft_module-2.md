## Draft

Now that we have covered the basics of Python. Let's take it from there.

In Python, there are certain data structures such as `tuples`, `lists`, `dictionaries`, `set`, etc.

```python
>>> tuple_example = (1,2,3,4,5) #stores in ()
>>> list_example = [1,2,3,4,5] #stores in []
>>> set_example = {1,2,3,4,5} #stores in {}
>>> dict_example = {1:[1,2,3,4,5],2:[2,4,6,8,10]} #holds a key:value relation
```
Let's write a program to store tables of 5 in a list.
To add data in a list, we use `.append()` method.

```python
n = 5
tables_of_five = [] #an empty list
for i in range(n, n*10+1, n):
    tables_of_five.append(i)
```

Now to access those values stored in that list, we use indexing. Indext starts from 0.

[Home](..\readme.md)