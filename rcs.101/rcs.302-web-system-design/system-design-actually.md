---
description: >-
  Understanding the essence of System Design, and how you could learn it
  systematically.
cover: ../.gitbook/assets/Group 7.png
coverY: 0
layout:
  cover:
    visible: true
    size: full
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# System Design, Actually

## Introduction

在經歷過 2023 \~ 2024 的 [Tech Layoff](https://www.youtube.com/watch?v=j6DG1NqgkSU)，現今軟體就業市場的[要求變的十分的高](https://www.youtube.com/watch?v=j6DG1NqgkSU)。

而 System Design Interview ([系統設計面試](https://github.com/donnemartin/system-design-primer))，由於他能涵蓋的深度與廣度十分充足，也逐漸成為公認能鑑定 senior engineer 的標準。

{% hint style="warning" %}
#### **However**

現下的軟體工程行業，對 system design 究竟代表什麼能力、Jr/New Grad 如何逐步學習 system design，是沒有共識的。



在筆者過往與 Senior/Staff 等級的工程師對談時，95% 以上的人都無法描述出 **「System Design 如何學」**。

而當我們詢問這些 Senior/Staff 工程師，他們是如何想出某個系統設計方案時，很多時候也僅能得到 **「靈光一閃就想到了、依賴以前的積累」**，這些落於 **經驗主義** 的答案。
{% endhint %}

在此篇文章，筆者會試著探討對於現今 Jr/New Grad **「System Design 學習障礙」** 的觀察，網路上的學習資源有哪些優劣。

最後，提出一個幾個筆者認為能讓學習 system design 事半功倍的 mindset，並希望最終能說服你 **「System Design 就等同 Problem Solving」** ，和 「**之所以 system design 會難，是因為多數人都沒把 Problem Solving 學好」**。

## System Design Interview Propaganda

作為 Jr, New Grad, or 想增進架構能力的人，初次會接觸的教材諸如：

* [System Design Interview – An insider's guide](https://www.amazon.com/System-Design-Interview-insiders-Second/dp/B08CMF2CQF?dib=eyJ2IjoiMSJ9.CZwZ7txhICEtME2JuLCqj9Bkde4opffmKt\_uE1rHfELX\_jk4zl8rgkiRLIVmk6Ez\_s7dU9Ybiy5klGL8pLX1ZoajyWuuF0DjqNCDh09MKwEsvNlz\_57cn14Bf488YE0PHlr\_KKWyKLrG38QK2kNpFXFnV\_YUlsYrwIfFBT0Rd5VPfJUmPPx\_sTtexI9qIQwxNl66diDWim8oMMGRKQnyCuxM-4huF2ZpWg7Jwd2PQEw.Er5hEIShVzcrU4Ba6hWeDKKz1wtdiMZLe74UlPfd7oc\&dib\_tag=se\&keywords=byte+byte+go+system+design\&qid=1708846788\&sr=8-1)
* [System Design Interview – An Insider's Guide: Volume 2](https://www.amazon.com/System-Design-Interview-Insiders-Guide/dp/1736049119/ref=sr\_1\_4?dib=eyJ2IjoiMSJ9.CZwZ7txhICEtME2JuLCqj9Bkde4opffmKt\_uE1rHfELX\_jk4zl8rgkiRLIVmk6Ez\_s7dU9Ybiy5klGL8pLX1ZoajyWuuF0DjqNCDh09MKwEsvNlz\_57cn14Bf488YE0PHlr\_KKWyKLrG38QK2kNpFXFnV\_YUlsYrwIfFBT0Rd5VPfJUmPPx\_sTtexI9qIQwxNl66diDWim8oMMGRKQnyCuxM-4huF2ZpWg7Jwd2PQEw.Er5hEIShVzcrU4Ba6hWeDKKz1wtdiMZLe74UlPfd7oc\&dib\_tag=se\&keywords=byte+byte+go+system+design\&qid=1708846788\&sr=8-4)
* [The System Design Primer](https://github.com/donnemartin/system-design-primer)
* [LeetCode System Design](https://leetcode.com/discuss/interview-question/system-design?currentPage=1\&orderBy=hot\&query=)

但當讀者試著參考、依賴以上的素材去學時，多少會發現一些怪味道 (待會會提到)

我們採用[ System Design Interview: A Step-By-Step Guide](https://www.youtube.com/watch?v=i7twT3x5yv8) 的幾個敘述，來試著傳達問題在哪：

<table data-view="cards"><thead><tr><th></th><th></th><th></th></tr></thead><tbody><tr><td><img src="../.gitbook/assets/image (4).png" alt="" data-size="original"></td><td><em>"For system design interviews, we suggest focusing on scale and performance"</em></td><td></td></tr><tr><td><img src="../.gitbook/assets/image (1) (1) (1).png" alt="" data-size="original"></td><td><em>"These non-functional requirements are what make our design unique and challenging"</em></td><td></td></tr><tr><td><img src="../.gitbook/assets/image (4) (1).png" alt="" data-size="original"></td><td><em>"For example, designing a Twitter clone to support a few hundred user is easy"</em></td><td></td></tr><tr><td><img src="../.gitbook/assets/image (5).png" alt="" data-size="original"></td><td><img src="../.gitbook/assets/image (6).png" alt="" data-size="original"></td><td><em>"The more senior the role is, the more important it is for us to demonstrate our ability to handle to non-functional requirements"</em></td></tr></tbody></table>

{% hint style="warning" %}
#### **在琢磨這些資源的陳述方式後，會發現包含了以下的主旋律**

1. 在系統設計、架構中，效能與可擴充性是最重要的
2. 只有盡可能展現出自己對 **非功能性需求** (non-functional requirement) 的硬理解，才像個 senior
3. **功能性需求** (functional requirement) 是系統設計的 easy parts
4. 在系統設計時，應該**要能快速、立即的提出一個 HLD** (high level design)
5. 相較於探討 profiling/benchmarking，設計者可以 **對 QPS/Bandwidth 輕易的訂下 assumption**
{% endhint %}

相對於上列的套路。筆者認為以下的哲學，才是實務和學習時，看待系統設計比較實際的方式：

{% hint style="success" %}
1. **遠離 Grand Design** (一眼定奪、天才且直覺產生的架構設計)，偏好 **逐步發展解法**
2. 偏好從 **功能性需求** (functional requirement)  **作為設計的開頭**，再逐漸納入 **非功能性需求** (non-functional requirement) 和 **Constraints** (系統的 tradeoff, 取捨)
3. **非功能性需求** (non-functional requirement) 的實現，必須要能基於 **Telemetry** 和 **Profiling** (效能量測) 的事實，並且 **深刻理解 infrastructure 背後的實作**。
{% endhint %}

## [Interview-Style System Design](https://republic-of-cs.gitbook.io/e/rcs.302-web-system-design/system-design-actually#zai-zhuo-mo-zhe-xie-zi-yuan-de-chen-shu-fang-shi-hou-hui-fa-xian-bao-han-le-yi-xia-de-zhu-xuan-lv), 會帶來什麼問題？

### ❌ 選擇追求 Grand Design

{% hint style="danger" %}
如果在系統設計實務、學習時，實作者只專注在 **快速、立即的提出 HLD**，而非逐步的發展解法。

這會導致實作者最終的設計提案，及學習的過程，都產生 **「去脈絡化」** 的成果。而這會導致：

* 對學習者，Grand Design 的思維陷阱，會讓人傾向去背答案/不求甚解，並且學到與實務 problem solving 相反的推導過程。
* 而對於架構師而言，追求一個 One-off, Clever 的 Grand Design，恰好踩中了 [**Who Needs an Architect?**](https://martinfowler.com/ieeeSoftware/whoNeedsArchitect.pdf) 這篇文中所描述的 anti-pattern：_Architectus Reloadus_

#### Architectus Reloadus

* 這樣的架構師，傾向在初期規劃就提出一個完備、複雜、又聰明的系統設計。
* 此舉會導致其他專案成員難以參透和證偽諸多的初期決策。最終使整個系統更難在未來有效的融入新的功能/非功能性考量。
{% endhint %}

### ❌ 忽略**功能性需求** (functional requirement)

{% hint style="danger" %}
在 [System Design Interview: A Step-By-Step Guide](https://www.youtube.com/watch?v=i7twT3x5yv8) 的宣揚中，營造了一個幻想：

* 認為軟體行業內的 Staff/Architect 全都是腦中只關注 Hard Skills, Non-functional Requirement 一群人。

但今天在任何型態的軟體公司中，去與團隊內的 Staff/Architect 訪談。筆者會發現，Staff/Architect 的實際模樣，和上述的幻想是完全相悖的。每個能被 promote 到 Staff/Architect 的工程師，在商業策略、宏觀的產品理解、使用情境上，全都比一般的工程師有過之而無不及。

#### Why is Functional Requirement Important?

在任何的軟體公司的開發上，產品都是從 MVP (最小可行產品)，逐步的發展到一個成熟的盈利功能。這也與架構的演進相互應。

並且一個軟體產品在本質上能帶來使用者價值與獲利，功能性需求是佔了絕大多數的貢獻。

因此，在任何的產品開發路徑上，架構很大程度都是從 **功能性需求** 的 **「分析」**、**「開發」**、**「驗證」**、**「擴充」** 來實現的。

因此，在任何場景的系統、架構設計中，從滿足功能性需求的路徑，去逐步納入效能、穩定性上的考量。才能確保架構師們不 over-design，也設計得精準。
{% endhint %}

### ❌ 忽略 Profiling 與 Benchmarking

{% hint style="danger" %}
諸如 QPS/Bandwidth 的非功能性需求，在實務上都不是能夠輕易的去做出 dare assumption 的。

多數時候，都得從使用者情境、Telemetry (系統遙測) 得到的效能觀察、作出假設與實驗，才能知道架構的預期與解法該往怎麼方向發展。而這才是實務上分析與理解 non-functional requirement 的標準解決流程。
{% endhint %}

## 結語：如何克服 「System Design 學習障礙」

在此文中，描述了網路上的 System Design 學習資源，以及常見的 [**認知誤區**](https://republic-of-cs.gitbook.io/e/rcs.302-web-system-design/system-design-actually#zai-zhuo-mo-zhe-xie-zi-yuan-de-chen-shu-fang-shi-hou-hui-fa-xian-bao-han-le-yi-xia-de-zhu-xuan-lv) 會如何讓 system design 的學習事倍功半。

而克服 System Design 這門知識混亂的學問，筆者認為可以從兩個方向進行主題式的學習。

{% hint style="success" %}
#### **Software Architecture**

<img src="../.gitbook/assets/image (2) (1).png" alt="" data-size="original">

軟體設計/架構這們學問，本質上探討的問題就是 **「從一群需求中，如何能發展出一個模型來陳述要實現的功能」**，掌握他能讓軟體工程師對功能性需求的實現有更全盤性的理解。



以下的幾個主題，及[ Architecture, Actually ](https://alxtz.substack.com/p/architecture-actually-w0)有提供數個學習方向：

* Domain Driven Design
* OOAD (Object-Oriented Analysis and Design)
* Clean Architecture



讀者的練習目標該放在**能做出精準、系統性的做出 Feature Modeling**，並能高效的草稿出滿足所有功能性需求的 design MVP。
{% endhint %}

{% hint style="success" %}
#### **System Programming**

![](<../.gitbook/assets/image (3).png>)

幾乎所有的 **非功能性需求 (non-functional requirement)**，在電腦科學的 Distributed Systems、Parallel Computing、Operating System 都有所琢磨。

因此，針對效能、穩定性、一致性等問題的解法，學習者可以將眼光放在熟讀以上的經典電腦科學知識。

\
並以此延伸，透過自己實作經典的系統元件 (如 Redis, Load Balance, BTree)，來熟知元件真正的效能瓶頸，解法和如何量測。(RCS.103 System Programming 就是希望能編排出能滿足以上能力的練習)&#x20;
{% endhint %}
