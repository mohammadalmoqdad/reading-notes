# Linked List

## What is a Linked List?
  - A Linked List is a sequence of Nodes that are connected/linked to each other. The most defining feature of a Linked List is that each Node references the next Node in the link.

  ## Types of it :
  1. *Singly* - Singly refers to the number of references the node has. A Singly linked list means that there is only one reference, and the reference points to the Next node in a linked list
  2. *Doubly* - Doubly refers to there being two (double) references within the node. A Doubly linked list means that there is a reference to both the Next and Previous node.

* *When traversing a linked list, you are not able to use a foreach or for loop*.

## code exaple: 
` ALGORTIHM Includes (value)
		// INPUT <-- integer value
		// OUTPUT <-- boolean
			Current <-- Head
			WHILE Current is not NULL
				IF Current.Value is equal to value
					return TRUE

				Current <-- Current.Next

			return FALSE `

* **Linked list** are Linear data structures which means that there is a sequence and an order to how they are constructed and traversed and in order to get to the end of the list, we have to go through all of the items in the list in order, or sequentially. Linear structures, however, are the opposite of non-linear structures.
 
