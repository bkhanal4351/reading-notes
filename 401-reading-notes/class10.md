## Stacks and Queues

What is a Stack
- A stack is a data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous.

Common terminology for a stack is

1. Push - Nodes or items that are put into the stack are pushed
2. Pop - Nodes or items that are removed from the stack are popped. When you attempt to pop an empty stack an exception will be raised.
3. Top - This is the top of the stack.
4. Peek - When you peek you will view the value of the top Node in the stack. When you attempt to peek an empty stack an exception will be raised.
5. IsEmpty - returns true when stack is empty otherwise returns false.

Concepts:

FILO: First In Last Out

LIFO: Last In First Out

Stack Visualization

![](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/images/stack1.PNG)


Push O(1)
Pushing a Nose is always constant as it takes same amount of time regardless of Nodes present.

Pop O(1)
Popping a Node off a stack is the action of removing a Node from the top. When conducting a pop, the top Node will be re-assigned to the Node that lives below and the top Node is returned to the user.

Peek O(1)
 - Peek method only inspects the top Node in stack which checks isEmpty before conducting a peek.his will ensure that an exception is not raised. Alternately, you can wrap the call in a try/catch block.

Here is the pseudocode for a peek

`ALGORITHM peek()`
// INPUT <-- none
// OUTPUT <-- value of top Node in stack
// EXCEPTION if stack is empty

   `return top.value`

IsEmpty O(1)

- `ALGORITHM isEmpty()`
// INPUT <-- none
// OUTPUT <-- boolean

`return top = NULL`

# What is a Queue
Common terminology for a queue is

Enqueue - Nodes or items that are added to the queue.
Dequeue - Nodes or items that are removed from the queue. If called when the queue is empty an exception will be raised.
Front - This is the front/first Node of the queue.
Rear - This is the rear/last Node of the queue.
Peek - When you peek you will view the value of the front Node in the queue. If called when the queue is empty an exception will be raised.
IsEmpty - returns true when queue is empty otherwise returns false.

Concepts:
FIFO: First In Last Out
LILO: Last In First Out

Queue Visualization

![](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/images/Queue.PNG)

Enqueue O(1)
When you add an item to a queue, you use the enqueue action. This is done with an O(1) operation in time because it does not matter how many other items live in the queue (n); it takes the same amount of time to perform the operation.

Dequeue O(1)
To remove an item we use dequeue action which is O(1) operation in time.

`ALGORITHM dequeue()`
// INPUT <-- none
// OUTPUT <-- value of the removed Node
// EXCEPTION if queue is empty

  `Node temp <-- front`
   `front <-- front.next`
   `temp.next <-- null`

   `return temp.value`

   Peek O(1)

   `ALGORITHM peek()`
// INPUT <-- none
// OUTPUT <-- value of the front Node in Queue
// EXCEPTION if Queue is empty

   `return front.value`

   IsEmpty O(1)

   `ALGORITHM isEmpty()`
// INPUT <-- none
// OUTPUT <-- boolean

`return front = NULL`

Notes taken from (https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/stacks_and_queues.html)

