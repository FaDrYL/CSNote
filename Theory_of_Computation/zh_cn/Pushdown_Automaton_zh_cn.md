# 下推自动机
[![Github link](https://img.shields.io/badge/FaDrYL--blue?style=social&logo=Github&logoWidth=15)](https://github.com/FaDrYL)
[![Website link](https://img.shields.io/badge/FaDr-YL-blue?style=flat&color=009f9f)](https://www.fadryl.com/)

**Pushdown Automaton (PDA)**

下推自动机像是一个带有**栈**数据结构的 **NFA**。

它能用于呈现 CFG，同时也能呈现 CFL。

<br/>

## 组成部分
- 用于输入的字母表
- 用于栈的字母表
- 一组状态
  - 其中一个为开始状态
  - 一些（或没有）为结束（接受）状态
- 输入纸带（Input tape）
  - 单方向读取（从左到右）
- 栈
  - 用于记忆
  - 可以有两个操作:
    1. Push (将物品加入栈顶)
    2. Pop (移出栈顶的物品)
- 一组转移函数
  - 以此形式表示: `a, b -> c` (任意的字符都可以是 `Ɛ`)
    - 从输入纸带读取 `a`。
    - 如果 `b` 在栈顶，则将其移出。
    - 然后，将 `c` 加入栈顶。
    
<br/>

## CFG 转换为 PDA
> 如何根据 CFG 得出相应的 PDA？

对于语言“回文”，我们有个 CFG：

```
S -> aSa          (1)
S -> bSb          (2)
S -> a            (3)
S -> b            (4)
S -> Ɛ            (5) 
```

我们能为此写出一个对应的 PDA：

![PDA of PALINDROME](../img/PDA_PALINDROME.png)

