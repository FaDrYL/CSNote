# 可判定语言
[![Github link](https://img.shields.io/badge/FaDrYL--blue?style=social&logo=Github&logoWidth=15)](https://github.com/FaDrYL)
[![Website link](https://img.shields.io/badge/FaDr-YL-blue?style=flat&color=009f9f)](https://www.fadryl.com/)

**Decidable Language**

对于一个可以用有限步数（对于所有的输入，于有限的步骤数停下）来进行识别其成员的语言，我们称其为**可判定语言**。

也称之为：递归语言（**recursive language**）。

<br/>

## 判定器
**Decider**

判定器是一个图灵机（或算法），它能于所有的输入停下，并会产生其中一个结果：
- 是 (接受), 或
- 否 (拒绝).

<br/>

## 可判定问题
**Decidable Problem**

如果我们能为一个问题找到一个判定器，那么这个问题就是可判定问题。

### 例子
> 输入: 两个正则表达式。  
> 问题: 它们是否定义一个相同的语言？

这是一个可判定问题，因为我们能为其写出一个判定器来解决它。

1. 我们根据输入的两个正则表达式来写出它们的 NFA（*N1* 和 *N2*）。
2. 将这两个 NFA 简化为 FA （*N1* -> *F1* 以及 *N2* -> *F2*）。
3. 对比这两个 FA 的状态和转移函数。
4. 如果它们相同，则同意。否则，拒绝。

<br/>

## 闭包性质
如果 `L` 是可判定语言，通过将结果反转，`~L` 也是可判定语言。

同时，如果 `A` 和 `B` 都是可判定语言，则以下亦然：

- `A ∩ B`
- `A ∪ B`
- `AB`

