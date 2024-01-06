# Operating-System-Project
# Sorting Algorithm Performance Comparison with Processes and Threads

## Objectives
The objective of this experiment is to test whether multithreading is faster than multiprocessing and a normal sorting algorithm.

## Introduction
In our semester project, we aimed to compare the performance of different sorting algorithms with multiprocessing and multithreading. We implemented the algorithms using the pthread.h library for threads and time.h to calculate the time taken to sort an array. We ran each test with six different arrays and recorded the results.

### Hypothesis
We predict that programs run with multithreading will produce the smallest elapsed time (ET). We predict that the programs running without any multithreading or multiprocessing will produce the largest ET.

## Algorithms
We used 5 algorithms to test our hypothesis:
- Mergesort
- Quicksort
- Selection sort
- Rank sort
- Radix sort

## Methodology
We first created an array of 8 elements and then ran the program using that array to minimize the variability in the generation of random numbers. We added the numbers to our spreadsheet and created a graph to compare each of the programs. We also did our best to write a program that produces the same number of threads as the number of fork calls to decrease variability. Our focus is on testing only the speed and not any other factors.

## Findings
### Mergesort
The normal (single-threaded) program consistently outperformed both the multithreaded and multiprocessing programs. Elapsed time for each sorting algorithm using normal, threading, and processing methods:

|        | Normal      | Threading   | Processing  |
|--------|-------------|-------------|-------------|
| 1      | 0.000003    | 4.00E-06    | 0.000683    |
| 2      | 0.000004    | 3.00E-06    | 0.001012    |
| 3      | 0.000003    | 5.00E-06    | 0.000484    |
| ...       | ...    | ...       | ...        |

<img width="900" alt="merge sort" src="https://github.com/0xZainRaza/Operating-System-Project/assets/154006182/043b163d-5313-412f-9d2d-383d893c523f">

### Quick sort
The findings indicate that the Quick sort algorithm has the smallest elapsed time when run in the normal program, followed by multithreading and multiprocessing.

| Algorithm | Normal | Threading | Processing |
|-----------|--------|-----------|------------|
| Quicksort | 0.000002 | 0.000174 | 0.000531 |
| ...       | ...    | ...       | ...        |

### Radix Sort
Based on the data, Radix sort with threading had the largest elapsed time, while Radix sort with multiprocessing had the smallest elapsed time.

| Algorithm | Normal | Threading | Processing |
|-----------|--------|-----------|------------|
| Radix sort| 0.000033 | 0.008366 | 0.000331 |
| ...       | ...    | ...       | ...        |

### Selection sort
The normal program consistently outperformed the multithreaded and multiprocessed programs for Selection Sort.

| Algorithm     | Normal | Threading | Processing |
|---------------|--------|-----------|------------|
| Selection Sort| 0.000002 | 0.00155 | 0.000949 |
| ...           | ...    | ...       | ...        |

### Rank sort
The performance of the rank sort algorithm with multiprocessing and multithreading is worse than the normal program.

| Algorithm | Normal | Threading | Processing |
|-----------|--------|-----------|------------|
| Rank Sort | 0.000002 | 0.001739 | 0.000246 |
| ...       | ...    | ...       | ...        |

## Conclusion
Contrary to our hypothesis, all the tests showed that the normal program runs faster than the multiprocess or multithreaded programs. It's important to note that the performance of multiprocessing and multithreading can vary depending on various factors such as the size of the data, the number of cores/threads available, the implementation of the algorithm, and the overhead of managing threads/processes. In our case, it's possible that the overhead of managing threads/processes outweighed the benefits of parallelization, leading to longer elapsed times.

In conclusion, our experiment showed that the normal program outperformed the programs with multiprocessing and multithreading. Future work could explore different implementations and configurations of the algorithms and experiment with larger datasets to further investigate the performance of multiprocessing and multithreading. It's important to interpret the findings in the context of the experimental setup and consider possible limitations and sources of error.

## Reference List
- [Reference programs](https://github.com/Mercurycode2002/OS_lab-_semester_4/tree/main/Semester_project)
- [Raw Data](https://docs.google.com/spreadsheets/d/1JxOdCUL4tyqbQ1IuryBof3mHqfYyAAj3SrZHm67oZvA/edit#gid=0)
- [Reference Study](https://www.diva-portal.org/smash/get/diva2:839729/FULLTEXT0)