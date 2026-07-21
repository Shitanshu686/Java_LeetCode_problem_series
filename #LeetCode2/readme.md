# LeetCode 2 - Add Two Numbers

## Problem Statement

You are given two non-empty linked lists representing two non-negative integers. The digits are stored in reverse order, and each node contains a single digit. Add the two numbers and return the sum as a linked list.

---

## Approach

- Create a dummy node to simplify linked list construction.
- Traverse both linked lists simultaneously.
- Add the corresponding digits along with the carry.
- Store the current digit (`sum % 10`) in a new node.
- Update the carry (`sum / 10`).
- Continue until both lists are fully traversed.
- If a carry remains after the loop, add it as the last node.
- Return `dummy.next` as the head of the resulting linked list.

---

## Algorithm

1. Initialize a dummy node and a current pointer.
2. Initialize `carry = 0`.
3. Traverse while either list has remaining nodes.
4. Read values from both lists (use `0` if a list has ended).
5. Compute the sum and update the carry.
6. Create a new node with the current digit.
7. Move all pointers forward.
8. Add the remaining carry if it exists.
9. Return `dummy.next`.

---

## Time Complexity

- **O(max(m, n))**

where `m` and `n` are the lengths of the two linked lists.

---

## Space Complexity

- **O(max(m, n))**

A new linked list is created to store the result.

---

## Concepts Used

- Linked List
- Dummy Node
- Carry Handling
- Pointer Manipulation
- Simulation

---

## Language

- Java
