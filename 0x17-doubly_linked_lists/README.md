# C - Doubly linked lists
In this project, I learned about using doubly-linked lists in C.

## Header File 📁
- [lists.h](https://github.com/richard-1257/alx-low_level_programming/blob/master/0x17-doubly_linked_lists/lists.h): Header file containing definitions and prototypes for all types and functions written for the project.


Function Prototypes:
| Type/File | Definition/Prototype |
| ---- | --------- |
| `struct dlistint_s` | `int n` `struct dlistint_s *prev` `struct dlistint_s *new` |
| `typedef dlistint_t` |`struct dlistint_s` |
| `0-print_dlistint.c` | `size_t print_dlistint(const dlistint_t *h);` |
| `1-dlistint_len.c` | `size_t dlistint_len(const dlistint_t *h);` |
| `2-add_dnodeint.c` | `dlistint_t *add_dnodeint(dlistint_t **head, const int n);` |
| `3-add_dnodeint_end.c` | `dlistint_t *add_dnodeint_end(dlistint_t **head, const int n);` |
| `4-free_dlistint.c` | `void free_dlistint(dlistint_t *head);` |
| `5-get_dnodeint.c` | `dlistint_t *get_dnodeint_at_index(dlistint_t *head, unsigned int index);` |
| `6-sum_dlistint.c` | `int sum_dlistint(dlistint_t *head);` |
| `7-insert_dnodeint.c` | `dlistint_t *insert_dnodeint_at_index(dlistint_t **h, unsigned int idx, int n);` |
| `8-delete_dnodeint.c` | `int delete_dnodeint_at_index(dlistint_t **head, unsigned int index);` |


- [deck.h](https://github.com/richard-1257/sorting_algorithms/blob/master/deck.h): Header file containing definitions and prototypes for all types and functions written for the task `1000-sort_deck.c`.

Data Structures:

```python
typedef enum kind_e
{
	SPADE = 0,
	HEART,
	CLUB,
	DIAMOND
} kind_t;

typedef struct card_s
{
	const char *value;
	const kind_t kind;
} card_t;

typedef struct deck_node_s
{
	const card_t *card;
	struct deck_node_s *prev;
	struct deck_node_s *next;
} deck_node_t;
```

Function Prototype:
| File | Prototype |
| ------------- | ------------- |
| `1000-deck_node.c` | `void sort_deck(deck_node_t **deck);` |


## Tasks 📃
- 0. Bubble sort
     - [0-bubble_sort.c](https://github.com/richard-1257/sorting_algorithms/blob/master/0-bubble_sort.c):  C function that sorts an array of integers in ascending order using the Bubble Sort algorithm.
     - Prints the array after each swap.
     - [0-O](https://github.com/richard-1257/sorting_algorithms/blob/master/0-O): Text file containing the best, average, and worst case time complexities of the Bubble Sort algorithm, one per line.
     
- 1. Insertion sort
     - [1-insertion_sort_list.c](https://github.com/richard-1257/sorting_algorithms/blob/master/1-insertion_sort_list.c): C function that sorts a `listint_t` doubly-linked list of integers in ascending order using the Insertion Sort algorithm.
     - Prints the list after each swap.
     - [1-O](https://github.com/richard-1257/sorting_algorithms/blob/master/1-O): Text file containing the best, average, and worst case time complexities of the Insertion Sort algorithm, one per line.
     
