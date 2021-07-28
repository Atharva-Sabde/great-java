# MultiThreading in Java
<hr>
<hr>






<details>
<summary>=============    CONTENTS    =============</summary>
<br> <br>
1. Introduction

2. The ways to define, instantiate and start a new Thread.

1. By extending Thread class
2.  By implementing Runnable interface
1. Thread class Constructors
2. Thread Prioirity
3. Getting and Setting name of a thread
4. The methods to Stop Thread Execution
    1. yield()
    2. join()
    3. sleep()
5. Synchronization
6. Inter Thread Communication
7. Deadlock
8. Daemon Threads.
9. Various Conclusions
    1. To stop a thread
    2. Suspend & resume a thread
    3. Thread group
    4. Green Thread
    5. Thread local
10. Lifecycle of Thread.
</details>


## Introduction:

Multitasking: why? To increase the efficiency and reduce idle time to improve performance.

Reduce response time of the system.


- Process Based Multitasking
    - Typing code , listening to music , and downloading content at the same time also resembles multitasking but it comes under process based multitasking because all the tasks are independent of each other but executing simultaneously.
    - Best suitable at OS level.
- Thread Based Multitasking
    - Executing several tasks simultaneously where each task is separate independent part of a single program, where, each part is called a thread.
    - Best suitable at Programmatic  level.

Whether it is Process based or Thread based the main objective of multitasking is to improve performance of the system by reducing response time.
 
<hr>

What is Thread? :  A small discrete part of a large program.

- Java provides in built support for multithreading through a rich
API (Thread, Runnable, ThreadGroup, ThreadLocal...etc).
- In multithreading on 10% of the work the programmer is required to do and
90% of the work will be down by java API.
- Main method is executed by main thread.
- Execution of threads can be mixed depending on system and each run.
- Applications include : Multimedia graphics , Games , animations , application-servers.

If the code has dependency ,then do not use multithreading.
