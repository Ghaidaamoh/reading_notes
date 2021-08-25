# Stacks and Queues

**What is a Stack**

- A stack is a data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous.

**Common terminology for a stack**

1. Push: Nodes or items that are put into the stack are pushed
2. Pop: Nodes or items that are removed from the stack are popped. When you attempt to pop an empty stack an exception will be raised.
3. Top: This is the top of the stack.
4. Peek: When you peek you will view the value of the top Node in the stack. When you attempt to peek an empty stack an exception will be raised.
5. IsEmpty: returns true when stack is empty otherwise returns false.

**Stacks follow these concepts**

- FILO: First In Last Out,this means that the first item added in the stack will be the last item popped out of the stack.
- LIFO: Last In First Out,this means that the last item added to the stack will be the first item popped out of the stack.

**Stack Visualization**

- example of what a stack looks like:
![stack](./images/stack1.png)

- As you can see, the topmost item is denoted as the top. When you push something to the stack, it becomes the new top. When you pop something from the stack, you pop the current top and set the next top as top.next.

**Push O(1)**

- Pushing a Node onto a stack will always be an O(1) operation. This is because it takes the same amount of time no matter how many Nodes (n) you have in the stack.
- When adding a Node, you push it into the stack by assigning it as the new top, with its next property equal to the original top.

**How push work**

1. First, you should have the Node that you want to add.
2. Next, you need to assign the next property of the added Node to reference the same Node that top is referencing
3. Your new Node is added to your stack, but there is no indication that it is the first Node in the stack. To make this happen, you have to re-assign our reference top to the newly added Node.
4. Now it's completed a successfully push of the new Node onto the stack.

**Here is the pseudocode to push a value onto a stack:**

- ALOGORITHM push(value)

- // INPUT <-- value to add, wrapped in Node internally

- // OUTPUT <-- none

- node = new Node(value)

- node.next <-- Top

- top <-- Node

**Pop O(1)**

- Popping a Node off a stack is the action of removing a Node from the top. When conducting a pop, the top Node will be re-assigned to the Node that lives below and the top Node is returned to the user.

- You would check isEmpty before conducting a pop.

**How pop work**

1. The first step of removing the Node from the stack is to create a reference named temp that points to the same Node that top points to.
2. Once you have created the new reference type, you now need to re-assign top to the value that the next property is referencing.
3. We can now remove the Node safely without it affecting the rest of the stack.Before we do that though you may want to make sure that you clear out the next property in your current temp reference.
4. Return the value of the temp Node that was just popped off.

**Here is the pseudocode for a pop**

- ALGORITHM pop()
- // INPUT <-- No input
- // OUTPUT <-- value of top Node in stack

- // EXCEPTION if stack is empty
- Node temp <-- top
- top <-- top.next
- temp.next <-- null
- return temp.value

**Peek O(1)** 

- When conducting a peek, you will only be inspecting the top Node of the stac
- You would check isEmpty before conducting a peek. This will ensure that an exception is not raised. Alternately, you can wrap the call in a try/catch block.

**Here is the pseudocode for a peek**

- ALGORITHM peek()
- // INPUT <-- none
- // OUTPUT <-- value of top Node in stack
- // EXCEPTION if stack is empty
- return top.value

**IsEmpty O(1)**

**Here is the pseudocode for isEmpty**

- ALGORITHM isEmpty()
- // INPUT <-- none
- // OUTPUT <-- boolean
- return top = NULL

**What is a Queue**

**Common terminology for a stack**

1. Enqueue: Nodes or items that are added to the queue.
2. Dequeue: Nodes or items that are removed from the queue. If called when the queue is empty an exception will be raised.
3. Front: This is the front/first Node of the queue.
4. Rear: This is the rear/last Node of the queue.
5. Peek: When you peek you will view the value of the front Node in the queue. If called when the queue is empty an exception will be raised.
6. IsEmpty: returns true when queue is empty otherwise returns false.

**Queues follow these concepts**

- FILO: First In Last Out,This means that the first item in the queue will be the first item out of the queue.
- LIFO: Last In First Out,This means that the last item in the queue will be the last item out of the queue.

**Queue Visualization**

- example of what a stack looks like:
![que](./images/que.png)

**Enqueue O(1)**

- When you add an item to a queue, you use the enqueue action. This is done with an O(1) operation in time because it does not matter how many other items live in the queue (n); it takes the same amount of time to perform the operation.

**How Enqueue work** 

1. First, we should change the next property of current Node to point to the new Node we are adding.

   - Following the rules of reference types, this means that we must change rear.next to new Node

2. After we have set the next property, we can re-assign the rear reference to point to new Node. By doing this, it allows us to keep a reference of where the rear is, and we can continue to enqueue Nodes into the queue as needed.
3. It's successfully added a Node to a queue by activating the enqueue action.

**Here is the pseudocode for the enqueue method**

- ALGORITHM enqueue(value)
- // INPUT <-- value to add to queue (will be wrapped in Node internally)
- // OUTPUT <-- none
- node = new Node(value)
- rear.next <-- node
- rear <-- node

**Dequeue O(1)**

- When you remove an item from a queue, you use the dequeue action. This is done with an O(1) operation in time because it doesn’t matter how many other items are in the queue, you are always just removing the front Node of the queue.
- you would check isEmpty before conducting a dequeue. This will ensure that an exception is not raised. Alternately, you can wrap the call in a try/catch block..

**How Dequeue work**

1. The first thing you want to do is create a temporary reference type named temp and have it point to the same Node that front is pointing too.
2. Next, you want to re-assign front to the next value that the Node front is referencing.
3. Now that we have moved front to the second Node in line, we can next re-assign the next property on the temp Node to null.
4. Finally, we return the value of the temp Node that was just removed.
5. It's successfully completed a dequeue action on a queue!

**Here is the pseudocode for the dequeue method**

- ALGORITHM dequeue()
- // INPUT <-- none
- // OUTPUT <-- value of the removed Node
- // EXCEPTION if queue is empty
- Node temp <-- front
- front <-- front.next
- temp.next <-- null
- return temp.value`

**Peek O(1)**

- When conducting a peek, you will only be inspecting the front Node of the queue.

- You would check isEmpty before conducting a peek. This will ensure that an exception is not raised. Alternately, you can wrap the call in a try/catch block.

**Here is the pseudocode for a peek**

- ALGORITHM peek()
- // INPUT <-- none
- // OUTPUT <-- value of the front Node in Queue
- // EXCEPTION if Queue is empty
- return front.value

*We do not re-assign the next property when we peek because we want to keep the reference to the next Node in the queue. This will allow the front to stay in the front until we decide to dequeue*

**IsEmpty O(1)**

**Here is the pseudocode for isEmpty**

- ALGORITHM isEmpty()
- // INPUT <-- none
- // OUTPUT <-- boolean
- return front = NULL