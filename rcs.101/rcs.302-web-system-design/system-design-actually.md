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

{% hint style="danger" %}
## However

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

<table data-view="cards"><thead><tr><th></th><th></th><th></th></tr></thead><tbody><tr><td><img src="../.gitbook/assets/image.png" alt="" data-size="original"></td><td><em>"For system design interviews, we suggest focusing on scale and performance"</em></td><td></td></tr><tr><td><img src="../.gitbook/assets/image (1).png" alt="" data-size="original"></td><td><em>"These non-functional requirements are what make our design unique and challenging"</em></td><td></td></tr><tr><td><img src="../.gitbook/assets/image (4).png" alt="" data-size="original"></td><td><em>"For example, designing a Twitter clone to support a few hundred user is easy"</em></td><td></td></tr><tr><td><img src="../.gitbook/assets/image (5).png" alt="" data-size="original"></td><td><img src="../.gitbook/assets/image (6).png" alt="" data-size="original"></td><td><em>"The more senior the role is, the more important it is for us to demonstrate our ability to handle to non-functional requirements"</em></td></tr></tbody></table>

{% hint style="danger" %}
#### 在琢磨這些資源的陳述方式後，會發現包含了以下的主旋律

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
3. **非功能性需求** (non-functional requirement) 的實現，必須要能基於 **Telemetry** 和 **Profiling** (效能量測) 的事實
{% endhint %}

## Interview-Style System Design, 會帶來什麼問題？
