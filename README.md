# Daily Reading Plus

2020 年 10 月起，加入了 [Daily-Reading](https://github.com/daily-reading/daily-reading) 组织，来督促自己每天进行一些英文阅读。这个仓库也是受到这件事的启发，想做更多的阅读和学习记录。这里不限语言和话题，大多数是技术成长为主的，也有个人成长、生活自律等

这里也分享一下自己长久以来坚持阅读的一点点小经验：

- **找到文章**。Push（ 主动搜 ）/ Pull（ 被动收到推送 ）是两条途径。无论是哪种，都要总结出内容、数量均适合自己的渠道。在 [Daily-Reading](https://github.com/highestop/Daily-Reading) 仓库中的 Issues 就是阅读清单。除了 Github Web 或邮件的 Subscription Notification 外，还可以定时用 Github 的 API 拉取 Opened Issues 列表 `curl -i "https://api.github.com/repos/daily-reading/daily-reading/issues`、解析 Content 中的链接、[Add 到 Pocket 的 API 中去](https://getpocket.com/developer/docs/v3/add)，傻瓜式完成同步（ 也许是多余的 ）
- **收录到 Pocket 中**。Chrome 和 Safari 都有 Pocket 插件，iPhone 上写了个 Shortcuts 放在通知栏顶部，这样就不用关闭 App 了
- **制作清单**。固定时间（ 如上下班通勤时、午餐后遛弯时 ）将 My List 中的文章分类（ 打 Tags ），并将今天想要读的文章归到 Favorites 中
- **随时随地进行阅读** —— 通过筛选 Favorites & My List 找出目标然后 be focused 去阅读它们。Pocket 有一个 tricky 的好处就是它的 Article Mode 可以阅读 Medium 订阅文章的全文。读完记得 Archive 掉
- **笔记归档**。睡觉前会将写下来的阅读笔记整理发布到仓库中，并去 Pocket 看下大概剩了多少。尽量一天的任务一天完结，越攒越多会让自己有压力，而且堆积起来之后 Read-It-Later 就会变成 Read-It-Never —— 据我来看这个时间不会超过 3 天

希望大家都能找到一种形式让自己养成阅读的好习惯~

## ChangeLogs

- **2021.1.25**：考虑到阅读和笔记的便捷性和舒适性，不再将每一篇阅读文章提交到仓库，转移到本地
- **2021.2.18**：会每月发布一份阅读报告，公布这段时间阅读的所有有价值的文章（ Pocket 中真正读的显然要比这个多，不是所有收录都有价值放出来 ）
