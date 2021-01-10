# [Errors and Error Handling in JavaScript](https://blog.bitsrc.io/errors-and-error-handling-in-javascript-52d448b8183d)

# [You don't have to be busy to be prolific](https://thesephist.com/posts/momentum/)

# [It's Not Just Standing Up: Patterns for Daily Standup Meetings](https://www.martinfowler.com/articles/itsNotJustStandingUp.html)

> 阅读来源：https://github.com/daily-reading/daily-reading/tree/main/2020/12/9

整体感受这篇文章读起来非常有结构性

先要明确站会的目的：

- 交流对共同目标的理解，提出问题并讨论改进方案
- 让大家意识到是一个团队，在相互协作中互相认可

两种维度的站会：

- 按人来（ All-Hands ）。这是我们目前多数站会的方式，但正因为每个人都要直接参与，所以要强调站会的原则
- 按事来（ Story-focused ）。以项目工作为粒度来组织，但可能不利于表达部分被动或害羞者的想法

聊的几件事：

- 昨天完成的工作（ Yesterday ）
- 是否有 block 的事情，是什么问题（ Obstacles ）
- 今天的目标（ Today ）

待解决事项看板（ Improvement/Impediment/Blockage Board ）

- 需要描述


# [Understanding Linux CPU Load](https://scoutapm.com/blog/understanding-load-averages)

> 阅读来源：https://github.com/daily-reading/daily-reading/tree/main/2020/12/20

- 用桥上交通的比喻来理解 Linux CPU load average，排队过桥的车辆就好比进程
- 单核边界值 1 表示车满了，小于 1 则有空余可以随时过桥，大于 1 表示桥过载需要排队等待。通常会有个 0.7 的界限，小于 0.7 表示还不需要关注
- 对于多核，1 的单位要乘以相应的倍数。1 只是一条路一座桥的度量，多核就是多条路。所以 3 对于四核来说是 ok 的
- 多核场景下「 核 」是个上限，两个四核、四个双核、一个八核是一样的
- 一般 load average 有三个指标供参考，分别是一分钟、五分钟和十五分钟内的平均值，不同 case 下关注的点不同
