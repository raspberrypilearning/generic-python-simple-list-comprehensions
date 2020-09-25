- Si quieres crear una lista con Python, es bastante fácil hacerlo con un **bucle for**.

    ```python
    nueva_lista = []
    for i in range(10):
        nueva_lista.append(i)
    ```

    ```python
    >>> nueva_lista
    [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
    ```


- La misma lista se puede crear en una línea simple al usar una construcción que ya existe en muchos lenguajes de programación: la **comprensión de lista**.

    ```python
    nueva_lista = [i for i in range(10)]
    ```

    ```python
    >>> nueva_lista
    [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
    ```
- Usa cualquier **iterable** en la comprensión de lista, es fácil crear listas de otras listas.

    ```python
    numeros = [1, 2, 3, 4, 5]
    copiar_numeros = [numero for numero in numeros]
    ```

    ```python
    >>> copiar_numeros
    [1, 2, 3, 4, 5]
    ```

- También puedes hacer cálculos dentro de una comprensión de lista.

    ```python
    numeros = [1, 2, 3, 4, 5]
    doble = [numero * 2 for numero in numeros]
    ```

    ```python
    >>> doble
    [2, 4, 6, 8, 10]
    ```

- Las operaciones de cadenas de carácteres también se pueden hacer.

    ```python
    verbos = ['shout', 'walk', 'see']
    participio_presente = [palabra + 'ing' for palabra in verbos]
    ```

    ```python
    >>> participio_presente
    ['shouting', 'walking', 'seeing']
    ```

- Es posible extender las listas con bastante facilidad.

    ```python
    animales = ['gato', 'perro', 'pez']
    animales = animales + [animal.upper() for animal in animales]
    ```

    ```python
    >>> animales
    ['gato', 'perro', 'pez', 'GATO', 'PERRO', 'PEZ']    
    ```
	
