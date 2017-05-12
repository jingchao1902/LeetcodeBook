# Overview

## Explanation

- ![must-have][must-have] means __must do__ question, that includes many key points;
- ![recommended][recommended] means __good question__, that is quite clear and enjoyable;
- ![easy][easy] means __this is easy__ for me, that there might only be no fancy things;
- ![medium][medium] means __this is medium__ for me, that there is at least one important thing;
- ![hard][hard] means __this is hard__ for me, that it's hard to code;
- ![star][star] means __how many times I've done__ for this question;
- ![freq][freq] means __this is frequently asked__ in interviews.

## When to use DFS

- Find all possible permutations or combinations.
- Non-recursion with stack.

## Comparsion with BFS

- In BFS, each node has a uniform rule to get its neighbors. But often DFS doesn't have such rule. Sometimes you need to consider other constraints, like __Subsets__ question. But it can still be solved by BFS.
- It's hard to pass information like __ArrayList__ from last level to next level in BFS to build some path. But it's easier to do in DFS since it's using recursion, and it has backtracking to return information even from low level to hight level.
- Why we need to use DFS not BFS sometimes ?
  - The interviewer wants to see that you can write recursion.
  - BFS is complicated for some kind of questions.
  - DFS can save a lot of memory, since it doesn't need to store previous state.

## Category

- Binary tree
  - Process node after poll or after offer (__it depends ?__).
  - Question list
    - [Level order](LevelOrderTraversal.md) ![star][star]
    - [BinaryTreeSerialization](BinaryTreeSerialization.md) ![star][star]
- Graph
  - Use "visited" set to avoid loops, no matter the graph is directed or undirected.
  - Build [all graph nodes first](CloneGraph.md) and store them into a list, and then it's easier to process.
  - Use `Map<Integer, Set<Integer>>` or graph node (__can we use graphnode ?__) to store a graph.
  - Question list
    - [SearchGraphNodes](SearchGraphNodes.md) ![star][star]
    - [GraphValidTree](GraphValidTree.md) ![recommended][recommended] ![star][star]
    - [CloneGraph](CloneGraph.md) ![must-have][must-have] ![star][star]
    - [TopologicalSorting](TopologicalSorting.md) ![must-have][must-have] ![star][star]
    - [CourseSchedule](CourseSchedule.md) ![star][star]
    - [CourseSchedule2](CourseSchedule2.md) ![star][star]
    - [SequenceReconstruction](SequenceReconstruction.md) ![must-have][must-have] ![star][star]
- 2D matrix
  - Regarded as an undirected matrix graph.
  - The 2D matrix plays the role as the HashMap in a graph, which contains information about neighbors for a node.
  - Question list
    - [NumberofIslands](NumberofIslands.md) ![recommended][recommended] ![star][star]
    - [BuildPostOffice2](BuildPostOffice2.md) ![recommended][recommended] ![must-have][must-have] ![star][star]

## Time complexity

- O(numer of answers * time spent on each answer)

## Notes

- DFS has __backtracking__ nature.
- For BFS, the "visited" set must ensure that every node will only be offered into the queue for once!!!
- [Divide a complicated question into several parts](CloneGraph.md), and write them as separate methods. Because during interview, we might not have enought time to implement every detail, so we need to implement most significant methods first.
- Remember to check if this node is valid before offering it to the queue.
- Remember to initializa root node.
- Learn to use global variables and constant values to make code clear.
  - For example, use m to represent number of rows, and n to represent number of columns.
- A most complete BFS algorithm includes three parts:
  - while(!queue.isEmpty())
  - for each node in current level
  - for each neighbor in current node

## Appendix

![](https://farm5.staticflickr.com/4187/34570613476_9a817f1255_o.jpg)

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