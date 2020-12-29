# [TypeScript: Stop Using 'any'](https://thoughtbot.com/blog/typescript-stop-using-any-there-s-a-type-for-that)

- TS 是静态编译，提前检查类型，any 违背了防御性代码的初衷
    - 从某个层面讲，和单测是一个作用
- 写代码成本低但阅读和维护成本高
    - 在编写代码时「 记录代码 」
- 只有在对接第三方库、且它没有提供接口定义时，允许用 any
    - 表示 nothing-to-see-here
