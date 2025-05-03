---
date: '2025-05-03T15:32:17+08:00'
draft: true
title: 'Delegating Constructor'
---

委托构造函数调用同一类的另一个构造函数，通过添加执行初始化步骤的函数来减少重复代码。

```
struct A {
int a;
float b;
bool c;
// standard constructor:
A(int a1, float b1, bool c1) : a(a1), b(b1), c(c1) {
// do a lot of work
}
A(int a1, float b1) : A(a1, b1, false) {} // delegate construtor
A(float b1) : A(100, b1, false) {} // delegate construtor
};
```
