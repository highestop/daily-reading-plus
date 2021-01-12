# [Errors and Error Handling in JavaScript](https://blog.bitsrc.io/errors-and-error-handling-in-javascript-52d448b8183d)

> 阅读来源：https://github.com/daily-reading/daily-reading/tree/main/2020/12/15

# [AST for JavaScript developers](https://itnext.io/ast-for-javascript-developers-3e79aeb08343)

> 翻译：[平庸前端码农之蜕变 — AST](https://juejin.cn/post/6844903725228621832)

AST 抽象语法树，CST 具象语法树

先是词法分析，也叫扫描器 scanner。然后是语法分析，也叫解析器。这跟大学时代写的编译原理大作业很像啊..

Babel 借助 AST，通过解析（ parsing ）、转译（ transforming ）、生成（ generation ）三个步骤，最终生成新代码

这些有助于开发 babel-plugin，也有助于编写一些代码工具

- CodeMods 描述代码要被转换为什么样，如 [ReactCodeMod](https://github.com/reactjs/react-codemod)
- FB 的 [JSCodeShift](https://github.com/facebook/jscodeshift)，用来跑 mods（ 这个词通常在各个领域表达为「 模型 」 ）

还可以将代码可视化地展现为流图，如 [js-code-to-svg-flowchart](https://github.com/Bogdan-Lyashenko/js-code-to-svg-flowchart)，这里[预览](https://bogdan-lyashenko.github.io/js-code-to-svg-flowchart/docs/live-editor/index.html)

# [WRITING A BABEL PLUGIN WITH GRANDMA](https://stephencook.dev/blog/writing-a-babel-plugin-with-grandma/)

介绍了一个简单的例子展示 How to Write a Custom Babel Plugin

思路大致就是，定制一些自己的 Visitor，然后在语法树中通过 traverse 遍历、使用这些 visitors

> I made my own babel plugin so I can stop writing JSX and just write emoji instead.
>
> 这是一个愿景，即可以创建自己的语法集来书写代码
