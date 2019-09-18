# Dinamic array

dinamic arrays are the data stucture which can grouw on its size as the input element size increases.

C#,python --> List;

Java --> ArrayList;

C++ --> std::vector;

## C# implimentations

### Size: 8 --> 4,2,4,5,6,7,8,8,_,_,\_ ---->>> full

    case 1 : Adding a new element in will not be depends on the size of array or nor the number of element in the array hence the worst case coplexity will in general be the constant as O(1);

    case 2 : Array is full -->> Size: 8 --> 4,2,4,5,6,7,8,8,8 ---->>> full when add a new element we need to increase the size comonly by 1.5 but the range is 1 to 2 and also need to copy all elements in new array in this case the worst case complexity is O(N) however this is in general done in the alrta fast memory meme cache but can be in slower case like taps and megnatic hard drives etc.

    for removing an element --> O(N);
    for searching also ----> O(N);

###

# Hash table

# Linked List

## C#, JAVA --> LinkedList

## C++ std::list

## python collections.deque

In linked list elemenst are stores in independent blocks of elements each element is a container with a pointer to the next container (Doubly link list if it has a pointer to the pervious container too) it also have a entry point container with head and tail pointers.

\*\* need to do the application of these stuff and add a performance mejore tool too.

#### complexity analysys

lets Assume N elements in the chain

gettting haed and tail is easy O(1);
Finding a specific element O(N);
Insertion if we already found the element O(N);
Deleting O(N);

# Priority queue

C# : C5.IntervalHeap
Java : PriorityQueue
python : heapq
c++ : std::priority_queue

it is a queue where elements add in back and remove from the frount the difference is it mantain order internally and the ordaring is completely tranformed to the progarmmer internally element is organized in the dataSttructure "Heap"

### HEAP

there are folling kinds of heaps

1). Min heap 2).Max Heap 3).Min-max heap 4).Intervel heap

### Min Heap

a heap is a binary balanced tree structure where each node have atmost 2 childreans
The Rule::
1). Each elements must be smaller to their most immidiate childrens.
2). elemets must store from the left to rigth in a dinamic array.
3). This array is organize in succha way that if an element is in posission k;
then ,
LeftChild = 2k; rigthChild = 2k + 1;
\*\* to get a minimum will always in the top hence the wort case comlexity will be O(1);

#### Insertions -

1). add to the left most possittion
2). rearrange the tree with the rule (1).

For total number of element N the lavels will be (Logb2N).

the worst case colplexity will be O(logb2N);
Noted here the swapping of the elements is independent of the total number of elements N in tree but may need to perform it each level of tree L.

#### Removal of min element -

1). remove from the top.
2). put last element on the top.
3). Repeat to follow the heap rule.
