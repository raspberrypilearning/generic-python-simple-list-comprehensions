- यदि आप Python का उपयोग करके एक सूची बनाना चाहते हैं, तो **for loop** का उपयोग करके यह करना काफी आसान है।

    ```python
    new_list = []
    for i in range(10):
        new_list.append(i)
    ```

    ```python
    >>> new_list
    [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
    ```


- यही सूची एक ही पंक्ति में बनाई जा सकती है ऐसे एक कंस्ट्रक्ट का उपयोग करके जो कई प्रोग्रामिंग भाषाओं में मौजूद होता है: एक **list comprehension**।

    ```python
    new_list = [i for i in range(10)]
    ```

    ```python
    >>> new_list
    [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
    ```
- आप किसी भी **iterable** का उपयोग कर सकते हैं एक list comprehension में, ताकि दूसरी सूची से एक सूची बनाना आसान हो।

    ```python
    numbers = [1, 2, 3, 4, 5]
    numbers_copy = [number for number in numbers]
    ```

    ```python
    >>> numbers_copy
    [1, 2, 3, 4, 5]
    ```

- आप एक list comprehension के भीतर गणना भी कर सकते हैं।

    ```python
    numbers = [1, 2, 3, 4, 5]
    double = [number * 2 for number in numbers]
    ```

    ```python
    >>> double
    [2, 4, 6, 8, 10]
    ```

- स्ट्रिंग ऑपरेशन भी किए जा सकते हैं।

    ```python
    verbs = ['shout', 'walk', 'see']
    present_participle = [word + 'ing' for word in verbs]
    ```

    ```python
    >>> present_participle
    ['shouting', 'walking', 'seeing']
    ```

- आप सूचियों का विस्तार भी आसानी से कर सकते हैं।

    ```python
    animals = ['cat', 'dog', 'fish']
    animals = animals + [animal.upper() for animal in animals]
    ```

    ```python
    >>> animals
    ['cat', 'dog', 'fish', 'CAT', 'DOG', 'FISH']    
    ```
	
