# C - Search Algorithms

This was my ALX project on search algorithms. I implemented various types of search algorithms and stated the corresponding space/time complexities for each.

## Tests 🧪
[Tests](https://github.com/richard-1257/alx-low_level_programming/tree/master/0x1E-search_algorithms/tests): Folder of test files for all tasks. Provided by ALX.

## Helper Files 🙌
[listint](https://github.com/richard-1257/alx-low_level_programming/tree/master/0x1E-search_algorithms/listint): Folder of helper files for task 12, singly linked list jump search.
  - [create_list.c](https://github.com/richard-1257/alx-low_level_programming/blob/master/0x1E-search_algorithms/listint/create_list.c): C function that creates a `listint_t` singly linked list.
  - [free_list.c](https://github.com/richard-1257/alx-low_level_programming/blob/master/0x1E-search_algorithms/listint/free_list.c): C function that frees a `listint_t` singly linked list.
  - [print_list.c](https://github.com/richard-1257/alx-low_level_programming/blob/master/0x1E-search_algorithms/listint/print_list.c): C function that prints the contents of a `listint_t` singly linked list.
  
[skiplist](https://github.com/richard-1257/alx-low_level_programming/tree/master/0x1E-search_algorithms/skiplist): Folder of helper files for task 13, singly skipped list jump search.
  - [create_skiplist.c](https://github.com/richard-1257/alx-low_level_programming/blob/master/0x1E-search_algorithms/skiplist/create_skiplist.c): C function that creates a `skiplist_t` singly skipped list.
  - [free_skiplist.c](https://github.com/richard-1257/alx-low_level_programming/blob/master/0x1E-search_algorithms/skiplist/free_skiplist.c): C function that frees a `skiplist_t` singly skipped list.
  - [print_skiplist.c](https://github.com/richard-1257/alx-low_level_programming/blob/master/0x1E-search_algorithms/skiplist/print_skiplist.c): C function that prints the contents of a `skiplist_t` singly skipped list.

## Header File 📁

- [search_algos.h](https://github.com/richard-1257/alx-low_level_programming/blob/master/0x1E-search_algorithms/search_algos.h): Header file containing definitions and prototypes for all types and functions written for the project.

Data Structure:

```python
/**
 * struct listint_s - singly linked list
 *
 * @n: Integer
 * @index: Index of the node in the list
 * @next: Pointer to the next node
 *
 * Description: singly linked list node structure
 * for ALX project
 */
typedef struct listint_s
{
    int n;
    size_t index;
    struct listint_s *next;
} listint_t;

/**
 * struct skiplist_s - Singly linked list with an express lane
 *
 * @n: Integer
 * @index: Index of the node in the list
 * @next: Pointer to the next node
 * @express: Pointer to the next node in the express lane
 *
 * Description: singly linked list node structure with an express lane
 * for Holberton project
 */
typedef struct skiplist_s
{
    int n;
    size_t index;
    struct skiplist_s *next;
    struct skiplist_s *express;
} skiplist_t;
```

Function Prototypes:
| File | Prototype |
| ---- | --------- |
| `0-linear.c` | `int linear_search(int *array, size_t size, int value);` |
| `1-binary.c` |`int binary_search(int *array, size_t size, int value);` |
| `100-jump.c` | `int jump_search(int *array, size_t size, int value);` |
| `102-interpolation.c` | `int interpolation_search(int *array, size_t size, int value);` |
| `103-exponential.c` | `int exponential_search(int *array, size_t size, int value);` |
| `104-advanced_binary.c` | `int advanced_binary(int *array, size_t size, int value);` |

## Tasks 📃

- 0. Linear search
  - [0-linear.c](https://github.com/richard-1257/alx-low_level_programming/blob/master/0x1E-search_algorithms/0-linear.c): C function that searches for a value in an array of integers using linear search.
  - If the value is not present or the array is `NULL`, returns `-1`.
    - Otherwise, returns the first index where `value` is located.
- 1. Binary search
  - [1-binary.c](https://github.com/richard-1257/alx-low_level_programming/blob/master/0x1E-search_algorithms/1-binary.c): C function that searches for a value in a sorted array of integers using binary search.
  - Assumes the array is sorted in ascending order and that the value to search for is not repeated in the array.
  - If the value is not present or the array is `NULL`, returns `-1`.
    - Otherwise, returns the index where `value` is located. 
