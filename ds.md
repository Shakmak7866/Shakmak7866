
# Table of Contents

1.  [Linked Lists](#org31abf92)
    1.  [Nodes](#orgef724f2)
    2.  [Head and Tail](#orgb541054)
        1.  [Head node](#org6f19028)
        2.  [Tail node](#org6d0a643)
    3.  [Iterating through the list](#org295f745)
    4.  [Different types of LinkedLists](#orgbe84b42)
        1.  [Doubly-Linked List](#org36e68f4)
        2.  [Circly-Linked List](#org6f1284b)
    5.  [Key facts about LinkedList to keep in mind](#org8cd4da0)
    6.  [Methods for Linked Lists](#orge306660)
        1.  [set()](#org3ed4936)
        2.  [get()](#orgbf94c5b)
        3.  [append()](#orgbdc76f5)
        4.  [add()](#org854871a)
        5.  [remove()](#org0129e3f)
        6.  [search()](#org25a35db)
        7.  [isEmpty() [Optional]](#org752d1cf)



<a id="org31abf92"></a>

# Linked Lists

-   An abstract data type that consistes of nodes
-   The nodes are connected via pointers and are dynamically allocated
-   The idea of this is kind of like a treasure hunt
-   Acts as a replacement for a list using an array
-   You can create a size variable to keep track of the size of the list


<a id="orgef724f2"></a>

## Nodes

-   Nodes work as an object that usually contains two fields
    -   The data element containing the information that the node stores
    -   The next element which points to the next node
-   When the next element does not have a node to point to, it points to null
-   Best practice to create a static node class within the linkedlist class


<a id="orgb541054"></a>

## Head and Tail

-   Another key characteristic about linked lists is that they have a header node and a tail node
-   These nodes can either be a reference to the desired node or a new node themselves


<a id="org6f19028"></a>

### Head node

-   A node that points to the beginning of the list


<a id="org6d0a643"></a>

### Tail node

-   A node that points to the end of the list


<a id="org295f745"></a>

## Iterating through the list

-   In an array, it would have indices and you would just increment the index
-   For linked list, you have to follow where the node goes
-   Given a header node, you find the next node via
    -   head.next
-   The node after that,
    -   head.next.next
-   If you want to go throught the whole list, it is easier to have a function like this

    Node curr = head;
    while (curr.next != null) {
            curr = curr.next;
    }


<a id="orgbe84b42"></a>

## Different types of LinkedLists


<a id="org36e68f4"></a>

### Doubly-Linked List

-   In this type of linked list, there is an additonal pointer that points to the previous node


<a id="org6f1284b"></a>

### Circly-Linked List

-   In this type of linked list, a latter node points to a previous node, creating a cycle
-   Usually, it can be thought of as the tail node pointing back to the head node


<a id="org8cd4da0"></a>

## Key facts about LinkedList to keep in mind

-   They are tiny blocks of memory linked together
-   There is no quick memory access
-   It requires extra memory to represnt compared to array
-   There are fewer expensive memory moves


<a id="orge306660"></a>

## Methods for Linked Lists


<a id="org3ed4936"></a>

### set()

-   Parameters:
    -   set(int index, Object obj<sub>of</sub><sub>choice</sub>)
-   Returns:
    -   Depends on the person writing the code


<a id="orgbf94c5b"></a>

### get()

-   Parameters:
    -   get(int index)
-   Returns:
    -   Returns the object at the index


<a id="orgbdc76f5"></a>

### append()

-   Parameters:
    -   append(Object obj<sub>of</sub><sub>choice</sub>)
-   Returns:
    -   Depends on the person writing the code


<a id="org854871a"></a>

### add()

-   Parameters:
    -   add(int index, Object obj<sub>of</sub><sub>choice</sub>)
-   Returns:
    -   Depends on the person writing the code


<a id="org0129e3f"></a>

### remove()

-   Possible Parameters:
    -   remove(int index)
    -   remove(Object obj<sub>of</sub><sub>choice</sub>)
-   Returns:
    -   Depends on the person writing the code


<a id="org25a35db"></a>

### search()

-   Parameters:
    -   search(Object obj<sub>of</sub><sub>choice</sub>)
-   Returns:
    -   Returns the index at which the object is found
    -   Or returns -1 if it is not found


<a id="org752d1cf"></a>

### isEmpty() [Optional]

-   No parameters needed
-   Returns:
    -   Returns a boolean
    -   True if empty or head.data == null
    -   False if not or head.data != null

