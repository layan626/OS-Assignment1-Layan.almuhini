# Development Log

## Instructions
Document your development process as you work on the assignment. Add entries showing:
- What you worked on
- Problems you encountered
- How you solved them
- Time spent

**Requirements**: Minimum 5 entries showing progression over time.

---

## Example Entry Format:

### Entry 1 - [April 1, 2026, 2:30 PM]
**What I did**: Forked the repository and set up my student ID

**Details**: 
- Created GitHub account with university email
- Forked the starter repository
- Changed student ID on line 92 to my actual ID (441234567)
- Compiled and ran the program successfully

**Challenges**: Had to install JDK first because javac wasn't recognized

**Solution**: Downloaded JDK 17 from Oracle website and set PATH variable

**Time spent**: 30 minutes

---

## Your Development Log:

### Entry 1 - [27 March 2026]
**What I did**: 
Set up my development environment and connected GitHub with my IDE.

**Details**: I opened the project in Visual Studio Code, installed the required extensions, and signed in to my GitHub account to access my repository.

**Challenges**: 
I had some difficulty linking my GitHub account with the IDE and understanding how to manage the repository locally.

**Solution**: I followed online tutorials and used the built-in GitHub sign-in feature in VS Code until the connection was successful.

**Time spent**: 25 minutes

---

### Entry 2 - [28 March 2026]
**What I did**: 
Forked the starter repository and created my own copy.

**Details**: I accessed the provided GitHub link and used the fork option to create a personal copy of the repository under my account.

**Challenges**: 
At first, I was confused about the difference between forking and cloning.

**Solution**: I reviewed the instructions again and understood that forking creates a copy in my account, which I can modify.

**Time spent**: 20 minutes

---

### Entry 3 - [29 March 2026]
**What I did**: 
Renamed the repository and added my student ID to the code.

**Details**: 
I changed the repository name according to the required format and edited the SchedulerSimulation.java file to include my student ID.

**Challenges**: 
I had difficulty finding the correct place to update the student ID in the code.

**Solution**: 
I carefully searched the file and followed the assignment instructions to locate the correct line.

**Time spent**: 25 minutes

---

### Entry 4 - [ 30 March 2026]
**What I did**: 
Implemented the priority feature in the Process class.

**Details**: 
I added a priority variable to the Process class and updated the constructor to accept and assign this value.

**Challenges**: 
I was unsure where to define the priority and how to pass it correctly.

**Solution**: 
I added the variable inside the class and generated a random value in the main method before creating each process.

**Time spent**: 40 minutes

---

### Entry 5 - [Date and Time]
**What I did**:
Implemented context switch counter and waiting time tracking. 

**Details**: 
I added a static counter to track context switches and implemented waiting time calculation using system time functions.

**Challenges**: 
It was difficult to understand where to increment the counter and how to calculate waiting time correctly.

**Solution**: 
I placed the counter before starting each thread and used System.currentTimeMillis() to track waiting time accurately.

**Time spent**: 40 minutes

---

### Entry 6 - [Optional - Date and Time]
**What I did**: 

**Details**: 

**Challenges**: 

**Solution**: 

**Time spent**: 

---

## Summary

**Total time spent on assignment**: [2.5 hours]

**Most challenging part**: 
The most challenging part was implementing the waiting time feature because it required understanding how to track time accurately and determine the correct place in the code to calculate it.

**Most interesting learning**: The most interesting part was learning how threads work in Java and how the Round-Robin scheduling algorithm manages multiple processes efficiently.

**What I would do differently next time**: 
I would start earlier and make commits more frequently to avoid losing any progress and to manage my work more efficiently.
