# [Errors and Error Handling in JavaScript](https://blog.bitsrc.io/errors-and-error-handling-in-javascript-52d448b8183d)

# [You don't have to be busy to be prolific](https://thesephist.com/posts/momentum/)

# [It's Not Just Standing Up: Patterns for Daily Standup Meetings](https://www.martinfowler.com/articles/itsNotJustStandingUp.html)

# [To listen well, get curious](https://www.benkuhn.net/listen/)

# [Modern storage is plenty fast. It is the APIs that are bad.](https://itnext.io/modern-storage-is-plenty-fast-it-is-the-apis-that-are-bad-6a68319fbc1a)

# [How Netflix Scales its API with GraphQL Federation (Part 1)](https://netflixtechblog.com/how-netflix-scales-its-api-with-graphql-federation-part-1-ae3557c187e2)

# [How Netflix Scales its API with GraphQL Federation (Part 2)](https://netflixtechblog.com/how-netflix-scales-its-api-with-graphql-federation-part-2-bbe71aaec44a)

# [Understanding Linux CPU Load](https://scoutapm.com/blog/understanding-load-averages)

作者用桥上交通的比喻对 Linux CPU load average 的理解

- 一般 load average 有三个指标供参考，分别是一分钟、五分钟和十五分钟内的平均值
- 先是单核场景下
    - 排队过桥的车辆就好比等待 CPU 的进程
    - 边界值 1 表示车满了，小于 1 则有空余可以随时过桥，大于 1 表示桥过载需要排队等待
    - 通常会有个 0.7 的界限，小于 0.7 表示还不需要关注
- 对于多核，1 的单位要乘以相应的倍数。1 只是一条路一座桥的度量，多核就是多条路。所以 3 对于四核来说是 ok 的
- 多核场景下「 核 」是个上限，两个四核、四个双核、一个八核是一样的
