
---
creation date: 2023-06-28 09:12
last updated: 2023-06-28 09:12
---
# [[20230628091242_asynchronous_iterators_in_python]] - Asynchronous Iterators in Python
__Tags__: #software-engineering #python #concurrency

---
__Contents__: The asynchronous iterators protocol is the same as iterators protocoll with the methods `__aiter__()` and `__anext__()`. The `__anext__()` function must raise a `StopAsyncIteration` exception and be defined with the `async def` keyword.

Note that the asynchronous iterators are *not* run in parallel ([[20230628091627_concurrency_in_python]]).

__References__:



