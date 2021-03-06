# Overview

## Explanation

- ![must-have][must-have] means __must do__ question, that includes many key points;
- ![recommended][recommended] means __good question__, that is quite clear and enjoyable;
- ![easy][easy] means __this is easy__ for me, that there might only be no fancy things;
- ![medium][medium] means __this is medium__ for me, that there is at least one important thing;
- ![hard][hard] means __this is hard__ for me, that it's hard to code;
- ![star][star] means __how many times I've done__ for this question;
- ![freq][freq] means __this is frequently asked__ in interviews.

## Outline

- LinkedList
  - Dummy node
- Array
  - Subarray
  - Sorted array

## Methodology

- LinkedList
  - **Add dummy node when the head of the list will change. So dummy node is used to preserve the head node**
    - Use `head = dummy` to include dummy node into your algorithms.
    - 90% of linked list questions have used **dummy node**, because most questions will actually change the original structure of the list.
  - First think about a general solution, and define APIs (input and output parameters for methods).
  - Think about what information we need to keep (normally it's dummy node). **Include all nodes that are affected in a same method.**
    - Adding a dummy node before the head node, and reset the head node as dummy node. In this way, we regard the dummy node as a part of the whole list.
    - We do need to include dummy node, but we will never run our algorithms on dummy node, it's just used to maintain a link to head node. Because dummy node is based on this **unchanged** rule, so we can do whatever we want on nodes behind dummy.
    - Provide an example about a question that must use dummy node, **not just copy a head node.** Then it should be [MergeTwoSortedLists](MergeTwoSortedLists.md).
  - Pointer movement questions: use slow and fast pointers.

## Category

- LinkedList
  - Question list
    - [InsertIntoCyclicSortedList](InsertIntoCyclicSortedList.md) ![medium][medium] ![must-have][must-have] ![star][star]
    - [MergeTwoSortedLists](MergeTwoSortedLists.md) ![easy][easy] ![must-have][must-have] ![star][star]
    - [ReverseLinkedList](ReverseLinkedList.md) ![easy][easy] ![must-have][must-have] ![star][star]
    - [ReverseLinkedList2](ReverseLinkedList2.md) ![hard][hard] ![star][star]
    - [RotateList](RotateList.md) ![hard][hard] ![must-have][must-have] ![recommended][recommended] ![star][star]
    - [ReorderList](ReorderList.md) ![hard][hard] ![must-have][must-have] ![recommended][recommended] ![star][star]
    - [ReverseNodesInKGroup](ReverseNodesInKGroup.md) ![hard][hard] ![recommended][recommended] ![must-have][must-have] ![star][star]
    - [PartitionList](PartitionList.md) ![easy][easy] ![recommended][recommended] ![star][star]
    - [LinkedListCycle](LinkedListCycle.md)
- Array
  - Subarray
    - [SubarraySum](SubarraySum.md) ![medium][medium] ![must-have][must-have] ![recommended][recommended] ![star][star]
    - [MaximumSubrray](MaximumSubrray.md) ![easy][easy] ![must-have][must-have] ![star][star]
    - [CopyListWithRandomPointer](CopyListWithRandomPointer.md) ![easy][easy] ![star][star]
    - [SubarraySumClosest](SubarraySumClosest.md) ![hard][hard] ![must-have][must-have]
    - [SortList](SortList.md) ![hard][hard] ![must-have][must-have]
  - Pointer
    - [MedianOfTwoSortedArrays](MedianOfTwoSortedArrays.md) ![hard][hard] ![star][star]

## Notes

- LinkedList
  - More temporary variables means a more clear program.
  - Don't use one variable name to denote multiple meanings.
- Dummy node will not change its position.
- `while (pos < num)`, so at the end, the condition should be `pos == num`.
- Just think the dummy node as a node whose `index` is 0.
- Normally we would choose `ListNode temp = head.next` to cache a temporary value before we change `head.next`;
- The `count = 0` in **count < length / 2** is based on dummy node, which means the starting node should be dummy node.
- Sorting algorithms
  - Heap sort
  - Merge sort
  - Quick sort
- Array
  - Partition is always the hardest part for me, but it is a common problem in array category.

[must-have]: https://jaywcjlove.github.io/sb/ico/min-bibei.svg
[recommended]: https://jaywcjlove.github.io/sb/ico/min-tuijian.svg
[easy]: https://jaywcjlove.github.io/sb/ico/min-free.svg
[medium]: https://jaywcjlove.github.io/sb/ico/min-oss.svg
[hard]: https://jaywcjlove.github.io/sb/ico/min-hot.svg
[freq]: https://jaywcjlove.github.io/sb/ico/min-app-store.svg
[star]: https://jaywcjlove.github.io/sb/star/red.svg
[star0]: https://jaywcjlove.github.io/sb/star/red0.svg
[star1]: https://jaywcjlove.github.io/sb/star/red1.svg
[star2]: https://jaywcjlove.github.io/sb/star/red2.svg
[star3]: https://jaywcjlove.github.io/sb/star/red3.svg
[star4]: https://jaywcjlove.github.io/sb/star/red4.svg
[star5]: https://jaywcjlove.github.io/sb/star/red5.svg