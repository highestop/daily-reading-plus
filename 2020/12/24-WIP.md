# [How to Evaluate NPM Packages](https://thecarrots.io/blog/how-to-evaluate-npm-packages)

# [RxJS with React Hooks for state management](https://blog.logrocket.com/rxjs-with-react-hooks-for-state-management/)

- 介绍了一种利用 Rx + Hooks 实现 State Control 的非常简单的实践
- Rx + Hooks 可能可以做到很优雅，这个需要找到最佳实践

# [What is a project management office (PMO) and do you need one?](https://www.cio.com/article/2441862/what-is-a-project-management-office-pmo-and-do-you-need-one.html)

- A PMO makes sure company procedures, practices and operations go right — on time, on budget and all in the same way. 很重要的一点是「 保证 」
- Is agile enough to adapt as strategy shifts. 需要有足够的经验才能做到，而不光光是熟练程度和视野
- 分为 Supportive、Controlling 和 Directive 三种 PMO，按顺序从主动性、驱动性、严格性排序
- 如果一件事需要多个团队沟通协作、且成本和紧急程度都相对可观时，需要一个 PMO 来掌管项目

扩展阅读：[How to develop a PMO strategic plan](https://www.cio.com/article/3288926/how-to-develop-a-pmo-strategic-plan.html)、[10 project management myths to avoid](https://www.cio.com/article/3252332/10-project-management-myths-to-avoid.html)

# [工作流引擎在有赞 DevOps 中的实践](https://tech.youzan.com/workflow-engine-in-youzan-devops/)

# [2020 国内公司前端团队都在搞些什么?](https://www.zhihu.com/question/398940598/answer/1269685808)

针对前端基建给了一些很实用的建议。大致可以分为三个阶段

- 规范化、工具化
    - 研发规范，包含代码规范、分支规范与环境管理等
    - 组件化和模板化
    - 用 CLI 集成组件、模板以及文件处理工具来统一代码规范
- 服务化、SOP
    - 接管项目从创建到发布发版流程，深度集成仓库、CI/CD 与环境服务器，工作流化
    - 私有部署的 NPM 服务器，更好管理包
    - 有了包的私有管理和统一工作流，可以做很多检查反馈。如发布代码前的统一静态检查、发布后的统一集成测试检查（ 如无头浏览器 ）、NPM 包依赖关系检查等
    - 生产环境的性能监控及错误报警，就是 APM 和 QoE 那套，结合源码做映射自动定位问题代码（ 像 Sentry ），数据与行为日志录制并回放（ 不能自动定位的问题手动观察 ）
    - 有了告警消息，类似的触达可以做很多事，结合上面的工作流管理，成立研发消息中心来收拢所有变更并做有效通知
    - 基础能力有了，考虑扩大端上范围，如移动端、桌面端
- 去服务化、上云
    - 后台的后台：配置中心、数据中心、基地页、低代码平台
    - 端与端架构：微服务、微前端、独立网关、接口配置与模拟、视图聚合与裁剪

# [当我们在谈论大前端时，我们在谈些什么](https://mp.weixin.qq.com/s/3sAnw1w1b5ZePvlFkBhHzw)
