# C - File I/O
In this project, I learned about the three standard file descriptors and their `POSIX` names as well as the difference between function and system calls. I practiced using the I/O system calls `open`, `close`, `read`, and `write` and the flags `O_RDONLY`, `WR_ONLY`, and `O_RDWR` to create, open, close, read, write, set permissions of files in C.

## Header File 📁
main.h: Header file containing prototypes for all functions written in the project.

Function Prototypes:
| File | Prototype |
| ---- | --------- |
| `print_array.c` | `void print_array(const int *array, size_t size)` |
| `print_list.c` |`void print_list(const listint_t *list)` |
| `0-bubble_sort.c` | `0-bubble_sort.c	void bubble_sort(int *array, size_t size);` |
| `1-insertion_sort_list.c` | `void insertion_sort_list(listint_t **list);` |
| `2-selection-sort.c` | `void selection_sort(int *array, size_t size);` |
| `3-quick_sort.c` | `void quick_sort(int *array, size_t size);` |
| `100-shell_sort.c` | `void shell_sort(int *array, size_t size);` |
| `101-cocktail_sort_list.c` | `void cocktail_sort_list(listint_t **list);` |
| `102-counting_sort.c` | `void counting_sort(int *array, size_t size);` |
| `103-merge_sort.c` | `void merge_sort(int *array, size_t size);` |
| `104-heap_sort.c` | `void heap_sort(int *array, size_t size);` |
| `105-radix_sort.c` | `void radix_sort(int *array, size_t size);` |
| `106-bitonic_sort.c` | `void bitonic_sort(int *array, size_t size);` |
| `107-quick_sort_hoare.c` | `void quick_sort_hoare(int *array, size_t size);` |
