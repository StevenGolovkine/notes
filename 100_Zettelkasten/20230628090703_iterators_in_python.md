
---
creation date: 2023-06-20 09:34
last updated: 2023-06-20 09:34
---
# [[20230620093441_iterators_in_python]] - Iterators and iterables in Python
__Tags__: #software-engineering #python

---
__Contents__:
Iteration is what happen when running a ``for`` or a ``while`` loop, it is the process. Iterator is going through the iteration process one item at a time. It can be created using generator expressions ([[20230628085312_generators_iterators_python]]).

Python implements the iterator design pattern. It basically goes through a container and access its elements. It is a class with two responsability: returning the data from a stream *one item at a time* and keeping track of the current and visited items.

The iterator protocol defines two special methods:
* ``__iter__()``: return the iterator object.
* ``__next__()``: iterate over the iterator, this should return the next item and raise a ``StopIteration`` exception at the end.
But it can be created by inheriting from the `ABC` called `Iterator`.

There are different types of iterators:
* Take a stream of data $\rightarrow$ return the data. The class has two attributes (sequence and index).
* Take a stream of data $\rightarrow$ transform the data $\rightarrow$ return the data. Do the modification of the data into the ``__next__()`` function.
* Take no data $\rightarrow$ generate data $\rightarrow$ return the data. The generation of the data has to be the `__next__()` function.

The main advantage of iterators is their memory efficience as there is no need to store all the data. It results to be more efficient than functions and list comprehensions. It is also the only way to define infinite data stream.

There are some drawbacks to iterators:
* can not iterate over an iterator more than once, the iterator is said _exhausted_;
* can not reset an exhausted iterator to start again;
* can not go back as it only defines the `__next__()` method;
* do not allow indexing and slicing operations.

Note that the built-in function `next()` has an optional argument for the default value to be returned when a `StopIteration` exception is raised.

__References__:

