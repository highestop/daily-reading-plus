# [Maximizing Developer Effectiveness](https://martinfowler.com/articles/developer-effectiveness.html)

# [如何让技术想法更容易被理解？](https://mp.weixin.qq.com/s/m_pdAJGU3pz27CZGV7uYHw)

- 换位思考，角色转变。如站在产品的角度讲看待开发的东西
- 费曼技巧，给一个小白讲明白一件事 —— 「 如果你认为自己学会了某个专业知识，看看能否把这个知识教会 10 岁的孩子就知道了 」。教授知识可以加深理解，自我审视
- 简化语言和尝试类比，也是换位思考的一种，还要换位表达 —— 套用他人能轻易理解的场景，类比另一个领域的问题。其实也是跨学科的味道
- 维护一个术语表，识别出在客户交流界面的高频术语 —— 至少统一自己对外的表达
- 为高频术语都分别准备一个有生活场景的介绍
- 及时做笔记和持续更新

# [数字化时代，如何构建下一代研发协作工具平台？](https://mp.weixin.qq.com/s/mSiGj6IJ4Lf0Rv6PfsnjBA)

# [RxJS：给你如丝一般顺滑的编程体验](https://mp.weixin.qq.com/s/KaLjNOAOW7OY0TvMVL3q3g)

挺好的一篇大而全的 Rx 入门介绍，把基本概念（ 包括 Hot&Cold 也介绍了 ）

- callback 到 promise 解决的是可读性问题，promise 到 rx 解决的是可控制问题
- 响应式和流解决的问题不同，响应式表示是事件驱动，流是一种视角，将数据+事件组成时间上的切面，每个切面都是一种局部可观察状态
- 订阅发布模式使得响应式可以实现，迭代器模式使得流可以成为一个实体，Observable 就是连接这些元素的实体
- rx 可以表现为同步，原因在 scheduler
- operator 介绍的也比较详细，作为巩固
