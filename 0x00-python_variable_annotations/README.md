# 0x00. Python - Variable Annotations

![python-3-documentation](https://i.redd.it/y9y25tefi5401.png)

## Learning Objectives

## General

At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

* Type annotations in Python 3
* How you can use type annotations to specify function signatures and variable types
* Duck typing
* How to validate your code with mypy
* Tasks :page_with_curl:

* **0. Basic annotations - add**
  * [0-add.py](./0-add.py): Write a type-annotated function add that takes a float a and a float b as arguments and returns their sum as a float.

* **1. Basic annotations - concat**
  * [1-concat.py](./1-concat.py): Write a type-annotated function concat that takes a string str1 and a string str2 as arguments and returns a concatenated string

* **2. Basic annotations - floor**
  * [2-floor.py](./2-floor.py): Write a type-annotated function floor which takes a float n as argument and returns the floor of the float.

* **3. Basic annotations - to string**
  * [3-to_str.py](./3-to_str.py): Write a type-annotated function to_str that takes a float n as argument and returns the string representation of the float.

* **4. Define variables**
  * [4-define_variables.py](./4-define_variables.py): Define and annotate the following variables with the specified values:

    * a, an integer with a value of 1
    * pi, a float with a value of 3.14
    * i_understand_annotations, a boolean with a value of True
    * school, a string with a value of “Holberton”

* **5. Complex types - list of floats**
  * [5-sum_list.py](./5-sum_list.py):Write a type-annotated function sum_list which takes a list input_list of floats as argument and returns their sum as a float.

* **6. Complex types - mixed list**
  * [6-sum_mixed_list.py](./6-sum_mixed_list.py):Write a type-annotated function sum_mixed_list which takes a list mxd_lst of integers and floats and returns their sum as a float.
  
* **7. Complex types - string and int/float to tuple**
  * [7-to_kv.py](./7-to_kv.py): Write a type-annotated function to_kv that takes a string k and an int OR float v as arguments and returns a tuple. The first element of the tuple is the string k. The second element is the square of the int/float v and should be annotated as a float.

* **8. Complex types - functions**
  * [8-make_multiplier.py](./8-make_multiplier.py): Write a type-annotated function make_multiplier that takes a float multiplier as argument and returns a function that multiplies a float by multiplier.

* **9. Let's duck type an iterable object**
  * [9-element_length.py](./9-element_length.py): Annotate the below function’s parameters and return values with the appropriate types

    ````markdown
    ```
    def element_length(lst):
        return [(i, len(i)) for i in lst]
    ```
    ````

* **10. Duck typing - first element of a sequence**
  * [100-safe_first_element.py](./100-safe_first_element.py): Augment the following code with the correct duck-typed annotations:

    ````markdown
    ```
    # The types of the elements of the input are not know
    def safe_first_element(lst):
        if lst:
            return lst[0]
        else:
            return None
    ```
    ````

* **11. More involved type annotations**
  * [101-safely_get_value.py](./101-safely_get_value.py):Given the parameters and the return values, add type annotations to the function

Hint: look into TypeVar
    ````markdown
    ```
    def safely_get_value(dct, key, default = None):
        if key in dct:
            return dct[key]
        else:
            return default
    ```
    ````

* **12. Type Checking**

  * [102-type_checking.py](./102-type_checking.py): Use mypy to validate the following piece of code and apply any necessary changes.

    ````markdown
    ```
    def zoom_array(lst: Tuple, factor: int = 2) -> Tuple:
        zoomed_in: Tuple = [
            item for item in lst
            for i in range(factor)
        ]
        return zoomed_in


    array = [12, 72, 91]

    zoom_2x = zoom_array(array)

    zoom_3x = zoom_array(array, 3.0)
    ```
    ````

## Authors &copy;

* Thami Baladi
