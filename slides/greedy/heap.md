---
title: Heap
theme: solarized
---
# heap
----
* tree-like data structure
* (max) *heap invariant*
  * root of heap > all children
  * all children are (max) heaps
----
* heap has:
  * `push`: append and item to heap while maintaining heap invariant
  * `top`: inspect value of root
  * `pop`: remove and return root from heap while maintaining heap invariant
----
```mermaid
graph TD
5((5))
4((4))
3((3))
2((2))
5 --- 2
5 --- 4
4 --- 3
```
# add 6

```mermaid
graph TD
5((5))
4((4))
3((3))
2((2))
6((6))
5 --- 2
5 --- 4
4 --- 3
4 --- 6
```
----
```mermaid
graph TD
5((5))
4((4))
3((3))
2((2))
6((6))
5 --- 2
5 --- 4
4 --- 3
4 --- 6

classDef recursive fill:#fc1313
class 2,4 recursive
```
----
```mermaid
graph TD
5((5))
4((4))
3((3))
2((2))
6((6))
5 --- 2
5 --- 6
6 --- 3
6 --- 4
```
----
```mermaid
graph TD
5((5))
4((4))
3((3))
2((2))
6((6))
5 --- 2
5 --- 6
6 --- 3
6 --- 4
```