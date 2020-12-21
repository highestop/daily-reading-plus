# [You Might Not Need Redux](https://medium.com/@dan_abramov/you-might-not-need-redux-be46360cf367)

- People often choose Redux before they need it。Redux 是繁琐的，或者「 多度设计 」的，所以用它之前要确「 你必须用它 」
- You can apply ideas from Redux without using Redux。例如你大可不必去全局强制使用，可以只在某个模块内使用这种思想编程
- Local state is fine，这一点在用 Angular Service 时的感受尤其多（ 我们把这样的 Service 称为 StateService，一种典型的场景就是 StorageService 用来当做 Store，而与之对应的是 StatelessService 或 LogicService，就可以看做是 Reducer 的集合 ），DI + Rx 完全可以不用 Redux 就可以做到比 Redux 更灵活可用

# [To listen well, get curious](https://www.benkuhn.net/listen/)

- 对于大多数的抱怨，just-listen 是一种「 还不够 」的反应，也包括机械式地回应，有效的聆听来源于对事情背后事实的好奇和关心
- Reality has a surprising amount of detail. 聆听问题时需要尝试去打开那些充满现实细节的「 盒子 」，才能用具有共鸣的语言进行交流
- 作者认为 sometimes people don’t want help, just to be listened to 可能是因为大多数人没有仔细听所以给出了不好的建议，这样反而不如干脆聆听，但 listener 作为 helper 应该做更多
- 非常赞成作者提到的 —— repeat things back to them in my own words，作者的表达是 eflective listening feels validating 以及 putting their idea into my own words shows them that I’ve fully digested it, and helps us establish a shared language in which to talk about it. 用自己的话说出来，不仅表现了你关心的态度，而且是在确认理解无误，在整个对话中保持与对方持有共同语言

# [Why Code Snippets From Stack Overflow Can Break Your Project](https://medium.com/better-programming/why-code-snippets-from-stack-overflow-can-break-your-project-ced579a48ddb)

> 翻译：[为什么 StackOverflow 上的代码片段会摧毁你的项目？](https://mp.weixin.qq.com/s/Q9f5RZqqRB0E-6NmMMwNlw)

- 不要轻易相信粘贴的代码，杜绝不理解问题场景就直接复制粘贴，重用代码的前提是理解它为什么这么写
- 会有什么问题？「 回答 」一个问题的代码也是作者粘贴上去的，很可能省略了问题本身所处的场景信息，如果你再截取一段复制下来，就会更脱离代码最初的上下文
- 怎么使用这些代码？做自己的 TestCase，备注上来源链接便于溯源
