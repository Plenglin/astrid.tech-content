---
title: The coding interview at Facebook
date: 2021-02-27 22:29:00-08:00
description: Part 2
tags:
  - job-interview
  - facebook
  - data-structures
---

In [Part 1](https://astrid.tech/2021/04/02/facebook-internship/), . Today, I'll talk about 

## Content

As described before, there are 2 coding interviews for software engineering and 1 coding interview for production engineering. They're all essentially the same structure: 2 questions, one that's Leetcode easy and another that's Leetcode medium or hard. They cover data structures and algorithms stuff, including:

- Iteration
- Recursion
- Arrays
- Lists
- Stacks
- Trees
- Maps
- ... and more!

Thankfully, they did not cover any dynamic programming stuff. I'm terrible at dynamic programming.

You are allowed to program in C++, Java, or Python., but of course, I chose Python. The code does not need to be syntactically correct, and the code will not be run, either; the test is in how you talk through your thought process with the engineer that you're interviewing with.

### First SWE Interview

In the first software engineering interview, the second question I was given was to [serialize and deserialize a binary tree](https://leetcode.com/problems/serialize-and-deserialize-binary-tree/). This is a Leetcode "hard" question.

> Design an algorithm to serialize and deserialize a binary tree. There is no restriction on how your serialization/deserialization algorithm should work. You just need to ensure that a binary tree can be serialized to a string and this string can be deserialized to the original tree structure.

### Second SWE Interview

In the first software engineering interview, the second question I was given was to [serialize and deserialize a binary tree](https://leetcode.com/problems/serialize-and-deserialize-binary-tree/). This is a Leetcode "hard" question.

> Design an algorithm to serialize and deserialize a binary tree. There is no restriction on how your serialization/deserialization algorithm should work. You just need to ensure that a binary tree can be serialized to a string and this string can be deserialized to the original tree structure.

### Production Engineering Interview

The question given here was the [word search](https://leetcode.com/problems/word-search/) problem, which is LeetCode medium:

> Given an `m` x `n` grid of characters board and a string word, return `true` if word exists in the grid.
>
> The word can be constructed from letters of sequentially adjacent cells, where adjacent cells are horizontally or vertically neighboring. The same letter cell may not be used more than once.

I recognized the solution to be finding the first character of the word, followed by a recursive floodfill-like algorithm where you search for the other letters of the word.

But the next part of this was related: instead of returning `true`, return the number of times the word shows up in the grid. At first, my mind went very far to construct some kind of graph, and do some wacky graph-related stuff, but then I eventually realized that you could just replace every `return False` with `return 0`, every `return True` with `return 1`, and every `or` with a `+`, and
