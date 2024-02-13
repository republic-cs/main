---
cover: ../.gitbook/assets/Group 9.png
coverY: 0
layout:
  cover:
    visible: true
    size: full
  title:
    visible: false
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: false
  pagination:
    visible: true
---

# §&#x20;

## RCS.101 - DSA In Action

{% hint style="success" %}
## What is RCS.101 for?

**RCS.101 - DSA In Action** 是一份旨在培養參與者 「資料結構」 與 「演算法」 實作精熟程度的 roadmap。

在 **RCS.101** 的四個模組中，我們編排了一系列在系統開發、學習 standard library 必不可少的的經典主題，並搭配一系列 LeetCode/LintCode 上的 Easy \~ Medium 題目，來鍛鍊實作能力。
{% endhint %}

{% hint style="danger" %}
## RCS.101 Doesn't Cover...

**RCS.101 - DSA In Action** 相較於其他屬性各異的教材，如 [Introduction to Algorithms](https://www.google.com/search?sca\_esv=f917e2823a31333e\&cs=0\&sxsrf=ACQVn0\_S1P6W4zIOOB4PPxATZqsCBEhlNQ:1707816716369\&q=Introduction+to+Algorithms\&stick=H4sIAAAAAAAAAONgVeLUz9U3sEwvMzMwEk7MSc8vyizJyC1WKEmtKEnKz88-xYhQcIqRVz9d39CwJLkqxbKq2BDGLzbPKzPPSc-B8dNys0qSKipSTjFygfSaGlRVFltAOXmmKVmGRjCVSebFRQa5pilI\_ALDipQqqGKTqhxLE0uYZFFVoXG8oQHQGh4Q38gkyyS3ON0cJp1lUpBlmlKW84jxHiO3wMsf94SlrjBOWnPyGuNZRi4Bn\_z84tScyqDUnMSS1JSQfCFRLjbXvJLMkkohbilOLnaQdVkFZUKuXNzBqSUh-b75KZlplUJmQiZcnL6puUmpRcX-aULqXFzO-Tk5qcklmfl5QpJS4lyi-slwAX1YoBUrRRq57bo07RybgyADEAhJBztIaWgJcrG55OcmZuYJipUdUfH9U22vJczFEZJYkZ-Xn1spaP81-jxn2gl7JU5OoB6FnX8u22sxTGBibNq34hAbBwejAIMREwdDFQPPIlYpz7ySovyUUrC1CiX5Co7wmJvAxggAiOO8m9YBAAA\&sa=X\&ved=2ahUKEwifwuCFgaiEAxUPmVYBHbUaBtIQ7fAIegQIABAv) 或 [九章算法](https://www.jiuzhang.com/) 「理解」 和 「充分熟悉」 經典的 DSA 實作。



因此，**RCS.101 - DSA In Action** 有以下的特色：



1. **預期參與者已經掌握基礎的 DSA 理論知識**，如時間複雜度、空間複雜度；此 roadmap 比起演算法課程，更像是一群由淺入深的 lab。
2. **作為 System Programming\* 相關主題的入門**，此 roadmap 的主題的編排次序並不是依照難度，而是他在系統開發上的相對重要性。
3. 許多在解題、證明、問題分析上經典的知識，如 **Dynamic Programming、Divide and Conquer、2 Pointers**，是此 roadmap 不會涵蓋的。而預期未來將它收錄在 [Broken link](broken-reference "mention") 上。
{% endhint %}

> System Programming\*：
>
> * [Broken link](broken-reference "mention")
> * [Broken link](broken-reference "mention")

{% hint style="success" %}
## As an Attendee

由於此 roadmap 與 system programming 預期帶來的銜接，我們會主要推薦參與者使用 Rust、C++、Go，或任何一門非 [Just-in-time Compilation](https://zh.wikipedia.org/zh-tw/%E5%8D%B3%E6%99%82%E7%B7%A8%E8%AD%AF) 的程式語言來進行學習。



採用較接近系統層的語言，是因為在開發過程中，benchmark CPU/memory 的用量都會較可控且容易。 許多經典的資料結構實作，也都是在系統層得到他的最大發揮。
{% endhint %}

{% hint style="info" %}
## Notice

* 想與社群一起參與學習這份 roadmap 的人，可以去 [RePublic of CS 的 Discord Server](https://discord.com/invite/cvbU8PYAYx)，領取 **`@rcs.101 ⌛`** 的身份組。
* `一起完整參與完`**RCS.101 - DSA In Action** 完整 classroom 的夥伴，可以獲得 **`@rcs.101 🏅`** 的身份組。



由於 **RCS.101 - DSA In Action** 和 lab 的同質性，我們期待參與者：\


* 在寫 「練習題」 時，請極力避免直接去看 LeetCode solution，因為最終目標是想將實作內化，而看解答很高機率會阻礙學習。
* 務必實作完所有的 「Graduation Challenge」 才視為自己完成了該主題。
* 在練習實作時，我們會極力推薦使用 「本地編輯器」 和 「撰寫單元測試」 來進行學習；這也是基於我們希望更貼近 system programming 和實務效能的量測。
{% endhint %}
