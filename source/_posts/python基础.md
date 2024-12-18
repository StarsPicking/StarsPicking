---
title: python基础
author:
  name: zhangtq
  link: 'https://hexo.zhangtq.com/'
top: false
cover: false
toc: true
mathjax: false
categories: python基础
tags:
  - 你的标签
  - Python
excerpt: >-
  python是一种计算机编程语言以及配套的软件工具和库。Python简单易学，代码十分简洁，它使用强制空白符作为缩进，这大大提高了Python的开发效率，使用Python能够在更短的时间内完成更多的工作。Python是一门开源的语言，并且Python还有许多强大的开源库，这些库使得Python无论是对云计算、大数据、还是人工智能，都有很强的支持能力
abbrlink: 81b2f4bf
date: 2023-06-23 06:52:36
img:
coverImg:
summary:
---

<!--more--> 

python是一种计算机编程语言以及配套的软件工具和库。Python简单易学，代码十分简洁，它使用强制空白符作为缩进，这大大提高了Python的开发效率，使用Python能够在更短的时间内完成更多的工作。Python是一门开源的语言，并且Python还有许多强大的开源库，这些库使得Python无论是对云计算、大数据、还是人工智能，都有很强的支持能力
<!-- more -->
# python知识点

## 列表

### append

```
#1. append用于在列表末尾追加新的对象
a = [1,2,3]
a.append(4)                          #the result ： [1, 2, 3, 4]
```

### count

```
#2. count方法统计某个元素在列表中出现的次数
a = ['aa','bb','cc','aa','aa']
print(a.count('aa'))                 #the result ： 3
```

### extend

```
#3. extend方法可以在列表的末尾一次性追加另一个序列中的多个值
a = [1,2,3]
b = [4,5,6]
a.extend(b)                          #the result ：[1, 2, 3, 4, 5, 6]
```

### index

```
#4. index函数用于从列表中找出某个值第一个匹配项的索引位置
a = [1,2,3,1]
print(a.index(1))                   #the result ： 0
```

这里只是找到第一个匹配项的位置

### insert

```
#5. insert方法用于将对象插入到列表中
a = [1,2,3]
a.insert(0,'aa')            #the result : ['aa', 1, 2, 3]
```

### pop

```
#6. pop方法会移除列表中的一个元素（默认是最后一个），并且返回该元素的值
a = [1,2,3]
a.pop()                             #the result ： [1, 2]
a.pop(0)
```

### remove

```
#7. remove方法用于移除列表中某个值的第一个匹配项
a = ['aa','bb','cc','aa']
a.remove('aa')                      #the result ： ['bb', 'cc', 'aa']
```

### reverse

```
#8. reverse方法将列表中的元素反向存放
a = ['a','b','c']
a.reverse()                         #the result ： ['c', 'b', 'a']
```

### sort

```
#9. sort方法用于在原位置对列表进行排序，意味着改变原来的列表，让其中的元素按一定顺序排列
a = ['a','b','c',1,2,3]
a.sort()                           #the result ：[1, 2, 3, 'a', 'b', 'c']
```

### enumerate

```
li = [11,22,33,44,55,66]
for k,v in enumerate(li, 1):  # 1.代表 k 从哪个数字开始
    print(k,v)
'''
1 11
2 22
3 33
'''
```

### range和xrange

*   指定范围，生成指定的数字
*   注：python3中的range类似python2中的xrange，比如a = range(1,4) : a返回的不是列表对象而是一个可迭代对象（<class 'range'>）

```
#1、range根据start与stop指定的范围以及step设定的步长，生成一个序列：range([start,] stop[, step])
#2、xrange 用法与 range 完全相同，所不同的是生成的不是一个list对象，而是一个生成器
for i in range(1,10,2):
    print(i)
```

### 列表去空

```
# 法1：
filter(None, your_list)

# 法2：
while '' in your_list:
    your_list.remove('')

# 法3：
your_list = [x for x in your_list if x != '']
```

## 元组

*   元组定义：元组和列表一样，也是一种序列，唯一的不同是元组不能修改。

### 创建元组

```
#1. 创建元组
a = (1,2,3,4,5,6)
#2. 将列表转换成元组
tuple([1,2,3,4])                                    #the result ： (1, 2, 3, 4)
```

### 列表和元组常用函数

| 方法 | 作用 |  
|