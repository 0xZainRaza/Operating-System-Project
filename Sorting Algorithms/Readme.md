# Sorting Algorithms Study

We conducted a study to test our hypothesis using five distinct sorting algorithms. Each algorithm has its unique approach to sorting data efficiently. Below is an overview of the algorithms employed in our study.

## Algorithms

1. **Mergesort**
   - Mergesort divides the array into two equal halves until only two elements remain. It then recursively sorts each half and merges them back together, producing a fully sorted array.

2. **Quicksort**
   - Quicksort selects a pivot (in our case, the last element) and rearranges the array such that elements greater than the pivot are placed after it, and elements less than the pivot are placed before it. This process is repeated recursively.

3. **Selection Sort**
   - Selection Sort is a simple sorting algorithm that iteratively finds the smallest element in the array and swaps it with the first element. This process is repeated for the remaining unsorted portion of the array.

4. **Rank Sort**
   - Rank Sort involves finding the maximum element in the input array, creating a count array, and determining the rank of each element. The sorted output array is then constructed based on the ranks of the elements in reverse order.

5. **Radix Sort**
   - Radix Sort is a non-comparative sorting algorithm that sorts numbers based on individual digits. It involves creating buckets for each digit (0-9) and repeatedly sorting the numbers based on their least significant digit, then moving to the next significant digit until all digits are sorted.

## Usage

Feel free to explore the source code in this repository to understand the implementation details of each sorting algorithm. Additionally, you can check the results obtained from our study to gain insights into their efficiency and performance in different scenarios.

