# [将超过 5000 万行 JS 代码迁移到 TypeScript，我们得到的 10 大见解](https://mp.weixin.qq.com/s/iC-wI4mK48b0hq0HvGrZ8g)

基于 TypeScript 的迁移如果有一套「 环境 」支持是好的，「 环境 」支持会让开发有非常大的动力自主向前迁移，而不会畏手畏脚

他们「 让常规 TypeScript 文件成为我们 API 的唯一事实来源 」，也就是仓库并不编译 TS 而是运行时编译，这样能在运行时保持所有的类型声明

作者提到了几个关键性原则：Scalability、Ecosystem Coherence、Standards Alignement

- 生态包含基础设施和规范，基础设施让开发能聚焦于业务逻辑而非平台过程，规范能让多个开发产出给平台的实体是标准的。这应该是双向收益的
- 提到了 CI 的统一构建，如果 CI build 中有与 TS 版本相关的规范，则平台级别设施才好保证一致执行
- 还提到了 `tsconfig.json` 的一致性，比如保证全局依赖一致就需要它来定义统一的路径
- 一致性的表现为「 exactly-one 」，要避免元素的重复和诸如隐式依赖和导出（ 隐式 export 之前没见过 ）
- 封装可能导致脆弱（ 不保证安全或冲突 ）的类型定义
