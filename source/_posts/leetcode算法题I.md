---
title: leetcode算法题I
author:
  name: zhangtq
  link: 'https://hexo.zhangtq.com/'
top: false
cover: false
toc: true
mathjax: false
categories: leetcode算法题I
tags:
  - 你的标签
  - 算法
excerpt: 顺序整理leetcode热门算法题，通过实际的题目提升算法水平，加强思维能力
abbrlink: f97434cd
date: 2023-06-29 00:45:21
img:
coverImg:
summary:
---

<!--more--> 

顺序整理leetcode热门算法题，通过实际的题目提升算法水平，加强思维能力
<!-- more -->
# 常见算法题

## 基础算法

### 求两数之和

> 给定一个整数数组 nums 和一个整数目标值 target，请你在该数组中找出 和为目标值 target 的那 两个 整数，并返回它们的数组下标。你可以假设每种输入只会对应一个答案。但是，数组中同一个元素在答案里不能重复出现。你可以按任意顺序返回答案。

*   可以直接暴力两个循环查找，时间复杂度为O(N2)
*   下面的代码主要是通过空间换时间的思想，利用hashmap来降低时间复杂度

### 无重复最长字串

> 给定一个字符串 `s` ，请你找出其中不含有重复字符的 **最长子串** 的长度。
> 
> **示例 1:**
> 
> ```
> 输入: s = "abcabcbb"
> 输出: 3 
> 解释: 因为无重复字符的最长子串是 "abc"，所以其长度为 3。
> ```
> 
> **示例 2:**
> 
> ```
> 输入: s = "bbbbb"
> 输出: 1
> 解释: 因为无重复字符的最长子串是 "b"，所以其长度为 1。
> ```
> 
> **示例 3:**
> 
> ```
> 输入: s = "pwwkew"
> 输出: 3
> 解释: 因为无重复字符的最长子串是 "wke"，所以其长度为 3。
>      请注意，你的答案必须是 子串 的长度，"pwke" 是一个子序列，不是子串。
> ```
> 
> **提示：**
> 
> *   `0 <= s.length <= 5 * 104`
> *   `s` 由英文字母、数字、符号和空格组成

### 最长回文字串

![image-20230629142155556](https://zhangtq-blog.oss-cn-hangzhou.aliyuncs.com/content_picture/image-20230629142155556.png)

image-20230629142155556