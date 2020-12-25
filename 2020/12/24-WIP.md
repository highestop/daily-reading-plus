# [How to Evaluate NPM Packages](https://thecarrots.io/blog/how-to-evaluate-npm-packages)

作者介绍了一些自己选择第三方库时的考虑因素和建议

好的选择会让长期体验更佳而不是更痛苦（ If software has eaten the world, then open-source software propels it forward ）

- 光看 Star 是片面的，还要看如 Contributor 数量、Userd 项目数量、是否有 Sponsor 等
    - 作者给了一个查询 Star 历史的工具，输入仓库地址即可。如 https://star-history.t9t.io/#NG-ZORRO/ng-zorro-antd
    - 还要看下 Contributors 的活跃程度与分布，比如「 换届了 」或总是少数几个人维护就不太理想
- 性能上看最大的因素是包体积，以及「 弹性 」？—— 比如提到了 AntD 的一些 side effect（ 部分因为 momentjs 造成 ）使得模块的 tree-shaking 效果不佳
- 安全性基本能靠广大的 Contributors 和依赖方得到保证

除此之外想做两点补充：

- 文档。个人感觉从文档上也能看出一个团队在维护一个开源成果上的态度和能力。有些库的文档不好读不好找，有些文档缺失关键信息，这都是一些不友好或者可预见的隐患
- Issue。Issue 绝对数量多少是一方面，最好还要看下 Issue 上的更新频率，尤其是 Contributors 对 Issues 的关注度。如果大多数问题总是很久才解决，可能也是个隐患。以及从一些 Closed Issue 的原因上能看出些许开发团队的立场和方向是否与自己团队的一致或相符，比如我们很重视 TS 的严格性，但因此提出的议题别人却觉得不重要因此被忽略，可能就会出现分歧甚至之后更大的问题

# [RxJS with React Hooks for state management](https://blog.logrocket.com/rxjs-with-react-hooks-for-state-management/)

- 介绍了一种利用 Rx + Hooks 实现 State Control 的非常简单的实践
- Rx + Hooks 可能可以做到很优雅，这个需要找到最佳实践

# [10 Ways to Speed Up React Development](https://thecarrots.io/blog/10-ways-to-speed-up-react-development)

- 选一款 Css-in-JS
- 推荐了 Storybook（ 能 mock 能 isolate config 有助于结构化 ）
- 强烈不建议手写 form，用 formik 或 hook-form
- zsh 等 Superpowered Terminal 可以提效
- React 社区很强大，不要重复造轮子

# [Facebook 新一代 React 状态管理库 Recoil](https://mp.weixin.qq.com/s/D867pstcuk4TszMn3zRJRw)

介绍了下 Recoil 的背景和基本用法。个人理解 Recoil 是基于 Context 做了更小粒度的（ Atom ）的变更订阅，同时代码上更友好。相比起来 Redux 还是太重了，而 Mobx 用了 decorator

# [What is a project management office (PMO) and do you need one?](https://www.cio.com/article/2441862/what-is-a-project-management-office-pmo-and-do-you-need-one.html)

- A PMO makes sure company procedures, practices and operations go right — on time, on budget and all in the same way. 很重要的一点是「 保证 」
- Is agile enough to adapt as strategy shifts. 需要有足够的经验才能做到，而不光光是熟练程度和视野
- 分为 Supportive、Controlling 和 Directive 三种 PMO，按顺序从主动性、驱动性、严格性排序
- 如果一件事需要多个团队沟通协作、且成本和紧急程度都相对可观时，需要一个 PMO 来掌管项目

扩展阅读：[How to develop a PMO strategic plan](https://www.cio.com/article/3288926/how-to-develop-a-pmo-strategic-plan.html)、[10 project management myths to avoid](https://www.cio.com/article/3252332/10-project-management-myths-to-avoid.html)

# [2020 国内公司前端团队都在搞些什么?](https://www.zhihu.com/question/398940598/answer/1269685808)

针对前端基建给了一些很实用的建议。大致可以分为三个阶段

- 规范化、工具化
    - 研发规范，包含代码规范、分支规范与环境管理等
    - 组件化和模板化
    - 用 CLI 集成组件、模板以及文件处理工具来统一代码规范
- 服务化、SOP
    - 接管项目从创建到发布发版流程，深度集成仓库、CI/CD 与环境服务器，工作流化
    - 私有部署的 NPM 服务器、Docker 镜像托管
    - 基于私有包管理和统一工作流，可以做很多检查反馈。如发布代码前的统一静态检查、发布后的统一集成测试检查（ 如无头浏览器 ）、NPM 包依赖关系检查等
    - 生产环境的性能监控及错误报警，就是 APM 和 QoE 那套，结合源码做映射自动定位问题代码（ 像 Sentry ），数据与行为日志录制并回放（ 不能自动定位的问题手动观察 ）
    - 基础能力有了，考虑扩大端上范围，如移动端、桌面端
    - 结合上面的工作流管理，收拢所有变更事件，做高效触达，支持订阅中心来提效整个团队管理
- 去服务化、上云
    - 后台的后台：配置中心、数据中心、基地页、低代码平台
    - 端与端架构：微服务、微前端、独立网关、接口配置与模拟、视图聚合与裁剪

# [从 Angular 转到 React，网易严选的前端工程化实践](https://mp.weixin.qq.com/s/6NBaHzMtTCmEk3SKJQDTUQ)

- 规范、提效
- 渐进式（ 演进能力 ）、扩展性（ 可伸缩、可插拔 ）、易用性（ 贴合实际、好推广落地 ）
- 基础能力需要分层：
    - 基础能力如 eslint 规范、webpack、schematics、node
        - 提供完备的 dev 环境，包含 eslint 规范、webpack 编译、本地 server、数据转发或 mock 等
    - 插件封装，允许自定义插件按给定的方式接入到基础层，保证扩展性
        - 插件的集成：用 npx 按需安装卸载，如自定义的 init
        - 插件的开发，描述为一套 schmatics，用 ng-cli 提供的 schmatics 能力来实现
    - 命令层，统一做收口，简单甚至零配置，一键式操作，增强易用性
- 基础能力要覆盖整个项目的生命周期，如初始化、新增和升级资源、新增组件、调试、静态检查、测试、编译、部署集成 CI/CD
- 工具为基础能力提供了落地的可能，如规范的落地用一个 CLI 就能解决，约定优于配置，大家直接用就好，减少心智成本