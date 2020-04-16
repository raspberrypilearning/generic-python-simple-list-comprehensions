- Als je een lijst wilt genereren met Python, is het vrij eenvoudig om dit te doen met een **for lus**.

    ```python
    nieuwe_lijst = []
for i in range(10):
    nieuwe_lijst.append(i)
    ```

    ```python
    >>> nieuwe_lijst
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
    ```


- Dezelfde lijst kan op één regel worden gemaakt met behulp van een constructie die in veel programmeertalen bestaat: een **list comprehension (lijstsamenstelling)**.

    ```python
    nieuwe_lijst = [i for i in range(10)]
    ```

    ```python
    >>> nieuwe_lijst
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
    ```
- Je kunt elke **iterable (herhaalbare)** in een lijstsamenstelling gebruiken, dus het is gemakkelijk om een lijst uit een andere lijst te maken.

    ```python
    getallen = [1, 2, 3, 4, 5]
getallen_kopie = [getal for getal in getallen]
    ```

    ```python
    >>> getallen_kopie
[1, 2, 3, 4, 5]
    ```

- Je kunt ook berekeningen uitvoeren binnen een lijstsamenstelling.

    ```python
    getallen = [1, 2, 3, 4, 5]
dubbel = [getal * 2 for getal in getallen]
    ```

    ```python
    >>> dubbel
[2, 4, 6, 8, 10]
    ```

- Stringbewerkingen kunnen ook worden uitgevoerd.

    ```python
    werkwoorden = ['roepen', 'lopen', 'kijken']
onvoltooid_deelwoorden = [woord + 'd' for woord in werkwoorden]
    ```

    ```python
    >>> onvoltooide_deelwoorden
['roepend', 'lopend', 'kijkend']
    ```

- Je kunt lijsten ook vrij gemakkelijk uitbreiden.

    ```python
    dieren = ['kat', 'hond', 'vis']
dieren = dieren + [dier.upper() for dier in dieren]
    ```

    ```python
    >>> dieren
['kat', 'hond', 'vis', 'KAT', 'HOND', 'VIS']    
    ```
	
