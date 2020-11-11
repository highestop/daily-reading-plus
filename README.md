# Daily Reading Plus

最近加入了 [Daily-Reading](https://github.com/highestop/Daily-Reading) 督促自己每天进行一些英文阅读，这个仓库也是受到这件事的启发

不同之处是，我只会将**自己读过**的、认为**有一定价值**的**文章链接**放到这里来 —— 每篇都写读书笔记或都将读书笔记粘到这里是件不太值得做的事。这里不局限于语言、话题，当然大多数都是技术成长为主的。**提一点小要求：尽量能用一两句话概括描述每篇文章的内容或感受，也就是 TL;DR**

另外也分享一下自己长久以来做阅读的方式：

- 找到文章。Push/Pull 是两条途径，感觉一定要有自己的渠道，但又不能太多
- 用工具收藏到 Pocket 服务中 —— Chrome 和 Safari 都有 Pocket 插件，iPhone 上自己写了个 Shortcuts 脚本然后将捷径放在通知栏中，这样不用关闭 App 就可以完成收录。另外，我们在 [Daily-Reading](https://github.com/highestop/Daily-Reading) 仓库中用 Issues 管理着阅读清单，可以定时用 Github 的 API 拉取 Opened Issues 列表 `curl -i "https://api.github.com/repos/daily-reading/daily-reading/issues`、解析 Content 中的链接、[Add 到 Pocket 的 API 中去](https://getpocket.com/developer/docs/v3/add)，傻瓜式完成同步
- 每天有固定的时间（ 如上下班通勤时、午餐后 ）将 My List 中的文章打上 Tags（ 分类很重要 ），并且将今天想要读的文章归到 Favorites 中
- 随时随地进行阅读 —— 可以快速通过筛选 Favorites & My List 得到当前的 TodoList 然后专注于阅读它们。读完的文章会被 Archive 掉
- 最后在睡觉前，会大概看下 TodoList 剩了多少，尽量一天的任务一天完结吧，否则堆积起来之后 Read-It-Later 就会变成 Read-It-Never —— 这个时间不会超过 3 天

希望大家都能找到一种形式让自己养成阅读的好习惯

让我们把墙刷起来吧！cheers~