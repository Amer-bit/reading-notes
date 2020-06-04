#   Stacks and Queues

## Stacks
A stack is a basic data structure that can be logically thought of as a linear structure represented by a real physical stack or pile, a structure where insertion and deletion of items takes place at one end called top of the stack. The basic concept can be illustrated by thinking of your data set as a stack of plates or books where you can only take the top item off the stack in order to remove things from it. This structure is used all throughout programming.

The basic implementation of a stack is also called a LIFO (Last In First Out) to demonstrate the way it accesses data, since as we will see there are various variations of stack implementations.

There are basically three operations that can be performed on stacks. They are 1) inserting an item into a stack (push). 2) deleting an item from the stack (pop). 3) displaying the contents of the stack (peek or top).

1. push → Add the new element to the stack
If the number of elements pushed on stack are greater than the maximum size of the stack, we have a “Stack Overflow”. Otherwise, we can add a new element to the stack.
2. pop → Remove the last element placed on the stack
If the stack doesn’t have any element (empty), we can’t pop. Otherwise, we just decrease the numberOfElements value.
3. top → Returns the last element placed on the stack
4. isEmpty → Returns if the stack is empty or not
Verify if there are any element in the stack. Returns true if the stack is empty, and false otherwise.
5. Peek - When you peek you will view the value of the top Node in the stack. When you attempt to peek an empty stack an exception will be raised.

## Queue
A Queue is a linear structure which follows a particular order in which the operations are performed. The order is First In First Out (FIFO). A good example of a queue is any queue of consumers for a resource where the consumer that came first is served first. The difference between stacks and queues is in removing. In a stack we remove the item the most recently added; in a queue, we remove the item the least recently added
Basic Operations
Queue operations may involve initializing or defining the queue, utilizing it, and then completely erasing it from the memory. Here we shall try to understand the basic operations associated with queues −

enqueue() − add (store) an item to the queue.

dequeue() − remove (access) an item from the queue.

Few more functions are required to make the above-mentioned queue operation efficient. These are −

peek() − Gets the element at the front of the queue without removing it.

Rear - This is the rear/last Node of the queue.

Peek - When you peek you will view the value of the front Node in the 
queue. If called when the queue is empty an exception will be raised.

isfull() − Checks if the queue is full.

isempty() − Checks if the queue is empty.

In queue, we always dequeue (or access) data, pointed by front pointer and while enqueing (or storing) data in the queue we take help of rear pointer.