# C - File I/O
In this project, I learned about the three standard file descriptors and their `POSIX` names as well as the difference between function and system calls. I practiced using the I/O system calls `open`, `close`, `read`, and `write` and the flags `O_RDONLY`, `WR_ONLY`, and `O_RDWR` to create, open, close, read, write, set permissions of files in C.

## Header File 📁
[main.h](https://github.com/richard-1257/alx-low_level_programming/blob/master/0x15-file_io/main.h): Header file containing prototypes for all functions written in the project.

Function Prototypes:
| File | Prototype |
| ---- | --------- |
| `0-read_textfile.c` | `ssize_t read_textfile(const char *filename, size_t letters);` |
| `1-create_file.c` |`int create_file(const char *filename, char *text_content);` |
| `2-append_text_to_file.c` | `int append_text_to_file(const char *filename, char *text_content);` |

## Tasks 📃
- 0. Tread lightly, she is near
     - [0-read_textfile.c](https://github.com/richard-1257/alx-low_level_programming/blob/master/0x15-file_io/0-read_textfile.c):  C function that reads a text file and prints it to the `POSIX` standard output.
     - The parameter `letters` is the number of letters the function should read and print.
     - If the file is `NULL` or cannot be opened or read - returns `0`.
     - If the `write` call fails or does not write the expected number of bytes - returns `0`.
     - Otherwise - returns the actual number of bytes the function can read and print.
     
- 1. Under the snow
     - [1-insertion_sort_list.c](https://github.com/richard-1257/sorting_algorithms/blob/master/1-insertion_sort_list.c): C function that sorts a `listint_t` doubly-linked list of integers in ascending order using the Insertion Sort algorithm.
     - Prints the list after each swap.
     - [1-O](https://github.com/richard-1257/sorting_algorithms/blob/master/1-O): Text file containing the best, average, and worst case time complexities of the Insertion Sort algorithm, one per line.
     
- 2. Selection sort
     - [2-selection_sort.c](https://github.com/richard-1257/sorting_algorithms/blob/master/2-selection_sort.c): C function that sorts an array of integers in ascending order using the Selection Sort algorithm.
     - Prints the array after each swap.
     - [2-O](https://github.com/richard-1257/sorting_algorithms/blob/master/2-O): Text file containing the best, average, and worst case time complexities of the Selection Sort algorithm, one per line.

- 3. Quick sort
     - [3-quick_sort.c](https://github.com/richard-1257/sorting_algorithms/blob/master/3-quick_sort.c): C function that sorts an array of integers in ascending order using the Quick Sort algorithm.
     - Implements the Lomuto partition scheme.
     - Always uses the last element of the partition being sorted as the pivot.
     - Prints the array after each swap.
     -[3-O](https://github.com/richard-1257/sorting_algorithms/blob/master/3-O): Text file containing the best, average, and worst case time complexities of the Quick Sort Lomuto Partition scheme algorithm, one per line.

- 4. Shell sort - Knuth Sequence
     - [100-shell_sort.c](https://github.com/richard-1257/sorting_algorithms/blob/master/100-shell_sort.c): C function that sorts an array of integers in ascending order using the Shell sort algorithm.
     - Implements the Knuth interval sequence.
     - Prints the array each time the interval is decreased.
     
- 5. Cocktail shaker sort
     - [101-cocktail_sort_list.c](https://github.com/richard-1257/sorting_algorithms/blob/master/101-cocktail_sort_list.c): C function that sorts a `listint_t` doubly-linked list of integers in ascending order using the Cocktail Shaker Sort algorithm.
     - Prints the list after each swap.
     - [101-O](https://github.com/richard-1257/sorting_algorithms/blob/master/101-O): Text file containing the best, average, and worst case time complexities of the Cocktail Shaker Sort algorithm, one per line.
     
- 6. Counting sort
     - [102-counting_sort.c](https://github.com/richard-1257/sorting_algorithms/blob/master/102-counting_sort.c): C function that sorts an array of integers in ascending order using the Counting Sort algorithm.
     - Assumes that the array will only contain numbers `>= 0`.
     - Prints the counting array after it has been initialized.
     - [102-O](https://github.com/richard-1257/sorting_algorithms/blob/master/102-O): Text file containing the best, average, and worst case time complexities of the Counting Sort algorithm, one per line.
     
- 7. Merge sort
     - [103-merge_sort.c](https://github.com/richard-1257/sorting_algorithms/blob/master/103-merge_sort.c): C function that sorts an array of integers in ascending order using the Merge Sort algorithm.
     - Implements the `top-down` Merge Sort algorithm
         - When an array is divided, the size of the left subarray is always less than or equal to the size of the right subarray.
         - Always sorts the left subarray before the right one.
     - Prints subarrays each time they are merged.
     - [103-O](https://github.com/richard-1257/sorting_algorithms/blob/master/103-O): Text file containing the best, average, and worst case time complexities of the Merge Sort algorithm, one per line.

- 8. Heap sort
     - [104-heap_sort.c](https://github.com/richard-1257/sorting_algorithms/blob/master/104-heap_sort.c): C function that sorts an array of integers in ascending order using the Heap Sort algorithm.
     - Implements the `sift-down` Heap Sort algorithm.
     - Prints the array after each swap.
     - [104-O](https://github.com/richard-1257/sorting_algorithms/blob/master/104-O): Text file containing the best, average, and worst case time complexiites of the Heap Sort algorithm, one per line.
     
- 9. Radix sort
     -[105-radix_sort.c](https://github.com/richard-1257/sorting_algorithms/blob/master/105-radix_sort.c): C function that sorts an array of integers in ascending order using the Radix Sort algorithm.
     - Implements the Least-Significant-Digit (LSD) Radix Sort algorithm.
     - Assumes that the array will only contain numbers `>= 0`.
     - Prints the array for each significant digit increase.
     - [105-O](https://github.com/richard-1257/sorting_algorithms/blob/master/105-O): Text file containing the best, average, and worst case time complexities of the Radix Sort algorithm, one per line.
     
- 10. Bitonic sort
      - [106-bitonic_sort.c](https://github.com/richard-1257/sorting_algorithms/blob/master/106-bitonic_sort.c):  C function that sorts an array of integers in ascending order using the Bitonic Sort algorithm.
      - Assumes that `size` is a power of 2 (ie. `size` can be expressed as `2^k` where `k >= 0`).
      - Prints subarrays each time they are merged.
      - [106-O](https://github.com/richard-1257/sorting_algorithms/blob/master/106-O): Text file containing the best, average, and worst case time complexities of the Bitonic Sort algorithm, one per line.
      
- 11. Quick Sort - Hoare Partition scheme
      - [107-quick_sort_hoare.c](https://github.com/richard-1257/sorting_algorithms/blob/master/107-quick_sort_hoare.c): C function that sorts an array of integers in ascending order using the Quick Sort algorithm.
      - Implements the Hoare partition scheme.
      - Always uses the last elemement of the partition being sorted as the pivot.
      - Prints the array after each swap.
      - [107-O](https://github.com/richard-1257/sorting_algorithms/blob/master/107-O): Text file containing the best, average, and worst case time complexities of the Quick Sort Hoare Partition cheme algorithm, one per line.
      
- 12. Dealer
      - [1000-sort_deck.c](https://github.com/richard-1257/sorting_algorithms/blob/master/1000-sort_deck.c): C function that sorts a `deck_node_t` doubly-linked list deck of cards.
      - Assumes that there are exactly 52 elements in the doubly-linked list.
      - Orders the deck from spades to diamonds and from aces to kings.
      
