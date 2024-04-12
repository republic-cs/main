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

# RCS.101.b

{% tabs %}
{% tab title="Map of Contents" %}
<figure><img src="../.gitbook/assets/image (8).png" alt=""><figcaption><p>RCS.101.b</p></figcaption></figure>
{% endtab %}

{% tab title="Linked List & Hash Map" %}
{% embed url="https://www.youtube.com/watch?index=5&list=PLskIq2MzopHCU6IAoYtedpzOzgWItmmQI&v=JYYhkqdK1zU" %}
\[RCS.101 x Miters] Linked List & Hash Map
{% endembed %}
{% endtab %}

{% tab title="Basic Recursion" %}
{% embed url="https://www.youtube.com/watch?index=6&list=PLskIq2MzopHCU6IAoYtedpzOzgWItmmQI&v=KXUYUhqGVgk" %}
\[RCS.101 x Miters] Basic Recursion
{% endembed %}
{% endtab %}

{% tab title="Sorting & Searching" %}
{% embed url="https://www.youtube.com/watch?index=7&list=PLskIq2MzopHCU6IAoYtedpzOzgWItmmQI&v=W6l-_SAhj7g" %}
\[RCS.101 x Miters] Sorting/Searching (1)
{% endembed %}

{% embed url="https://www.youtube.com/watch?index=8&list=PLskIq2MzopHCU6IAoYtedpzOzgWItmmQI&v=yLYSIbeV4po" %}
\[RCS.101 x Miters] Sorting/Searching (2)
{% endembed %}
{% endtab %}
{% endtabs %}

## Linked List

{% hint style="info" %}
**Linked Lists**, similar to arrays, are a data structure that allow you to store a collection of items in a specific order. Unlike arrays, elements in a linked list are not stored at contiguous memory locations and are instead stored in nodes that are linked using pointers.



#### Learning Material

