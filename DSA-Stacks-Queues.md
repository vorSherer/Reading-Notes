# Read 10 - Stacks and Queues in Python

#### 2020-06-30

## RESOURCES:
#### Stacks and Queues <br>
https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/stacks_and_queues.html <br>

---
### Stacks
A __*Stack*__ is a __data structure__ that links __nodes__, but in a __First-In-Last-Out/Last-In-First-Out (FILO/LIFO)__ fashion. That is, each new node added ("__pushed__") to the stack points to the node previously at the "__top__" of the stack. The top node is the only node that can be removed ("__popped__") from the stack. One may "__peek__" at the falue of the __top__ node while it remains on the stack. It is recommended that one check to see whether the stack __IsEmpty__ (a boolean return) before attempting to pop a node off the stack to avoid raising an exception. <br>
*Think of a stack of pancakes; if eaten one-at-a-time, the first on the plate is the last one eaten. The diner can see the top pancake before eating it, but not the ones below. The pancakes are then eaten from top to bottom, but attempting to continue eating after the bottom pancake is gone doesn't work very well.* <br>

---
### Queues
A __Queue__ is similar to a singly linked list, but with the difference that new nodes are added ("__enqueued__") at the __rear__ of the queue, and removed ("__dequeued__") from the __front__ of the queue in a __First-In-First-Out/Last-In-Last-Out (FIFO/LILO)__ fashion. One may still __peek__ at the value of the __front__ node without dequeuing it, and check to see whether the queue is empty with __IsEmpty__ before attempting to dequeue a node to avoid raising an exception. <br>
*Think of a vending machine; one may see what is at the front of a given location in the machine, but if one desires the third item in, one must first pop off the two in front of it before getting the desired item. New items are restocked at the back of each position, one at a time. As before, once a queue is empty, trying to get anything more from it doesn't go very well.* <br>
