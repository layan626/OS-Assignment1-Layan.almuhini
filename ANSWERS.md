# Assignment Questions

## Instructions
Answer all 4 questions with detailed explanations. Each answer should be **3-5 sentences minimum** and demonstrate your understanding of the concepts.

---

## Question 1: Thread vs Process

**Question**: Explain the difference between a **thread** and a **process**. Why did we use threads in this assignment instead of creating separate processes?

**Your Answer:**

[A process is an independent program that has its own memory space, while a thread is a smaller unit of a process that shares memory with other threads. Threads are faster to create and communicate more efficiently compared to processes. In this assignment, we used threads because they are lightweight and suitable for simulating multiple processes running concurrently. Threads allow better performance when handling multiple tasks at the same time.]

---

## Question 2: Ready Queue Behavior

**Question**: In Round-Robin scheduling, what happens when a process doesn't finish within its time quantum? Explain using an example from your program output.

**Your Answer:**

[In Round-Robin scheduling, if a process does not finish within its time quantum, it is moved back to the ready queue. For example, a process like P1 may run for a short time and then get re-queued if it still has remaining time. This behavior ensures fairness because every process gets a chance to use the CPU. Without this, some processes might never get executed.]

Example from my output:
```
[Paste a relevant snippet from your program output here showing a process being re-queued]
```

**Explanation of example:**
[Explain what's happening in the output snippet you pasted]

---

## Question 3: Thread States

**Question**: A thread can be in different states: **New**, **Runnable**, **Running**, **Waiting**, **Terminated**. Walk through these states for one process (P1) from your simulation.

**Your Answer:**

[A thread starts in the new state when it is created. After calling Thread.start(), it moves to the runnable state and then to the running state when it gets CPU time. If the thread waits, it enters the waiting state, such as when Thread.sleep() is used. Finally, when the task is completed, the thread moves to the terminated state. In this assignment, we observed these states during process execution.]

1. **New**: [
P1 is in the New state when the thread object is created using "new Thread(process)" but before calling start(). At this point, the thread is not yet running.]

2. **Runnable**: [
P1 becomes Runnable after calling thread.start(). In this state, it is ready to run and waiting for the CPU to assign it execution time.]

3. **Running**: [
P1 is in the Running state when the CPU starts executing the run() method of the thread. During this time, the process is actively using the CPU for its time quantum.]

4. **Waiting**: [
P1 may enter the Waiting state when thread.join() is called, causing the main thread to wait until P1 finishes its execution. It can also conceptually wait in the ready queue before getting CPU time again.]

5. **Terminated**: [
P1 enters the Terminated state when it finishes execution completely and its remaining time becomes zero. At this point, the thread has completed its run() method and will not execute again.]

---

## Question 4: Real-World Applications

**Question**: Give **TWO** real-world examples where Round-Robin scheduling with threads would be useful. Explain why this scheduling algorithm works well for those scenarios.

**Your Answer:**

### Example 1: [Web Server]

**Description**: 
[
A web server handles multiple user requests at the same time. Each request can be processed using a separate thread.]

**Why Round-Robin works well here**: 
[Round-Robin ensures that each request gets a fair share of CPU time. It prevents one request from taking too long and blocking others, which improves responsiveness and user experience.]

### Example 2: [Operating System Process Scheduling]

**Description**: 
[An operating system manages multiple programs running at the same time, such as applications opened by the user.]

**Why Round-Robin works well here**: 
[Round-Robin scheduling allows each process to run for a short time quantum, ensuring fairness among all processes. It keeps the system responsive and prevents any single process from dominating the CPU.]

---

## Summary

**Key concepts I understood through these questions:**
1. The difference between threads and processes and how they work together.
2. How Round-Robin scheduling ensures fairness between processes.
3. The lifecycle of a thread from creation to termination.

**Concepts I need to study more:**
1. Thread synchronization and how to manage shared resources safely between multiple threads.
2. Advanced scheduling algorithms and how they differ from Round-Robin scheduling.
