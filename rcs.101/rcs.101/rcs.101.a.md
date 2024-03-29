---
cover: ../.gitbook/assets/Group 9 (2).png
coverY: 0
layout:
  cover:
    visible: true
    size: full
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# RCS.101.a

{% tabs %}
{% tab title="Map of Contents" %}
<figure><img src="../.gitbook/assets/image (26).png" alt=""><figcaption><p>RCS.101.a</p></figcaption></figure>
{% endtab %}

{% tab title="Basic Stack & Basic DFS" %}
{% embed url="https://www.youtube.com/watch?index=2&list=PLskIq2MzopHCU6IAoYtedpzOzgWItmmQI&v=n_-u4Q-OZBE" %}
\[RCS.101 x Miters] Basic Stack & DFS
{% endembed %}
{% endtab %}

{% tab title="Queue & Basic BFS" %}
{% embed url="https://www.youtube.com/watch?index=3&list=PLskIq2MzopHCU6IAoYtedpzOzgWItmmQI&v=XiiYd4p8Fa0" %}
\[RCS.101 x Miters] Queue & BFS
{% endembed %}
{% endtab %}

{% tab title="Binary Search" %}
{% embed url="https://www.youtube.com/watch?index=4&list=PLskIq2MzopHCU6IAoYtedpzOzgWItmmQI&v=uVsU5vuDDS8" %}
\[RCS.101 x Miters] Binary Search
{% endembed %}
{% endtab %}
{% endtabs %}

## Basic Stack

{% hint style="info" %}
Stack 是電腦科學中最為基礎的資料結構，擁有 LIFO (Last In, First Out) 的特性。

