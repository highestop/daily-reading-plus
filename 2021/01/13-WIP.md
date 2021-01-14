# [Building On-Call Culture at GitHub](https://github.blog/2021-01-06-building-on-call-culture-at-github/)

> 阅读来源：https://github.com/daily-reading/daily-reading/tree/main/2021/1/8

# [微信十年，数字化转型的「 大江大河 」](https://mp.weixin.qq.com/s/lHs-Q-qYeY-xOMhlI1MrCQ)

- 数字化转型
- 如何优化配置稀缺资源，始终是经济学研究的重要议题
- 如果说工业化的魅力是将人们从重复体力劳动中解放出来，那么数字化的魅力就在于让整个社会不再受地理空间范围的限制
- 平台具备快速孵化和培养更多小生态的能力
- 数字孪生（ Digital Twin ）并非简单的平移和复制，它的真实目标是转型和升级

# [瑞幸教会咖啡行业的事](https://mp.weixin.qq.com/s/g2aiR-Kb6hv9mT3gAg-CSQ)

- 咖啡店是消费者在家和办公室以外用到的临时空间 —— 星巴克创始人霍华德·舒尔茨（ Howard Schultz ）的 “第三空间” 理论
- 单位经济模型 UE（ Unit Economics ）—— 日销额 × 毛利率 - 人力成本 - 物流成本 - 实体店铺成本
- 用户的复购率和留存率
- 各环节尽可能标准化
- 私域流量运营，非分众广告主

# [值得信赖的合作伙伴](https://mp.weixin.qq.com/s/uCH2wnrpQvdFf97ICSaXAA)

- 信任 =（ 可信度 + 可靠度 + 亲近度 ）/ 自我导向（ 自我利益为中心的动机 ） —— 《 值得信赖的顾问 》
- 提高可信度：
    - 彰显专业性，用硬实力说话
    - 积极主动表达，热心帮助，心态放平
    - 谦虚谨慎，做事说话适度，不要虚有其表
- 提高可靠度：
    - 言必信行必果，做事让人放心
    - 在小事上也能驻守承诺
- 提升亲近度
    - 坦诚
    - 相互尊重
    - 深度表达好奇或关心（ 保持好奇才能有效聆听 ）
    - 不对立，换位思考，理性看待冲突
- 消除自我导向
    - 少掌控话题，多聆听
    - 补位、合作精神
    - 鼓励失败
- 信赖的建立是多方面的，不仅仅是 nice to have

# [领域模型 vs 数据模型，应该怎么用？](https://mp.weixin.qq.com/s/Wt2Fssm8kd8b8evVD9aujA)

- 领域模型：领域知识，业务实体，概念及其之间的关系。形态是显性表达业务语义
- 数据模型：数据存储，强调罗占星、性能等非业务功能属性

领域是核心，围绕数据的是技术细节

![](https://mmbiz.qpic.cn/mmbiz_jpg/Z6bicxIx5naKibkYRKlteh0EeWBbhYkdEmCpIBgUiav8ka7JnxyqOPH1RhHeUx2TGicia1CtpbsUx6dLHu4CcFiaJcOg/640)

一种让领域模型和数据模型各司其职的手段是，利用一层 gateway 做转译、解耦和防腐

![](https://mmbiz.qpic.cn/mmbiz_jpg/Z6bicxIx5naKibkYRKlteh0EeWBbhYkdEmh5uicbPolPicNFmmgGj2oORRKiaoBkzXdsyqcEclvSyqclmIXvZ8D62oA/640)

扩展：在业务领域模型未知的情况下做好数据模型的扩展。参考 Salesforce 的匿名字段表，元数据驱动，描述业务表意，支撑上面的 SaaS 业务

延伸阅读：https://github.com/alibaba/COLA

# [2021 年前端趋势预测](https://mp.weixin.qq.com/s/OAKvV3HHkIEnzXdvuiCkuA)

- Deno 开创的 Http Module Import 技术，把 CJS 转 ESM 都交给 CDN 类的服务来做，通过代码地址来引用代码，运行时引入执行，取代编译前引入解析
    - [2021 再看 Deno（ 关于 CDN for JavaScript Modules 的思考）](https://mp.weixin.qq.com/s/EzmNQ_oqxUuPQFfZYJWDzA) 这篇文章提到，其实 Http Import 很可能也是低代码可视化编排系统的一个基础，否则扩展性太差了。ESM.Run 是一个将 NPM 或 Github 代码直接托管到 S3 CDN 上的方案
- 逻辑编排，以函数为粒度，可视化流程。这一点可以延伸到系统的低代码上，无非就是提炼业务领域模型、创建一套语义描述业务领域知识、可视化编排语义树和数据，从而直接生成业务系统
- 智能 UI 精细化。[智能 UI：面向未来的 UI 开发技术](https://mp.weixin.qq.com/s/1RNEQb8N68Muu6YmFa-QrQ)、[CBU 智能 UI 落地最佳实践](https://juejin.cn/post/6889305339172323336)。很多是站在 P2C 基础上的，PD 标注体系是个大工程，需要站在 PD 角度理解，但这里的建模思考非常有价值