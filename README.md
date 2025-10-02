
# Queue in C++

## Theory

A **Queue** is a linear data structure that works on the **FIFO (First In, First Out)** principle.
This means the element inserted first is the one that gets removed first.

It contrasts with a **Stack**, which follows the **LIFO (Last In, First Out)** principle.

---

## Key Concepts

* **Front** → Position of the element to be removed (oldest element).
* **Rear** → Position where the next element will be inserted.
* **Enqueue (Insertion)** → Adds an element at the rear.
* **Dequeue (Deletion)** → Removes an element from the front.
* **Display** → Shows all elements in the queue.

---

## Characteristics

* **Sequential Processing** → Elements are handled in the order they arrive.
* **Restricted Operations** → Insertions only at the rear, deletions only from the front.
* **Overflow** → Occurs when the queue is full and no more elements can be added.
* **Underflow** → Occurs when the queue is empty and no element can be removed.

---

## Types of Queues

1. **Simple (Linear) Queue** → Insertion at rear, deletion from front.
2. **Circular Queue** → Solves the space wastage problem of linear queues.
3. **Priority Queue** → Elements are dequeued based on priority rather than order.
4. **Deque (Double-Ended Queue)** → Allows insertion and deletion from both ends.

---

## Stack vs Queue

| Feature          | Stack (LIFO)         | Queue (FIFO)          |
| ---------------- | -------------------- | --------------------- |
| **Insertion**    | At the top           | At the rear           |
| **Deletion**     | From the top         | From the front        |
| **Access Order** | Last in, first out   | First in, first out   |
| **Use Cases**    | Function calls, undo | Scheduling, buffering |

---

## Program Summary

The program implements a **simple queue using arrays**.
It supports **enqueue, dequeue, and display operations**, while also handling **overflow** and **underflow** conditions.

---

## Algorithm

1. **Start**
2. **Initialize**: `front = -1, rear = -1`.

### Enqueue(value):

* If `rear == SIZE - 1` → print `"Overflow"`.
* Else, increment `rear` and insert value into `arr[rear]`.
* If `front == -1`, set `front = 0`.

### Dequeue():

* If `front == -1 OR front > rear` → print `"Underflow"`.
* Else, remove element at `arr[front]` and increment `front`.

### Display():

* If queue is empty → print `"Queue is empty"`.
* Else, traverse from `front` to `rear` and print elements.

3. Perform operations as per `main()`.
4. **End**

---

## Conclusion

This experiment demonstrated the **concept and implementation of a queue in C++** using arrays.

### Key observations:

* The **FIFO principle** was effectively demonstrated.
* **Overflow** occurs when inserting into a full queue.
* **Underflow** occurs when removing from an empty queue.
* **Class-based encapsulation in C++** simplifies queue operations and improves modularity.

### Real-Life Applications:

* **CPU scheduling** in operating systems.
* **Printer queue management**.
* **Buffering** in network communications.
* **Task scheduling systems**.

Queues are essential for **managing sequential tasks efficiently** and ensuring smooth operation in both software and hardware systems.

