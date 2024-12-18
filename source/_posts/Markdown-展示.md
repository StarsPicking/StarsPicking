---
title: Markdown 展示
author:
  name: zhangtq
  link: 'https://hexo.zhangtq.com/'
top: false
cover: false
toc: true
mathjax: false
categories: Markdown 展示
tags:
  - 你的标签
  - 使用指南
excerpt: >-
  VuePress 主要从 Markdown 文件生成页面。因此，你可以使用它轻松生成文档或博客站点。 你需要创建并编写 Markdown，以便
  VuePress 可以根据文件结构将它们转换为不同的页面。
abbrlink: 81a1a517
date: 2024-12-11 17:41:15
img:
coverImg:
summary:
---

<!--more--> 

VuePress 主要从 Markdown 文件生成页面。因此，你可以使用它轻松生成文档或博客站点。 你需要创建并编写 Markdown，以便 VuePress 可以根据文件结构将它们转换为不同的页面。
<!-- more -->
VuePress 主要从 Markdown 文件生成页面。因此，你可以使用它轻松生成文档或博客站点。

你需要创建并编写 Markdown，以便 VuePress 可以根据文件结构将它们转换为不同的页面。

## Markdown 介绍

如果你是一个新手，还不会编写 Markdown，请先阅读 [Markdown 介绍](https://theme-hope.vuejs.press/zh/cookbook/markdown/) 和 [Markdown 演示](https://theme-hope.vuejs.press/zh/cookbook/markdown/demo.html)。

## Markdown 配置

VuePress 通过 Frontmatter 为每个 Markdown 页面引入配置。

Frontmatter

Frontmatter 是 VuePress 中很重要的一个概念，请阅读 [Frontmatter 介绍](https://theme-hope.vuejs.press/zh/cookbook/vuepress/page.html#front-matter) 了解详情。

## Markdown 扩展

VuePress 会使用 [markdown-it](https://github.com/markdown-it/markdown-it) 来解析 Markdown 内容，因此可以借助于 markdown-it 插件来实现 [语法扩展](https://github.com/markdown-it/markdown-it#syntax-extensions) 。

### VuePress 扩展

为了丰富文档写作，VuePress 对 Markdown 语法进行了扩展。

关于这些扩展，请阅读 [VuePress 中的 Markdown 扩展](https://theme-hope.vuejs.press/zh/cookbook/vuepress/markdown.html)。

### 主题扩展

通过 VuePress 插件，主题扩展了更多 Markdown 语法，提供更加丰富的写作功能。

#### 选项卡

*   [查看详情](https://theme-hope.vuejs.press/zh/guide/markdown/content/tabs.html)

#### 脚注

此文字有脚注[\[1\]](#footnote1).

*   [查看详情](https://theme-hope.vuejs.press/zh/guide/markdown/content/footnote.html)

#### 导入文件

*   [查看详情](https://theme-hope.vuejs.press/zh/guide/markdown/content/include.html)

#### TeX 语法

$$  
\\frac {\\partial^r} {\\partial \\omega^r} \\left(\\frac {y^{\\omega}} {\\omega}\\right)  
\= \\left(\\frac {y^{\\omega}} {\\omega}\\right) \\left{(\\log y)^r + \\sum\_{i=1}^r \\frac {(-1)^i r \\cdots (r-i+1) (\\log y)^{r-i}} {\\omega^i} \\right}  
$$

*   [查看详情](https://theme-hope.vuejs.press/zh/guide/markdown/grammar/math.html)

#### 任务列表

*    计划 1
*    计划 2

[查看详情](https://theme-hope.vuejs.press/zh/guide/markdown/grammar/tasklist.html)

### 图片增强

支持为图片设置颜色模式和大小。

*   [查看详情](https://theme-hope.vuejs.press/zh/guide/markdown/grammar/image.html)

#### 上下角标

19th H2O

*   [查看详情](https://theme-hope.vuejs.press/zh/guide/markdown/stylize/sup-sub.html)

#### 组件