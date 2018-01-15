---
title: 数组的归并方法
date: 2018-01-10 17:55:52
tags: javaScript-Array
categories:
- 前端基本问题
- 数组
---
**1.reduce()与reduceRight()**  **返回数组项的总和**
<!-- more -->
示例：

```javascript
var values = [1,2,3,4,5];
var sum = values.reduce(function(prev, cur, index , array){
  console.log(prev)
  return prev + cur
});
console.log(sum);

var values = [1,2,3,4,5];
var sum1 = values.reduceRight(function(prev, cur, index , array){
  console.log(prev)
  return prev + cur
});
console.log(sum);
```
