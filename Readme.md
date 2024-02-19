What is a linked list, and why is it useful?
    A linked list is a bunch of nodes, each of which is connected to either the next node, or both the next and previous node, and each node only appears once in the list.
In what scenarios is a linked list more efficient for finding specific data, and in what scenarios is it more efficient for adding new data compared to other data structures like arrays or dynamic arrays (e.g., List in C#)?
    Linked lists are very good for sequential reads, or for adding/reading items to the start and, in a doubly linked list, the end. It is also generally faster to add items to a linked list, as the only data that
    needs to be changed is in two nodes, instead of having to rewrite all data.
What is the importance of proper referencing of nodes in a linked list, and what potential issues can arise from improper referencing?
    Proper node referencing is essential in a linked list, if any error is made, the list will loop, or end prematurely.
Critical Thinking: What software or systems might benefit from using a Linked List, a system that is slow to search for something, but quick to add.
    I don't know right now. The first thing that comes to mind is some sort of archival system, where it may never be read from, but the structure of a linked list makes it very vulnerable to data loss compermising
    the whole structure, and it is not suited for use in permanent storage. It might be handy in some sort of framebuffer or game development context, where over the course of a frame, data is added to it, and is
    only read once to display it. It would probably be better for that SHMUP I was working on a few months ago.
Follow Up: Which system would it be more beneficial to use a List or Array, where all the data is grouped together for easy searching, but slow to add?
    Pretty much any kind of database or similar scenario.
Any thoughts for combining the two to make it really efficient?
    Multiple locations other than just the head and tail can be stored, for easy acess to the middle of the list. This, along with multithreading, could be used to make searches much faster.
