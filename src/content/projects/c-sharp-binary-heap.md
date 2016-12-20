+++
date = "2016-12-20T14:12:31+11:00"
title = "C# Binary Heap"
draft = false

+++

A simple class for a binary heap (AKA Priority Queue). Supports the following operations:

## Heap

| Function                       | Time complexity |
| ------------------------------ |:---------------:|
| void **Insert**(T Item);       | O(log(n))       |
| T **Extract**();               | O(log(n))       |
| bool **Remove**(T item);       | O(n)       |
| bool **Contains**(T item);     | O(n)       |
| T **Peek**();                  | O(1)       |

`DictionaryHeap` is the same as `Heap` but improves on the running time on methods `Remove()` and `Contains()` at the expense of holding a dictionary in memory.

## DictionaryHeap

| Function                       | Time complexity |
| ------------------------------ |:---------------:|
| bool **Remove**(T item);       | O(log(n))       |
| bool **Contains**(T item);     | O(1)       |


# Example:
A simple one to start off:

    IHeap<int> heap = new Heap<int>(Comparer<int>.Default);
    heap.Insert(4);
    heap.Insert(-25);
    heap.Insert(2523);
    heap.Insert(1);

    heap.Extract(); // Returns -25
    heap.Extract(); // Returns 1
    heap.Extract(); // Returns 4
    heap.Extract(); // Returns 2523
    heap.Extract(); // Throws InvalidOperationException

Note:  `Heap` can be changed to `DictionaryHeap`.

A little more involved

    class NodeComparer : Comparer<Node>
    {
        public override int Compare(Node n1, Node n2)
        {
            return n1.Cost - n2.Cost;
        }
    }

    class Node
    {
        public int Cost { get; private set; }

        public Node(int cost)
        {
            this.Cost = cost;
        }
    }

    using HoangPaul.Heap;

    IHeap<Node> heap = new DictionaryHeap<Node>(new NodeComparer());
    Node n = new Node(4);
    heap.Insert(n);
    heap.Insert(new Node(1));
    heap.Insert(new Node(0));
    heap.Insert(new Node(5));

    Console.WriteLine(heap.Count);  // 4

    heap.Contains(n);               // Returns true
    heap.Remove(n);                 // Returns true
    heap.Contains(n);               // Returns false
    heap.Remove(n);                 // Returns false

    Console.WriteLine(heap.Count);  // 3

    heap.Extract();                 // Returns node with cost 0
    heap.Extract();                 // Returns node with cost 1
    heap.Extract();                 // Returns node with cost 5
    heap.Extract();                 // Throws InvalidOperationException

