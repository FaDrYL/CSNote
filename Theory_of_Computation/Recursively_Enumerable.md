# Recursively Enumerable
[![Github link](https://img.shields.io/badge/FaDrYL--blue?style=social&logo=Github&logoWidth=15)](https://github.com/FaDrYL)
[![Website link](https://img.shields.io/badge/FaDr-YL-blue?style=flat&color=009f9f)](https://www.fadryl.com/)

A language is recursively enumerable (RE) 
if there exist a TM such that `Accept(T) = L`. 
For the string outside the language, the TM may be `reject` or `loops forever`. (Main difference between RE an R)

Also known as, **Turing recognizable**, **Type 0** (in CNF).

<br/>

## Enumerator
Enumerator is a Turing Machine which can output some strings.

A language `L` is enumerated by an enumerator `M` if:

`L = {all strings in the sequence outputted by M}`

A language is Recursively Enumerable if and only if it is enumerated by some enumerator.

<br/>

## RE And Decidable
If a language and its complement is RE, then this language is also decidable.

Run two enumerators in parallel. 
When either one halts, we can decide it in the language or not.

