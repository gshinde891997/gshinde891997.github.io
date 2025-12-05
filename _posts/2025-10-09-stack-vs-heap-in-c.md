---
layout: post
title: "Stack VS Heap in C"
date: 2025-10-09
categories: [Programming]
tags: [c, memory, stack, heap]
---

Understanding how **stack** and **heap** memory work is critical for embedded developers.

## 🔹 Stack Memory
- Fast, automatically managed  
- Stores local variables, function parameters, return addresses  
- Memory is freed when function exits  
- Limited size → stack overflow possible  

Example:

```c
void func()
{
    int x = 10;   // stored on stack
}
