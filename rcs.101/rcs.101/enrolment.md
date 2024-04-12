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
    visible: false
  pagination:
    visible: true
---

# § DSA In Action

<figure><img src="../.gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>

### RCS.101 Offerings

{% hint style="success" %}
**RCS.101** 是一份旨在培養軟體工程師對 「資料結構」 與 「演算法」 實作精熟程度的 Roadmap。

在 **RCS.101** 的四個模組中，RePublic of CS 編排了一系列在系統開發、學習 Standard Library 必不可少的的經典資料結構知識，搭配常見的 Online Judge，來鍛鍊實作能力。
{% endhint %}

***

### RCS.101 並不包含 / Out of Scope

{% hint style="danger" %}
**RCS.101** 相較於其他屬性各異的教材 (Ex. [**Introduction to Algorithms**](https://www.google.com/search?sca\_esv=f917e2823a31333e\&cs=0\&sxsrf=ACQVn0\_S1P6W4zIOOB4PPxATZqsCBEhlNQ:1707816716369\&q=Introduction+to+Algorithms\&stick=H4sIAAAAAAAAAONgVeLUz9U3sEwvMzMwEk7MSc8vyizJyC1WKEmtKEnKz88-xYhQcIqRVz9d39CwJLkqxbKq2BDGLzbPKzPPSc-B8dNys0qSKipSTjFygfSaGlRVFltAOXmmKVmGRjCVSebFRQa5pilI\_ALDipQqqGKTqhxLE0uYZFFVoXG8oQHQGh4Q38gkyyS3ON0cJp1lUpBlmlKW84jxHiO3wMsf94SlrjBOWnPyGuNZRi4Bn\_z84tScyqDUnMSS1JSQfCFRLjbXvJLMkkohbilOLnaQdVkFZUKuXNzBqSUh-b75KZlplUJmQiZcnL6puUmpRcX-aULqXFzO-Tk5qcklmfl5QpJS4lyi-slwAX1YoBUrRRq57bo07RybgyADEAhJBztIaWgJcrG55OcmZuYJipUdUfH9U22vJczFEZJYkZ-Xn1spaP81-jxn2gl7JU5OoB6FnX8u22sxTGBibNq34hAbBwejAIMREwdDFQPPIlYpz7ySovyUUrC1CiX5Co7wmJvAxggAiOO8m9YBAAA\&sa=X\&ved=2ahUKEwifwuCFgaiEAxUPmVYBHbUaBtIQ7fAIegQIABAv) 或 [**九章算法**](https://www.jiuzhang.com/))，聚焦在 「理解」 和 「充分熟悉」 經典的 DSA 實作。



因此，**RCS.101** 有以下的特色：



1. **預期參與者已經掌握基礎的 DSA 理論知識**，如時間複雜度、空間複雜度；**RCS.101** 比起演算法課程，更偏重提供由淺入深的 Lab。
2. **作為 System Programming** ([Broken link](broken-reference "mention") [Broken link](broken-reference "mention")) **相關主題的入門**，此 Roadmap 的主題的編排次序並不是依照難度，而是他在系統開發上的相對重要性。
3. 許多在解題、證明、問題分析上經典的知識，如 **Dynamic Programming、Divide and Conquer、2 Pointers**，是此 Roadmap 不會涵蓋的。而預期未來將它收錄在 [Broken link](broken-reference "mention") 上。
{% endhint %}

***

### RCS.101 參與須知 / Notice&#x20;

{% hint style="success" %}
由於此 Roadmap 與 System Programming 預期帶來的銜接，我們會主要推薦參與者使用 Rust、C++、Go，或任何一門非 [**Just-in-time Compilation**](https://zh.wikipedia.org/zh-tw/%E5%8D%B3%E6%99%82%E7%B7%A8%E8%AD%AF) 的程式語言來進行學習。



採用較接近系統層的語言，是因為在開發過程中，Benchmark CPU/Memory 的用量都會較可控且容易。 許多經典的資料結構實作，也都是在系統層得到他的最大發揮。
{% endhint %}

{% hint style="info" %}
* 想與社群一起參與學習這份 Roadmap 的人，請去 RePublic of CS [Discord](https://discord.com/invite/cvbU8PYAYx)，領取 **`@rcs.101 ⌛`** 的身份組。
* 一起完整參與完 [Broken link](broken-reference "mention") 完整 Classroom 的夥伴，可以獲得 **`@rcs.101 🏅`** 的身份組。



#### 由於 [Broken link](broken-reference "mention") 和 lab 的同質性，我們期待參與者：

1. 在寫 「練習題」 時，<mark style="color:red;">**極力避免去看 「任何形式的解答」**</mark>  (如 Solutions/Hints/題解影片)。
2. 因為 [Broken link](broken-reference "mention") 的學習目標是想將實作內化，而看解答很高機率會阻礙認知的培養。
3. <mark style="color:red;">**務必實作完所有的 Lab**</mark>，才能視為完成了該主題。
4. 在練習實作時，<mark style="color:red;">**使用  「本地編輯器開發」  和  「用單元測試描述測資」  來進行開發**</mark> (而非採用 online editor)。
   * 這是基於 [Broken link](broken-reference "mention") 希望能以此銜接 [Broken link](broken-reference "mention") 在開發與偵錯時的實體環境。
5. 在解題時，<mark style="color:red;">**Write Out Loud、White-boarding、Dry Run**</mark>，儘管在 [Broken link](broken-reference "mention") 才會比較要求。但我們也鼓勵參與者用這些方式來讓自己更熟悉腦內構思的流程。
{% endhint %}
