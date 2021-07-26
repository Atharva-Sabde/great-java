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

1. Process Based Multitasking
process based multitasking is best suitable at OS level.
2. Thread Based Multitasking

    Executing several tasks simultaneously where each task is separate independent part of a single program, and each part is called a thread.

    Best suitable at Programmatic  level.

What is Thread? :  a part of a huge program 

Main method is executed by main thread.

If the code has dependency ,then do not use multithreading.
