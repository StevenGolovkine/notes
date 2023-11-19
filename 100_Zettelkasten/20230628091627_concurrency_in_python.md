
---
creation date: 2023-06-28 09:16
last updated: 2023-06-28 09:16
---
# [[20230628091627_concurrency_in_python]] - Concurrency in Python
__Tags__: #python #concurrency 

---
__Contents__: Concurrency stands for simultaneous occurence. In Python, it is a sequence of instructions that run in order (thread, task, process). It could be of three types:
* Process (`multiprocessing`, run at the same time), creates new processes that run on a different Python interpreter and that can be run on different cores.
* Task (`asyncio`, run one at a time), cooperate by announcing when they are ready to be switched out (cooperative multitasking).
* Thread (`threading`, run on at a time), OS knows about each thread and can interupt them at any time to start running a different thread (pre-emptive multitasking).

Concurrency is useful for two types of problems:
* CPU-bounded problems ([[20230628092500_cpu_bounded_problems_in_python]])
* I/O bounded problems ([[20230628092436_io_bounded_problem_in_python]])

When to use concurrency? Wait until a know performance issue appears to consider concurrency. Then, determine if it is an I/O or CPU bounded problem to choose which concurrency method to use. If it is a I/O problem, "use `asyncio` when you can and `threading` when you must".

__References__:



