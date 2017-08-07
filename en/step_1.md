- If you want to generate a list using Python, it is quite easy to do so using a `for ` loop.

	```python
	new_list = []
	for i in range(10):
		new_list.append(i)
	```
	
	```python
	>>> new_list
	[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
	```


- The same list can be created in a single line using a construct that is common in many programming languages, called a list comprehension.

	```python
	new_list = [i for i in range(10)]
	```

	```python
	>>> new_list
	[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
	```
- You can use any **iterable** in a list comprehension, so making a list from another list is easy.

	```python
	numbers = [1, 2, 3, 4, 5]
	numbers_copy = [number for number in numbers]
	```
	
	```python
	>>> numbers_copy
	[1, 2, 3, 4, 5]
	```

- You can also do calculations within a list comprehension.

	```python
	numbers = [1, 2, 3, 4, 5]
	double = [number * 2 for number in numbers]
	```
	
	```python
	>>> double
	[2, 4, 6, 8, 10]
	```

- And string operations can also be done as well.

    ```python
	verbs = ['shout', 'walk', 'see']
	present_participle = [word + 'ing' for word in verbs]
	```
	
	```python
	>>> present_participle
	['shouting', 'walking', 'seeing']
	```
	
- You can also extend lists quite easily.

	```python
	present participleanimals = ['cat', 'dog', 'fish']
	animals = animals + [animal.upper() for animal in animals]
	```
	
	```python
	>>> animals
	['cat', 'dog', 'fish', 'CAT', 'DOG', 'FISH']	
	```
	
