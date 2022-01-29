# Common Terminology 
Node - a Tree is a component which may contain it’s own values, and references other nodes
Root - The root is the node at the beginning of the tree
K - A number that specifies the maximum number of children any node may have in k- any tree. In a binary tree, `k = 2`
Left - A reference to one child node, in a binary tree
Right - A reference to the other child node, in a binary tree
Edge - The edge in a tree is the link between a parent and a child node
Leaf - A leaf is a node that does not have any children
Hieght - The height of a tree is the number of edges from the root to the furthest leaf


# Traversals
Traversing a tree allows us to search for a node
*there are two categories of traversals*
- Depth First
- Breadth First
# Depth First
- This means that we want to go through the height first
- There are three methods to carry out the traversal
- Each methods changes the order in which we print the root
### Pre-order: root > left >right
### In-order: left > root > right
### Post-order left > right > root

Pre-order means that the root has to be locked at first. In our case, looking at the root just means that we output its value. When we call pre_order for the first time, the root will be added to the call stack.

Then we start reading our pre_order function’s code from top to bottom. The first line of code reads this:

Root.value
This means that we will output the root value out to the console. Then, our next block of code instructs us to check if our root has a left node set. If the root does, we will then send the left node to our pre_order method recursively. This means that we make another function call, where B is our new root

The process keeps going recursively until we reach our leaf.


# notes about this 
- The program will look for both a root.left and a root.right. Both return none so it will end the execution of that method call.
- D will pop off the call stack and the root will be reassigned back to B
- This is the heart of recursion: when we complete a function call, we pop it off the stack and are able to continue execution through previous function call.
- The code bleck will now pick up where it left off when b was the root. Since it already looked for root.left, it will now look for root.right
- E will output to the console. Since E is a leaf, it will complete the method code block, and pop E off of the call stack and make its way back up to B.
- In the function call, B has already checked for root.left and root.right. There no further lines of code to execute so B will be popped off the call stack. So that we can resume execution of A


# Breadth First
Breadth first traversal iterates through the tree by going through each level of the tree node by node. 

So you will put the root into the queue

Now that we have one node in our queue we can dequeue it and use that node in our code

And then we can enqueue the left and right chile in that order

This leaves us with b as the new front of our queue. We can then repeat the process we did with A Dequeue the front node, enqueue that node left and right nodes and move to the next new front of the queue.

Now our front is C, so we can repeat the dequeue + enqueue children process

And we continue onwards when we reach a node that doesn’t have any children, we just dequeue it without any further enqueue


# Binary Tree Vs k-ary Trees

In the previous examples we used a Binary Tree. Trees can have any number of children per node, but Binary Trees restrict the number of children to two (hence our left and right children)

## K-aryy Trees
If nodes are able to have more than 2 child nodes, we call the tree that contains them a k-ary Tree. in this type of tree we use k to refer to the maximum number of children that each node is able to have


## breadth first traversal

Traversing a K-ary tree requires a similar approach to the breadth first traversal. We are still pushing nodes into a queue, but we are now moving down a list of children of length k, instead of checking for the presence of a left and a right child

If we traversed this tree Breadth First we should see the output 
Abcdefgh


We will still start at the root node and we will add it to out queue

Much like before, as long as we have a node in our queue we can dequeue

With every node we dequeue, we check it’s list of our children and dequeue each one

Once these are queued up, can move on to node b at the front of the queue, which we can dequeue followed by enqueing node b’s children

This process of dequeuing and processing the nodes at the front of the queue, followed by enqueing the current node’s children continues until our queue is empty of child nodes
