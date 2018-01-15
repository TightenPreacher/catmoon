---
title: 数组的迭代方法
date: 2018-01-10 13:25:52
tags: javaScript-Array
categories:
- 前端基本问题
- 数组
---
**1.every()**  **判断数组所有项是否符合条件**
<!-- more -->
示例：

```javascript
var numbers = [1,2,3,4,5,4,3,2,1];
var everyResult = numbers.every(function(item, index , array){
  return (item > 2)
});
console.log(everyResult);
```

**2.some()**  **判断数组某项是否符合条件**

示例：

```javascript
var numbers = [1,2,3,4,5,4,3,2,1];
var someResult = numbers.some(function(item, index , array){
  return (item > 2)
});
console.log(someResult);
```
**3.filter()**  **筛选数组返回出符合条件的项**

示例：

```javascript
var numbers = [1,2,3,4,5,4,3,2,1];
var filterResult = numbers.filter(function(item, index , array){
  return (item > 2)
});
console.log(filterResult);
```

**4.map()**  **返回对数组运算后的结果**

示例：

```javascript
var numbers = [1,2,3,4,5,4,3,2,1];
var mapResult = numbers.map(function(item, index , array){
  return (item * 2)
});
console.log(mapResult);
```

**5.forEach()**  **等同for循环迭代数组**

示例：

```javascript
var numbers = [1,2,3,4,5,4,3,2,1];
numbers.forEach(function(item, index , array){
  //执行某些操作
});
```

