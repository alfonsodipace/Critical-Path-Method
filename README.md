# Critical Path Method
The critical path method (CPM), or critical path analysis (CPA), is an algorithm for scheduling a set of project activities. It is commonly used in conjunction with the program evaluation and review technique (PERT). A critical path is determined by identifying the longest stretch of dependent activities and measuring the time required to complete them from start to finish. It has been built in the context of Project Management course with the Professor Francesco Orciuoli at the University of Salerno(UNISA).

# Why use it?
The critical path is the longest path in the project network diagram:
- Any activity on the critical path, if delayed, can delay the project;
- A critical path also gives the shortest time possible to complete the project;
- It is possible to have more than one critical path on a project. 

The “critical path” is the longest path in the network with only zero float activities

# Features
Implement a Python program for:
- reading a file with a table containing tasks, durations and dependencies;
- constructing the AON with ES, EF, LS and LF for each task;
- determining, for each task, if it is on the critical path;
- printing such information and the critical path.

# Architecture
- delivery.py is the program file.
- CPM.txt and CPM1.txt are the input files. You can choose which one to use.

Input file:
- (task id, task name, duration, dependencies) i.e. 20,B,10,10

Output file:
-task id, task name, duration, ES, EF, LS, LF, float, isCritical
-1, A, 12, 1, 12, 1, 12, 0, True
-2, B, 6, 13, 18, 31, 36, 18, False
-3, E, 12, 13, 24, 19, 30, 6, False
-4, F, 18, 13, 30, 13, 30, 0, True
-5, C, 2, 19, 20, 37, 38, 18, False
-6, G, 10, 31, 40, 31, 40, 0, True
-7, I, 8, 31, 38, 37, 44, 6, False
-8, D, 8, 21, 28, 39, 46, 18, False
-9, H, 6, 41, 46, 41, 46, 0, True
-10, J, 2, 39, 40, 45, 46, 6, False
-11, K, 8, 47, 54, 47, 54, 0, True

True if is on the critical path, false otherwise.

# Implementation
The app is built in Python.

# Credits
Critical Path Method has been developed by [Alfonso Di Pace](https://github.com/alfonsodipace).