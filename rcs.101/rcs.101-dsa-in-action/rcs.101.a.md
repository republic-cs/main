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

* Prerequisite
  * [#queue](rcs.101.a.md#queue "mention")
* Learning Material
  * [**Level Order Traversal**](https://faculty.cs.niu.edu/\~mcmahon/CS241/Notes/Data\_Structures/binary\_tree\_traversals.html)
* Practices
  * [ ] **M** [**102. Binary Tree Level Order Traversal**](https://leetcode.com/problems/binary-tree-level-order-traversal/)
  * [ ] **M** [**854 · Closest Leaf in a Binary Tree**](https://www.lintcode.com/problem/854/)
* Graduation Challenge
  * [ ] **M** [**1302. Deepest Leaves Sum**](https://leetcode.com/problems/deepest-leaves-sum/)
  * [ ] **M** [**103. Binary Tree Zigzag Level Order Traversal**](https://leetcode.com/problems/binary-tree-zigzag-level-order-traversal/)

{% hint style="warning" %}
**BFS - Shortest Path Finding**

> This is an extension of the BFS topic (as we've not included in the original scope)
>
> Shortest Path Finding in an Unweighted Graph is considered a CS classic in BFS. Thus we've reserved a spot for it.&#x20;

* Learning Material
  * [**Shortest Path in a Binary Matrix - LeetCode 1091 - Python**](https://www.youtube.com/watch?v=YnxUdAO7TAo)
  * [**Breadth First Search - Finding Shortest Paths in Unweighted Graphs**](https://www.youtube.com/watch?v=T\_m27bhVQQQ)
* Practices
  * [ ] **M** [**1091. Shortest Path in Binary Matrix**](https://leetcode.com/problems/shortest-path-in-binary-matrix/)
  * [ ] **M** [**3719 · Shortest Path to Get Bubble Tea**](https://www.lintcode.com/problem/3719)
{% endhint %}

***

## Binary Search

* Learning Material
  * [**LC Explore: Binary Search**](https://leetcode.com/explore/learn/card/binary-search/)
* Practices
  * [ ] **E** [**704. Binary Search**](https://leetcode.com/problems/binary-search/)
    * [ ] Implement via [**Template I**](https://leetcode.com/explore/learn/card/binary-search/125/template-i/938/)
    * [ ] Implement via [**Template II**](https://leetcode.com/explore/learn/card/binary-search/126/template-ii/937/)
    * [ ] Implement via [**Template III**](https://leetcode.com/explore/learn/card/binary-search/135/template-iii/936/)
  * [ ] **E** [**69. Sqrt(x)**](https://leetcode.com/problems/sqrtx/)
  * [ ] **E** [**278. First Bad Version**](https://leetcode.com/problems/first-bad-version/)
  * [ ] **M** [**375. Guess Number Higher or Lower II**](https://leetcode.com/problems/guess-number-higher-or-lower-ii/) (tricky)
  * [ ] **M** [**162. Find Peak Element**](https://leetcode.com/problems/find-peak-element/)
* Graduation Challenge
  * [ ] **M** [**33. Search in Rotated Sorted Array**](https://leetcode.com/problems/search-in-rotated-sorted-array/)
  * [ ] **M** [**34. Find First and Last Position of Element in Sorted Array**](https://leetcode.com/problems/find-first-and-last-position-of-element-in-sorted-array/)
