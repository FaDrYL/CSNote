# 递归可枚举语言
[![Github link](https://img.shields.io/badge/FaDrYL--blue?style=social&logo=Github&logoWidth=15)](https://github.com/FaDrYL)
[![Website link](https://img.shields.io/badge/FaDr-YL-blue?style=flat&color=009f9f)](https://www.fadryl.com/)

**Recursively Enumerable (RE) **

一个语言是 递归可枚举语言，如果存在一个满足 `接受 Accept(T) = L` 的图灵机。
且当一个字符串不属于这个语言时，这个图灵机会 `拒绝 reject` 或 `一直循环 loops forever`。（RE 和 R 的主要区别）

也称之为，**图灵可识别 Turing recognizable**，**Type 0** (CNF 形式).

<br/>

## 枚举器
**Enumerator**

枚举器是一个可以输出一组字符串（单词）的图灵机。

一个语言 `L` 是由枚举器 `M` 枚举的，只有：

`L = {所有的单词都由 M 枚举}`

当且仅当某种枚举器枚举某语言时，该语言才可以递归可枚举语言。

<br/>

## 递归可枚举语言与可判定语言（递归语言）
当一个语言及其补集都是递归可枚举的，则这个语言是可判定语言。

并行运行这两个枚举器，
当其中一个停止时，我们可以决定当前单词属于或不属于这个语言。

