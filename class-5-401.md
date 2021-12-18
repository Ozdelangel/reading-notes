Linked List
Is a sequence of Nodes that are connected/linked to each other. The most defining feature of a linked list is that each Node references the next node in the link.
There are two types singly and doubly
Singly - singly refers to the number of references the node has a singly linked list means that there is only one reference and the reference points to the next node.
Doubly - doubly refers to there being double references within the node. Doubly linked list means that there is a reference to both the next and previous node.
Node - nodes are the individual items/links that live in a linked list. Each node contains the data for each link
Next - each node contains a property called next. This property contains the reference to the next node
Head - the head is reference to the first node in the linked list
Current - the current is a reference of type node to the node that is currently being looked at. When you are going through you create a new current variable at the head to guarantee you are starting from the beginning of the linked list

Travel 
You are not able to use a for each a for loop
Depends on the next value
Best way is a while loop it continually checks the next node in the list
Directions for traversal 
We are first creating current at the head to guarantee we are starting from the beginning
We are creating a while loop. This loop will only run if the node at the current is pointing to is not null
Once we are in the while loop we are checking if the value of the current node is equal to the value we are looking for. If its true then we have found what we are looking for.
If the current node does not contain the value we are looking for we then must move current to the next node that is being referenced.
The while loop keeps going steps three and four get repeated until the current reaches the end

Adding a node
Order is important make sure each link and node are properly assigned
Instatiate the new node that we are adding the values will be passed in add method as arguments
Newnode.next by default is set to null. We want to set newnode.next propert to the same location that the head node is point towards because hea is just a reference type we will be assigning it to the same allocations in memory as the  node it is point to
