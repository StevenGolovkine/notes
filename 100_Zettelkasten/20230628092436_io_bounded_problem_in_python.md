
---
creation date: 2023-06-28 09:24
last updated: 2023-06-28 09:24
---
# [[20230628092436_io_bounded_problem_in_python]] - I/O bounded problems in Python
__Tags__: #python #concurrency 

---
__Contents__: The program has to wait for external ressources like file system and network connection. The three types of concurrency can be used to deal with it.

* Threading: use `ThreadPoolExecutor` to create and control a pool of threads. The `map()` method is used to delegate work to each thread. Each thread needs its own `requests.Session` object. The data sharing between threads is not easy and has to be protected.
* Asyncio: event loop controls how and when each task gets run. Tasks can be in multiple states (but one at a time), e.g. ready and wait. Tasks never give up control without intentionally doing so, data sharing is easier than for the Threading method. Two methods are needed: `await`, that allows the task to hand control back to the event loop and `async`, that flag to Python telling it that the function must await.
* Multiprocessing: ran code across multiple CPUs. Some time is lost when creating new processes (created using `multiprocessing.Pool()`). It needs some thinking about which variables can be accessed in each process.



__References__:



