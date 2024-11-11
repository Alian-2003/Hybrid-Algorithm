**Overview:**
Merge Sort for large subarrays to guarantee O(n log n) performance.
Quick Sort as a primary sorting method, ideal for medium-sized subarrays.
Insertion Sort for very small subarrays, where it is often faster than Quick Sort and Merge 	Sort due to low overhead.
**Hybrid Strategy:**
Quick Sort is used as the main sorting technique.
If the subarray size becomes very small (e.g., fewer than 50 elements), switch to Insertion Sort for improved efficiency.
Merge Sort is used to handle large subarrays to ensure stability and predictable performance on large, unsorted data.

**Explanation of the Code:**
Insertion Sort is applied to very small subarrays within Quick Sort (e.g., arrays smaller than 20 elements).
Quick Sort is the primary sorting mechanism when array sizes are moderately small (e.g., less than 50 elements).
Merge Sort is used on large arrays to ensure stable O(n log n) performance for large datasets.

  **Performance Analysis:**

**Time Complexity:**
Quick Sort with Insertion Sort handles small and moderately sized arrays efficiently.
Merge Sort provides stable O(n log n) performance for large arrays.
**Space Complexity:**
Quick Sort is efficient with minimal extra space, especially when combined with Insertion Sort.
Merge Sort requires additional space but performs reliably on larger datasets.