* Learning Material
  * [**Comp Sci in 5: Stacks**](https://www.youtube.com/watch?v=\_7Z07tI-xrA)
  * [**LC Explore: Queue & Stack**](https://leetcode.com/explore/learn/card/queue-stack/)
  * [**Core Dumped: WHY IS THE STACK SO FAST?**](https://www.youtube.com/watch?v=N3o5yHYLviQ)
{% endhint %}

* Practices
  *   [ ] 題目：**E** [**495 · Implement Stack**](https://www.lintcode.com/problem/495)

      OJ：**E** [**225. Implement Stack using Queues**](https://leetcode.com/problems/implement-stack-using-queues/) (支援的語言較多
  * [ ] **E** [**423 · Valid Parentheses**](https://www.lintcode.com/problem/423/) or [**20. Valid Parentheses**](https://leetcode.com/problems/valid-parentheses/)\
    (note: description from LC is imperfect, should tell `[(]): false`)
  * [ ] **M** [**1001 · Asteroid Collision**](https://www.lintcode.com/problem/1001/description)
* Graduation Challenge
  * [ ] **M** [**268 · Parentheses Score**](https://www.lintcode.com/problem/268/)

***

## Basic DFS

* Prerequisite
  * [#basic-stack](rcs.101.a.md#basic-stack "mention")
* Learning Material
  * [**Preorder Traversal**](https://faculty.cs.niu.edu/\~mcmahon/CS241/Notes/Data\_Structures/binary\_tree\_traversals.html)
  * [**Inorder Traversal**](https://faculty.cs.niu.edu/\~mcmahon/CS241/Notes/Data\_Structures/binary\_tree\_traversals.html)
  * [**Postorder Traversal**](https://faculty.cs.niu.edu/\~mcmahon/CS241/Notes/Data\_Structures/binary\_tree\_traversals.html)
* Practices
  * [ ] **E** [**94. Binary Tree Inorder Traversal**](https://leetcode.com/problems/binary-tree-inorder-traversal/)
  * [ ] **E** [**144. Binary Tree Preorder Traversal**](https://leetcode.com/problems/binary-tree-preorder-traversal/)
  * [ ] **E** [**145. Binary Tree Postorder Traversal**](https://leetcode.com/problems/binary-tree-postorder-traversal/)
* Graduation Challenge
  * [ ] **M** [**230. Kth Smallest Element in a BST**](https://leetcode.com/problems/kth-smallest-element-in-a-bst/)
  * [ ] **M** [**690. Employee Importance**](https://leetcode.com/problems/employee-importance/)

{% hint style="warning" %}
Appendix: 3rd way the traverse a binary tree other than stack or recursion

* Learning Material
  * [**解法三 Morris Traversal**](https://leetcode.wang/leetCode-94-Binary-Tree-Inorder-Traversal.html)
  * [**CPP Morris Traversal**](https://leetcode.com/problems/binary-tree-inorder-traversal/solutions/148939/CPP-Morris-Traversal/)
  * [**L37. Morris Traversal | Preorder | Inorder | C++ | Java**](https://www.youtube.com/watch?v=80Zug6D1\_r4)
* Practices
  * [ ] **M** [**114. Flatten Binary Tree to Linked List**](https://leetcode.com/problems/flatten-binary-tree-to-linked-list/) (expecting pre-order outcome
  * [ ] **M** [**915 · Inorder Predecessor in BST**](https://www.lintcode.com/problem/915) (implement using Morris Traversal
  * [ ] **M** [**430. Flatten a Multilevel Doubly Linked List**](https://leetcode.com/problems/flatten-a-multilevel-doubly-linked-list/) (conceptually similar
{% endhint %}

***

## Queue

{% hint style="info" %}
Queue 是電腦科學中基礎的資料結構，擁有 FIFO (First In, First Out) 的特性。

與現實中的排隊概念接近，Message Queue 則是 Infrastructure 版本的實現。

* Learning Material
  * [**Comp Sci in 5: Queues**](https://www.youtube.com/watch?v=-1oFihNj6Vw)
  * [**LC Explore: Queue & Stack**](https://leetcode.com/explore/learn/card/queue-stack/)
{% endhint %}

* Practices
  * [ ] 題目：**E** [**492 · Implement Queue by Linked List**](https://www.lintcode.com/problem/492)\
    OJ：**E** [**232. Implement Queue using Stacks**](https://leetcode.com/problems/implement-queue-using-stacks/) (支援的語言較多
  * [ ] **E** [**1700. Number of Students Unable to Eat Lunch**](https://leetcode.com/problems/number-of-students-unable-to-eat-lunch/)
  * [ ] **E** [**2073. Time Needed to Buy Tickets**](https://leetcode.com/problems/time-needed-to-buy-tickets/)
* Graduation Challenge
  * [ ] **M** [**950. Reveal Cards In Increasing Order**](https://leetcode.com/problems/reveal-cards-in-increasing-order/)

***

## Basic BFS

{% hint style="info" %}
BFS is the first relatively advanced, yet power algorithm we get to study.

We start by introducing the essence of BFS via the classic **Binary Tree Level Order Traversal**.

Once your done with the basic understanding. Combing BFS with the knowledge of [#hash-map](rcs.101.b.md#hash-map "mention") and [#basic-graphs](rcs.101.c.md#basic-graphs "mention"), you'll now able to bridge yourself into the challenging-yet-exciting **Shortest Path Finding** problems.

* Learning Material
  * **Binary Tree BFS**
    * [ ] [**Level Order Traversal**](https://faculty.cs.niu.edu/\~mcmahon/CS241/Notes/Data\_Structures/binary\_tree\_traversals.html)
    * [ ] **M** [**102. Binary Tree Level Order Traversal**](https://leetcode.com/problems/binary-tree-level-order-traversal/)
  * **(Unweighted, Undirected) Graph BFS**
    * [ ] [**Shortest Path in a Binary Matrix - LeetCode 1091 - Python**](https://www.youtube.com/watch?v=YnxUdAO7TAo)
    * [ ] [**Breadth First Search - Finding Shortest Paths in Unweighted Graphs**](https://www.youtube.com/watch?v=T\_m27bhVQQQ)
    * [ ] **M** [**1091. Shortest Path in Binary Matrix**](https://leetcode.com/problems/shortest-path-in-binary-matrix/)
{% endhint %}

* Prerequisite
  * [#queue](rcs.101.a.md#queue "mention")
  * [#hash-map](rcs.101.b.md#hash-map "mention")
  * [#basic-graphs](rcs.101.c.md#basic-graphs "mention")
* Practices
  * [ ] **M** [**854 · Closest Leaf in a Binary Tree**](https://www.lintcode.com/problem/854/) (tricky)
  * [ ] **M** [**1302. Deepest Leaves Sum**](https://leetcode.com/problems/deepest-leaves-sum/)&#x20;
* Graduation Challenge
  * [ ] **M** [**3719 · Shortest Path to Get Bubble Tea**](https://www.lintcode.com/problem/3719)
  * [ ] **M** [**103. Binary Tree Zigzag Level Order Traversal**](https://leetcode.com/problems/binary-tree-zigzag-level-order-traversal/)

***

## Binary Search

{% hint style="info" %}
Binary Search/Bisection Search is one of the fundamental algorithms in Computer Science. It describes the process of searching for a specific value in an ordered collection.

Still, it's one of the must error-prone DSA in implementing.&#x20;

Not only it's tricky to get right, it's also hard to comprehend one's binary search implementation without context.
{% endhint %}

{% hint style="success" %}
#### Learning Material

* [**Binary Search - A Different Perspective**](https://www.youtube.com/watch?v=tgVSkMA8joQ) (introduces the concept of partitioning)
* [**Binary Search tutorial (C++ and Python)**](https://youtu.be/GU7DpgHINWQ?si=jGV8lyrvyN4XEdvF\&t=198)
* [**The 3 Levels of Binary Search**](https://www.youtube.com/watch?v=nuN3-AkykfM\&t=1081s)



1. Understanding **Binary Tree**'s fundamentals & applications.
   * [ ] **E** [**278. First Bad Version**](https://leetcode.com/problems/first-bad-version/)
2. Learn the classic **"Find Index of Given Target from Sorted Array"** problem & implementing it.
3. Elevate your understanding, think binary search in the terms of **"Partitioning"** from now on. Then using this to deconstruct a few other ppl's code.
{% endhint %}

{% hint style="success" %}
#### Summary

Binary Search can applied to the follow problem types



#### Type A - <mark style="color:green;">Searching for Target Deemed to Exist / Not-Exist</mark>

> * Conceptually similar to [**Template I**](https://leetcode.com/explore/learn/card/binary-search/125/template-i/938/)
> * [**Binary Search tutorial (C++ and Python) 3:18**](https://youtu.be/GU7DpgHINWQ?si=jGV8lyrvyN4XEdvF\&t=198)
> * [**Finding the Pivot in a Rotated and Sorted Array Using Binary Search in C++**](https://medium.com/@utkarsh.gupta0311/finding-the-pivot-in-a-rotated-and-sorted-array-using-binary-search-in-c-fdac97e566ce)

* [ ] **E** [**704. Binary Search**](https://leetcode.com/problems/binary-search/) (implement via [**Template I**](https://leetcode.com/explore/learn/card/binary-search/125/template-i/938/))
* [ ] **E** [**3621 · Fixed Point**](https://www.lintcode.com/problem/3621/description)



#### Type B - <mark style="color:green;">Approximation Narrowing</mark> (Recursive / Divide and Conquer)

> * There could be no exact value to locate. While having to recognise the closest target(s). High likelihood having to memorisation (variable for candidate values), also there might not be a finite list given upfront.
> * [**Binary Search tutorial (C++ and Python) 6:27**](https://youtu.be/GU7DpgHINWQ?si=CDuSwhe\_mWrWSuHo\&t=387)

* [ ] **E** [**69. Sqrt(x)**](https://leetcode.com/problems/sqrtx/)
* [ ] **M** [**875. Koko Eating Bananas**](https://leetcode.com/problems/koko-eating-bananas/)
* [ ] **M** [**34. Find First and Last Position of Element in Sorted Array**](https://leetcode.com/problems/find-first-and-last-position-of-element-in-sorted-array/)
* [ ] **M** [**33. Search in Rotated Sorted Array**](https://leetcode.com/problems/search-in-rotated-sorted-array/) (find [Pivot Point](https://www.ideserve.co.in/learn/find-pivot-in-a-sorted-rotated-array) with type B first , then do a type A search)



#### Type C - <mark style="color:green;">Partitioning</mark> ( <mark style="color:purple;">TTT</mark> | # | <mark style="color:red;">??FF</mark> )

> * Can be conceptualised using partitioning. (think in terms of ranges and anchors, not necessary indices)

* [ ] **M** [**162. Find (local) Peak Element**](https://leetcode.com/problems/find-peak-element/)
* [ ] **E** [**35. Search Insert Position**](https://leetcode.com/problems/search-insert-position/)
{% endhint %}



## Graduation Challenge (Binary Search)

* [ ] Identify which type of Binary Search does the follow code falls into.

| <img src="../.gitbook/assets/image (31).png" alt="" data-size="original"> | <img src="../.gitbook/assets/image (30).png" alt="" data-size="original">                                                                                |
| ------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <img src="../.gitbook/assets/image (33).png" alt="" data-size="original"> | <img src="../.gitbook/assets/image (34).png" alt="" data-size="original">                                                                                |
| <img src="../.gitbook/assets/image (35).png" alt="" data-size="original"> | [**Problems on Binary Search & Patterns**](https://docs.google.com/document/d/1V6-bCyst7xYYiMl6mjrg802VjikoKbssvwLTuFw9G\_Y/edit#heading=h.a5dh3x8vafix) |

