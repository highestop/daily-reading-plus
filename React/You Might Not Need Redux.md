# [You Might Not Need Redux](https://medium.com/@dan_abramov/you-might-not-need-redux-be46360cf367)

- People often choose Redux before they need it。Redux 是繁琐的，或者「 多度设计 」的，所以用它之前要确「 你必须用它 」
- You can apply ideas from Redux without using Redux。例如你大可不必去全局强制使用，可以只在某个模块内使用这种思想编程
- Local state is fine，这一点在用 Angular Service 时的感受尤其多（ 我们把这样的 Service 称为 StateService，一种典型的场景就是 StorageService 用来当做 Store，而与之对应的是 StatelessService 或 LogicService，就可以看做是 Reducer 的集合 ），DI + Rx 完全可以不用 Redux 就可以做到比 Redux 更灵活可用
