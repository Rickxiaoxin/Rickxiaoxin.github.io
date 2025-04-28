---
date: "2025-04-12T10:11:19+08:00"
draft: true
title: 对象和变量
---


# 对象
Object是一个能够存储值的存储区域（通常是内存）

# 变量初始化
## 变量初始化
### 复制初始化
```
    int a = 5;
```

允许向下转换

### 直接初始化
```
    int a(5);
```

允许向下转换

### 列表初始化
```
    int a{5};
```

允许对列表的值进行初始化

不允许向下转换

## 值初始化和零初始化

```
    int width {};
    int width {0};
```

## [[maybe_unused]]
允许编译器接受未使用的变量，不生成警告

```
    [[maybe_unused]] double pi {3.14};
```


## Reference
1. [learncpp](https://www.learncpp.com/)
