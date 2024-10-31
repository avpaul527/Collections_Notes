# Java Collections Notes
- A unified architecture for representing and manipulating collections.
- Provides interfaces, implementations, and algorithms to work with groups of objects.

## Core Interfaces
- Collection: Root interface for all collections.
 - Subinterfaces include Set, List, and Queue

- List: An ordered collection (also known as a sequence). Allows duplicates.
 - ArrayList, LinkedList, Vector

- Set: A collection that does not allow duplicate elements.
 - HashSet, LinkedHashSet, TreeSet

- Map: An object that maps keys to values. Keys must be unique.
 - HashMap, LinkedHashMap, TreeMap

- Queue: A collection designed for holding elements prior to processing.
 - PriorityQueue, LinkedList (also implements Queue)

## Common Implementations
- ArrayList: Resizable array implementation of the List interface. Provides fast random access.
- LinkedList: Doubly linked list implementation. Efficient for insertions and deletions.
- HashSet: Implements Set using a hash table. Offers constant time performance for basic operations.
- TreeSet: Implements Set using a red-black tree, ensuring elements are sorted.
- HashMap: Implements Map using a hash table. Offers constant time complexity for basic operations.
- TreeMap: Implements Map using a red-black tree, keeping keys in sorted order.
## Utility Classes
- Collections: Contains static methods for operating on collections
- Arrays: Provides static methods for manipulating arrays 
- Sorting, searching, etc.

## Key Operations
- Insertion: Adding elements to a collection
- Deletion: Removing elements from a collection
- Traversal: Iterating over elements in a collection
- Sorting: Ordering elements in a specific sequence

## Iterators
- Provide a way to access elements of a collection sequentially without exposing its underlying structure.
- Types:
 - Iterator: Can traverse elements and remove elements during traversal.
 - ListIterator: Extends Iterator to allow bidirectional traversal of lists

## Performance Considerations
- Different collections have varying performance characteristics for different operations.
- Choose the right collection based on:
 - Size of the data
 - Frequency of operations (insertion, deletion, access)
 - Order requirements (sorted vs. unsorted).

## Concurrency
- Java Collections Framework does not provide synchronized collections. Use Collections.synchronizedCollection or ConcurrentHashMap for thread-safe operations.

## Generics
- The Collections Framework supports generics, allowing for type-safe collections.

## Java 9 Enhancements
- New factory methods for creating immutable lists, sets, and maps (List.of(), Set.of(), Map.of())
