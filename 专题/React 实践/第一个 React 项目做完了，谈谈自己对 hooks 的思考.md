# [第一个 React 项目做完了，谈谈自己对 hooks 的思考](https://mp.weixin.qq.com/s/kMLeg5KLFhXFZnjOF0fhvQ)

- 心智模型。「 函数式组件捕获了渲染所用的值 」—— [函数式组件与类组件有何不同？](https://overreacted.io/zh-hans/how-are-function-components-different-from-classes/)
  - function 因为 js 特性，更接近大家对代码的直观理解，class 引入了 this、闭包等复杂度
- 理解大佬发明新东西的思维，背后的逻辑最重要，不要跟风
  - function 比 class 简单，所以简化复制了 class 的能力到 function 中，就成了 hook。一切为了轻量灵活
  - conposition 的问题。hook 使得代码结构变化，一件事更能被写到一起了，所以复用的单元本身更好读
    - props + state -> view 是 functional component 的范式，其中 props 是围绕组件树的，state 因为有了 hook 就可以来源于脱离于组件树的逻辑，是否复用不是关键
- hook 的负担还是来自于心智成本
  - 「 在一次渲染中，组件的 props 和 state 是保持不变的 」
  - 例如 useEffect 淡化了组件生命周期，所以其影响也容易被忽略
  - 再例如性能优化的需求引入了 useMemo 和 useCallback 来控制数据变更的影响
- React 本身就很灵活，Hook 使得如何组织代码更灵活
  - ESLint 约束不了代码风格，但对于一个项目或团队，一致的风格才能有效减少心智成本
    - 形成自己的 React 是一种有效手段，培训是一种传承方式 —— 来自于原先读的「 一万个公司有一万种 Java 」
