# 🧠 CPU Scheduling Algorithms Simulator (C++)

This project is a **C++ console-based simulator** that demonstrates the functionality of various **CPU scheduling algorithms** used in operating systems. It includes:

- FCFS (First-Come, First-Served)
- RR (Round Robin)
- SPN (Shortest Process Next)
- SRT (Shortest Remaining Time)
- HRRN (Highest Response Ratio Next)
- FB-1 (Feedback Queue with 1-Quantum Levels)

## 📌 Project Features

- ✅ Clean and readable single-file implementation.
- ✅ Supports user-defined process arrival times and burst times.
- ✅ Configurable time quantum for Round Robin and Feedback Queue.
- ✅ Calculates and displays:
  - Completion Time
  - Turnaround Time
  - Waiting Time
  - Gantt Chart representation
- ✅ Easy to compile and run on any C++ environment.

---

## 🚀 Algorithms Implemented

### 1. FCFS (First-Come, First-Served)
- Non-preemptive
- Processes are scheduled in the order they arrive.

### 2. RR (Round Robin)
- Preemptive
- Each process gets a fixed time slice (quantum).
- Ensures better fairness and responsiveness.

### 3. SPN (Shortest Process Next)
- Non-preemptive
- Selects the process with the shortest burst time among those that have arrived.

### 4. SRT (Shortest Remaining Time)
- Preemptive version of SPN
- Picks the process with the shortest remaining burst time.

### 5. HRRN (Highest Response Ratio Next)
- Non-preemptive
- Priority = (Waiting Time + Burst Time) / Burst Time
- Helps balance fairness and efficiency.

### 6. FB-1 (Feedback Queue with 1-Quantum Levels)
- Preemptive, multi-level queue
- Each process starts in the highest priority queue and moves down if it doesn’t finish within its time slice.
- Uses 1 time quantum per level, ensuring dynamic aging.

---

## 🛠️ How to Compile and Run

### ✅ Requirements
- A C++ compiler (g++, clang++, etc.)
- Any OS (Windows, Linux, Mac)

### ⚙️ Compile:
```bash
g++ -o scheduler main.cpp
