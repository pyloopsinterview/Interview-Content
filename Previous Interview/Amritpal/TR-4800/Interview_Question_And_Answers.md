Here is the complete question written as a clean **Markdown (.md) document** you can save as an MD file.

---

# Recursion Symlink Linked List Problem

## Problem Statement

You are given a filesystem path that represents the head node of a singly linked list.
Each node in the list is represented by a symbolic link (symlink).
A symlink points to the next node in the linked list.

The linked list terminates when a path resolves to a regular file that is **not** a symlink.
This acts as the null pointer / end of list.

Your task is to write a Python program that:

1. Accepts a starting filesystem path from the command line.
2. Recursively follows symbolic links to traverse the linked list.
3. When recursion reaches the final non-symlink file, treat it as the end of list.
4. On the return (unwind) of recursion, collect node names in order.
5. Print the node names reversed, comma-separated.
6. Exit process successfully (exit code = 0).

---

## Requirements

### Functional Requirements

* Traverse a symlink-based linked list recursively.
* Print node names in **reverse** order.
* Recursion must do the reversal itself (no list.reverse, no slicing tricks).

### Constraints

* No loops and no explicit stacks.

* No reversing helper other than recursion.

* Errors (missing path, permission) must propagate.

* Only allowed filesystem methods/attributes:

  * `Path.is_symlink()`
  * `Path.readlink()`
  * `Path.name`

* Symlink targets may be relative paths and should resolve correctly.

* Program must be executable from the command line.

---

## Example

Given the following symbolic link chain:

```
4 -> 5
5 -> 6
6 -> 7
7 -> 8
8 -> /dev/null   # a regular file, base case
```

Running the program:

```
python reverse.py ./4
```

Expected output:

```
8,7,6,5,4
```

---

## Key Recursion Concepts Interviewer Expected

* Identify the base case: non-symlink = null pointer.
* Identify recursive case: follow symlink to next node.
* Use call stack to construct reversed result.
* Combine subproblem results through **return values**, not shared mutation.
* Think about how solution pieces compose during recursive unwind.

---

## Interviewer Hints and Discussion Notes

* Treat `/dev/null` like a null terminator.
* The recursion must "rebuild" solution while unwinding.
* Avoid relying only on side effects; return accumulated data.
* Using recursion for reversal is intentional for screening.
* Solver must demonstrate ability to decompose and recombine recursively.

---

If you want, I can now:

* include a polished recursive solution in idiomatic Python
* construct a spoken reasoning narrative for the interview
* write a unit test for the solution
* produce dry-run stack traces showing recursion unwind