* [**Comp Sci in 5: Introduction to Nodes and Linked List**](https://www.youtube.com/watch?v=m40pUS58i7k)
* [**LeetCode The Hard Way: Linked List**](https://leetcodethehardway.com/tutorials/basic-topics/linked-list)
  * [ ] (traversal) **Naive** [**466 · Count Linked List Nodes**](https://www.lintcode.com/problem/466/?showListFe=true\&page=1\&problemTypeId=2\&tagIds=362\&ordering=level\&pageSize=50)
  * [ ] (deletion) **E** [**452 · Remove Linked List Elements**](https://www.lintcode.com/problem/452/?showListFe=true\&page=1\&problemTypeId=2\&tagIds=362\&ordering=level\&pageSize=50)
* [**Google Tech Dev Guide: Linked Lists**](https://techdevguide.withgoogle.com/paths/data-structures-and-algorithms/#sequence-2)
  * (build your own) **M** [**707. Design Linked List**](https://leetcode.com/problems/design-linked-list/)
{% endhint %}

* Practices
  * [ ] **E** [**83. Remove Duplicates from Sorted List**](https://leetcode.com/problems/remove-duplicates-from-sorted-list/)
  * [ ] **E** [**206. Reverse Linked List**](https://leetcode.com/problems/reverse-linked-list/)
  * [ ] **M** [**92. Reverse Linked List II**](https://leetcode.com/problems/reverse-linked-list-ii/) (with 1-pass)
* Graduation Challenge
  * [ ] **M** [**2. Add Two Numbers**](https://leetcode.com/problems/add-two-numbers/)

***

## Hash Map

{% hint style="info" %}
**Maps** (also known as **Dictionaries**) are data structures stores a collection of key-value pairs. Each key is unique and allows for quick access to values. A real life example of a map could be storing the grades for students in a class (student name is key, grade is value).



#### Learning Material

* [**LeetCode The Hard Way: Hash Map**](https://leetcodethehardway.com/tutorials/basic-topics/hash-map)
* [**Google Tech Dev Guide: Map/Dictionaries**](https://techdevguide.withgoogle.com/paths/data-structures-and-algorithms/#linear)
* [**Internals of Maps in Golang**](https://www.youtube.com/watch?v=ACQs6mdylxo) (useful for Design HashMap)



In real-world use cases, there's a few classic concept & approaches to implement a performant HashMap

* Open Addressing
* Separate Chaining
* Load Factor
* Re-hashing
* Linear Probing
* Eternal Tombstone
{% endhint %}

* Practices
  * [ ] **E** [**706. Design HashMap**](https://leetcode.com/problems/design-hashmap/)
  * [ ] **E** [**217. Contains Duplicate**](https://leetcode.com/problems/contains-duplicate/)
  * [ ] **E** [**3642 · Counting Elements**](https://www.lintcode.com/problem/3642/)
  * [ ] **E** [**383. Ransom Note**](https://leetcode.com/problems/ransom-note/)
* Graduation Challenge
  * [ ] **E** [**1832. Check if the Sentence Is Pangram**](https://leetcode.com/problems/check-if-the-sentence-is-pangram/)
  * [ ] **M** [**2225. Find Players With Zero or One Losses**](https://leetcode.com/problems/find-players-with-zero-or-one-losses/)
  * [ ] **M** [**1604 · Maximum Sum of Two Numbers**](https://www.lintcode.com/problem/1604/)

***

## Sorting & Searching

{% hint style="info" %}
Searching algorithms are used to Sorting algorithms are used to rearrange a list of elements so that they're in a specified order (e.g. sorting numbers to go from highest to lowest).

* Learning Material
  * [**LeetCode Explore: Sorting**](https://leetcode.com/explore/learn/card/sorting/)
  * [**Google Tech Dev Guide: Map/Dictionaries**](https://techdevguide.withgoogle.com/paths/data-structures-and-algorithms/#sequence-8)
  * [**Dutch National Flag Problem**](https://en.wikipedia.org/wiki/Dutch\_national\_flag\_problem)
    * [ ] Understand [**DNF Algorithm**](https://www.youtube.com/watch?v=9pdkbqGwUhs)
    * [ ] **M** [**75. Sort Colors**](https://leetcode.com/problems/sort-colors/)
  * **Coursera: Algorithms I: System Sort**
    * [ ] **M** [**912. Sort an Array**](https://leetcode.com/problems/sort-an-array/) with Merge Sort
    * [ ] **E** [**479 · Second Max of Array**](https://www.lintcode.com/problem/479/?\_from=problem\_tag\&fromId=383) with Quick Sort
    * [ ] **E** [**464 · Sort Integers II**](https://www.lintcode.com/problem/464/description) with Heap Sort
  * [**Knuth (Fisher-Yates) Shuffle**](https://www.youtube.com/watch?v=tLxBwSL3lPQ)
    * [ ] **M** [**384. Shuffle an Array**](https://leetcode.com/problems/shuffle-an-array/)
  * [**Quick Select**](https://www.lintcode.com/problem/3731/description)
    * [ ] **M** [**215. Kth Largest Element in an Array**](https://leetcode.com/problems/kth-largest-element-in-an-array/)
{% endhint %}

* Practices
  * [ ] **M** [**148. Sort List**](https://leetcode.com/problems/sort-list/)
  * [ ] **M** [**3653 · Meeting Scheduler**](https://www.lintcode.com/problem/3653/?\_from=problem\_tag\&fromId=383)
  * [ ] **M** [**2545. Sort the Students by Their Kth Score**](https://leetcode.com/problems/sort-the-students-by-their-kth-score/)
* Graduation Challenge
  * [ ] 能描述出 Merge/Quick/Heap Sort 在 time, space, stable, in-place 上的差別
  * [ ] 提供 Merge/Quick/Heap Sort 的實作程式碼
  * [ ] **E** [**1153 · string sorting**](https://www.lintcode.com/problem/1153/?showListFe=true\&page=1\&problemTypeId=2\&tagIds=383\&level=1\&ordering=id\&pageSize=50)
  * [ ] **M** [**508 · Wiggle Sort**](https://www.lintcode.com/problem/508/?showListFe=true\&page=1\&problemTypeId=2\&tagIds=383\&level=2\&ordering=level\&pageSize=50)
  * [ ] **M** [**3731 · Minimize Product Sum of Two Arrays**](https://www.lintcode.com/problem/3731/description)
  * [ ] **M** [**973. K Closest Points to Origin**](https://leetcode.com/problems/k-closest-points-to-origin/)
