# Operating Systems Laboratory

## CS25C11 - Operating Systems Laboratory

This repository contains the programs and practical implementations for the **Operating Systems Laboratory**.

**Course:** CS25C11 - Operating Systems Laboratory  
**Program:** B.E. Computer Science and Engineering (AI & ML)  
**Regulation:** Anna University - Regulation 2025  
**Language:** C  
**Platform:** UNIX / Linux

---

## 📚 Experiments

| No. | Experiment |
|---|---|
| 1 | Basic UNIX Commands |
| 2 | Implementation of `fork()`, `exec()` and `wait()` System Calls |
| 3 | File Copy using `open()`, `read()` and `write()` System Calls |
| 4 | CPU Scheduling - First Come First Serve (FCFS) |
| 5 | CPU Scheduling - Shortest Job First (SJF), Non-Preemptive |
| 6 | CPU Scheduling - Round Robin |
| 7 | CPU Scheduling - Priority Scheduling (Non-Preemptive) |
| 8 | Process Synchronization - Producer-Consumer Problem using Semaphores |
| 9 | Process Synchronization - Dining Philosophers Problem using Semaphores |
| 10 | Deadlock Avoidance - Banker's Algorithm |
| 11 | Memory Management - Contiguous Allocation (First Fit, Best Fit, Worst Fit) |
| 12 | Memory Management - Page Replacement Algorithms (FIFO, LRU, Optimal) |
| 13 | Disk Scheduling Algorithms (SSTF, SCAN, C-SCAN) |

---

## 🧪 Experiment Details

### 1. Basic UNIX Commands

Study and practice basic UNIX commands for:

- Directory navigation
- File creation and manipulation
- File permissions
- Searching and viewing files

Commands covered include:

```bash
pwd
ls
cd
mkdir
rmdir
touch
cat
cp
mv
rm
head
tail
wc
grep
chmod
chown
```

---

### 2. fork(), exec() and wait()

Demonstrates:

- Process creation using `fork()`
- Replacing a process image using `exec()`
- Parent-child process synchronization using `wait()`

---

### 3. File Copy using System Calls

Copies the contents of one file to another using low-level UNIX system calls:

```text
open()
read()
write()
close()
```

---

## ⚙️ CPU Scheduling Algorithms

### 4. First Come First Serve (FCFS)

Simulates FCFS scheduling and calculates:

- Waiting Time
- Turnaround Time
- Average Waiting Time
- Average Turnaround Time

### 5. Shortest Job First (SJF)

Implements **Non-Preemptive SJF** scheduling.

The process with the shortest burst time among the arrived processes is selected.

### 6. Round Robin

Implements Round Robin CPU scheduling using a specified **Time Quantum**.

Calculates:

- Waiting Time
- Turnaround Time
- Average Waiting Time
- Average Turnaround Time

### 7. Priority Scheduling

Implements **Non-Preemptive Priority Scheduling**.

In this implementation, a smaller priority number represents a higher priority.

---

## 🔄 Process Synchronization

### 8. Producer-Consumer Problem

Implements the bounded-buffer Producer-Consumer problem using:

- POSIX Threads
- Semaphores
- Mutex

Compile using:

```bash
gcc producer_consumer.c -o producer_consumer -lpthread
```

Run:

```bash
./producer_consumer
```

### 9. Dining Philosophers Problem

Implements the Dining Philosophers problem using:

- POSIX Threads
- Semaphores
- Counting semaphore

The program uses a `room` semaphore to allow at most `N-1` philosophers to attempt to pick up forks, preventing circular wait.

Compile:

```bash
gcc dining_philosophers.c -o dining_philosophers -lpthread
```

Run:

```bash
./dining_philosophers
```

---

## 🔐 Deadlock

### 10. Banker's Algorithm

Implements the **Banker's Algorithm** for deadlock avoidance.

The program:

- Calculates the Need matrix
- Checks whether the system is in a safe state
- Displays the safe sequence
- Processes resource requests
- Grants a request only when the resulting state remains safe

---

## 🧠 Memory Management

### 11. Contiguous Memory Allocation

Implements three memory allocation strategies:

- First Fit
- Best Fit
- Worst Fit

The program displays the block allocated to each process.

### 12. Page Replacement Algorithms

Implements:

- FIFO
- LRU
- Optimal

The program calculates the number of page faults and displays the frame contents during execution.

---

## 💾 Disk Scheduling

### 13. Disk Scheduling Algorithms

Implements the following disk scheduling techniques:

- SSTF - Shortest Seek Time First
- SCAN
- C-SCAN - Circular SCAN

The algorithms are used to study disk head movement and scheduling.

---

## 🛠️ Requirements

To run the programs, the following are recommended:

- Linux / UNIX-based operating system
- GCC Compiler
- POSIX Threads support for synchronization programs
- Basic knowledge of C programming

Check GCC installation:

```bash
gcc --version
```

---

## ▶️ How to Run

Clone the repository:

```bash
git clone <YOUR-REPOSITORY-URL>
```

Move into the project directory:

```bash
cd <REPOSITORY-NAME>
```

Compile a C program:

```bash
gcc filename.c -o filename
```

Run the program:

```bash
./filename
```

For programs using POSIX Threads:

```bash
gcc filename.c -o filename -lpthread
./filename
```

---

## 📁 Suggested Repository Structure

```text
Operating-Systems-Lab/
│
├── README.md
│
├── Experiment-01-UNIX-Commands/
│   └── commands.txt
│
├── Experiment-02-fork-exec-wait/
│   └── fork_exec_wait.c
│
├── Experiment-03-File-Copy/
│   └── file_copy.c
│
├── Experiment-04-FCFS/
│   └── fcfs.c
│
├── Experiment-05-SJF/
│   └── sjf.c
│
├── Experiment-06-Round-Robin/
│   └── round_robin.c
│
├── Experiment-07-Priority-Scheduling/
│   └── priority.c
│
├── Experiment-08-Producer-Consumer/
│   └── producer_consumer.c
│
├── Experiment-09-Dining-Philosophers/
│   └── dining_philosophers.c
│
├── Experiment-10-Bankers-Algorithm/
│   └── bankers.c
│
├── Experiment-11-Memory-Allocation/
│   └── memory_allocation.c
│
├── Experiment-12-Page-Replacement/
│   └── page_replacement.c
│
└── Experiment-13-Disk-Scheduling/
    └── disk_scheduling.c
```

---

## 🎯 Learning Objectives

Through these experiments, the following Operating Systems concepts are practiced:

- UNIX commands and file management
- Process creation and system calls
- CPU scheduling
- Process synchronization
- Semaphores and POSIX threads
- Deadlock avoidance
- Memory allocation
- Page replacement
- Disk scheduling

---

## 👩‍💻 Author

**Subhashini S**

Computer Science and Engineering (AI & ML)

---

## 📌 Note

This repository is created for **Operating Systems Laboratory academic practice and reference**.

Each experiment contains the relevant program and can be compiled and executed using GCC on a UNIX/Linux environment.
