# 图灵机
[![Github link](https://img.shields.io/badge/FaDrYL--blue?style=social&logo=Github&logoWidth=15)](https://github.com/FaDrYL)
[![Website link](https://img.shields.io/badge/FaDr-YL-blue?style=flat&color=009f9f)](https://www.fadryl.com/)

**Turing Machine (TM)**

图灵机是一种抽象的计算模型。

> **邱奇-图灵论题 （Church-Turing Thesis）**  
> 任意由一个算法定义的函数，都能被图灵机表示。

<br/>

## 组成
- 一条无限长度的纸带（tape）
  - 分割为一个个的小格子，
  - 纸带能被向左或向右移动。
- “输入”的字母表
- “纸带”的字母表
- 一组有限数量的状态
  - 其中一个为开始状态，
  - 一些为结束（接受）状态。
- 一些转移函数
  - `读取 -> 写入, 方向`
    - `读取` 是读取当前格子的字符。
    - `写入` 是将字符写入当前格子。
    - `方向` 是指代的移动方向。 (左 `L` 或右 `R`)
  - `1 -> 0, L`
    - 读取 `1` 并将其替换为 `0`，然后移动到左边的格子。

<br/>

## 定义
对于一个图灵机 *T*：
- `Accept(T)`
  - 在结束（接受）状态停下， 
  - 则该语言被 *T* 接受。
- `Reject(T)`
  - 在接受状态以外的状态停下，或崩溃。
  - 对于当前字符没有合适的转移函数。
- `Loop(T)`
  - 输入使 *T* 一直循环。

<br/>

## 例子
一个 TM 接受：以 `AA` 结尾的语言。

不符合则拒绝。

![TM for aa](../img/TM_aa.png)

