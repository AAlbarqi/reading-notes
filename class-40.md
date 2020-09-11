# Stacks and Queues

## Queue 
A queue works like a line for an amusement park ride -- people enter at the end of the queue and leave from the front (FIFO: first in, first out).

![](https://s3-us-west-2.amazonaws.com/forge-production.galvanize.com/releases/4395/Data%20Modeling%20%26%20Classes/images/200px-Data_Queue.svg.png)

A queue would be great for....
Issuing instructions to your sandwich-making robot.

**Operations:**

![](https://i1.faceprep.in/Companies-1/queue-operations.gif)

- Enqueue O(1)
When you add an item to a queue, you use the enqueue action. This is done with an O(1) operation in time because it does not matter how many other items live in the queue (n); it takes the same amount of time to perform the operation.

- Dequeue O(1)
When you remove an item from a queue, you use the dequeue action. This is done with an O(1) operation in time because it doesn’t matter how many other items are in the queue, you are always just removing the front Node of the queue.

## Stack 

A stack is a data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous.

A stack works like a stack of plates -- plates are added and removed from the the top of the stack (LIFO: last in, first out).

![](https://s3-us-west-2.amazonaws.com/forge-production.galvanize.com/releases/4395/Data%20Modeling%20%26%20Classes/images/200px-Data_stack.svg.png)

A stack would be great for...
Implementing your browser's back button.

**Operations:**

![](https://i1.faceprep.in/Companies-1/stack-operations-in-c.gif)

- Push O(1)
Pushing a Node onto a stack will always be an O(1) operation. This is because it takes the same amount of time no matter how many Nodes (n) you have in the stack.

- Pop O(1)
Popping a Node off a stack is the action of removing a Node from the top. When conducting a pop, the top Node will be re-assigned to the Node that lives below and the top Node is returned to the user.