---
layout: post
title: "String Helper Functions"
date: 2025-10-09
categories: [Programming]
tags: [c, strings, helpers]
---

In embedded systems, writing safe and lightweight string helper functions
saves time and increases code reliability.

Here are some simple string helpers frequently used in low-level C projects:

```c
int str_len(const char *s)
{
    int n = 0;
    while (*s++) n++;
    return n;
}

void str_copy(char *dest, const char *src)
{
    while ((*dest++ = *src++));
}
