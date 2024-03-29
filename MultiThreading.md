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

![image](https://user-images.githubusercontent.com/67774570/127376494-68ee363d-4360-4eb3-b7e7-8d1ae3db5792.png)



## The ways to define, instantiate and start a new Thread:

1. Extending Thread Class
2. Implementing Runnable Interface

### Best approach to define a Thread:

- Among the 2 ways of defining a Thread, implements Runnable approach is
always recommended.
- In the 1st approach our class should always extends Thread class there is no
chance of extending any other class hence we are missing the benefits of
inheritance.
- But in the 2nd approach while implementing Runnable interface we can extend
some other class also. Hence implements Runnable mechanism is recommended
to define a Thread.
