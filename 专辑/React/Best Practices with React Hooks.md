# [Best Practices with React Hooks](https://blog.bitsrc.io/best-practices-with-react-hooks-69d7e4af69a7)

> - [6 Tips and Best Practices for a Scalable React Project](https://blog.bitsrc.io/best-practices-and-tips-for-a-scalable-react-application-db708ae49227)
>
> 翻译：[6 个 React Hook 最佳实践技巧](https://mp.weixin.qq.com/s/3sXQ8jrZN9N4lhKecWR7Sw)

- 用 hook 时思考是否被复用到。但其实没复用，为什么代码结构清晰，也可以用 hook？
- 借助工具保证代码风格的一致，有利于项目扩张。包括文件目录组织方式
- 面向测试编程，React 的函数式写法更有利于测试
- 分离开发 UI 渲染层组件，逻辑与功能元素分离。也是面向测试的一种体现，因为逻辑测试和 UI 测试是分开的，虽然都是单测
