# Implementing a critical section on the STM32

An led is treated as the shared resource here.Two threads of equal priority try to acquire access to the led.However,led access is protected using a semaphore.Therefore,thread1 gets access while thread 2 is forced to wait.After t1 releases the semaphore,t2 gets access and the process repeats.The threads are scheduled using round robin scheduling.

This can be seen using Keil's event viewer and thread viewer


![Alt text](https://github.com/amateurcoder10/stmcriticaloverview.png?raw=true "Optional Title")
