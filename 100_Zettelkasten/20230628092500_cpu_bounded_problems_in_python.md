
---
creation date: 2023-06-28 09:25
last updated: 2023-06-28 09:25
---
# [[20230628092500_cpu_bounded_problems_in_python]] - CPU bounded problems in Python
__Tags__: #python #concurrency 

---
__Contents__: The program mostly do CPU operations. The problem is roughly how fast the data can be processed. 

Thread and tasks are not useful in this context, because they run on a unique core.
Usually, multiprocessing is an answer to that problem but it can sometime be difficult to split the problem to be run on different cores.


__References__:



