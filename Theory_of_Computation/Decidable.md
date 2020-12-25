# Decidable Language
[![Github link](https://img.shields.io/badge/FaDrYL--blue?style=social&logo=Github&logoWidth=15)](https://github.com/FaDrYL)
[![Website link](https://img.shields.io/badge/FaDr-YL-blue?style=flat&color=009f9f)](https://www.fadryl.com/)

For a language that can use finite number of steps (halt on all inputs in finite number of steps) to decide the membership, 
we call that decidable language.

Also known as recursive language.

<br/>

## Decider
Decider is a TM (or algorithm) such that halts on all input and has one of these results:
- YES (Accept), or
- NO (Reject).

<br/>

## Decidable Problem
If we can find a decider for a problem, we can say it is a decidable problem.

### For example
> Input: Two regular expression.  
> Question: Do they define a same language?

It is decidable, hence we can write a decider to solve it.

1. We write two NFAs, *N1* and *N2*, for these two RegEx.
2. Simplify these two NFAs to FAs (*N1* -> *F1* and *N2* -> *F2*).
3. Compare states and transitions of these two FAs.
4. If they are same, return YES. Otherwise, NO.

<br/>

## Closure Properties
If `L` is decidable, `~L` is also decidable by flip the result.

Also, if `A` and `B` are decidable, then also

- `A ∩ B`
- `A ∪ B`
- `AB`

<br/>

## 
