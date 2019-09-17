# Dinamic array

dinamic arrays are the data stucture which can grouw on its size as the input element size increases.

C#,python --> List;

Java --> ArrayList;

C++ --> std::vector;

## C# implimentations

### Size: 8 --> 4,2,4,5,6,7,8,8,_,_,_ ---->>> full

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

  #### complexity analysys 

  lets Assume N elements in the chain

  gettting haed and tail is easy O(1);
  Finding a specific element O(N);
  Insertion if we already found the element O(N);
  Deleting O(N); 

# Priority queue
