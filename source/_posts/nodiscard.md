---
title: nodiscard in C++
date: 2023-11-12 19:51:47
tags: c++
---

The `[[nodiscard]]` attribute is a part of C++17 and onwards, which signals the compiler to issue a warning if the return value of a function is ignored. This attribute can be applied to functions, enumerations, and classes.

<!-- more -->

## Usage

1. To annotate a function to ensure its return value is not ignored:

```cpp
[[nodiscard]] int compute();
```

2. To annotate an enumeration or class so that when its object is returned by a function, it should not be ignored:

```cpp
class [[nodiscard]] ImportantResult {...};
```

3. Since C++20, a string literal can be provided to explain why the return should not be ignored:

```cpp
[[nodiscard("Reason for not discarding")]] int performAction();
```

## When Is a Warning Issued?

A warning is encouraged to be issued by the compiler in the following cases:

- A function declared with `[[nodiscard]]` is called and its value is not used.
- An object of a class or enumeration declared with `[[nodiscard]]` is initialized and not used.
- In C++20, if a string literal is provided with the `[[nodiscard]]` attribute, it is usually included in the warning message issued by the compiler.

## Purpose

The purpose of the `[[nodiscard]]` attribute is to catch potential bugs where a function's return value, which might be significant, is accidentally ignored.
