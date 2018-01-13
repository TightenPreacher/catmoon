---
title: 数组的倒序与重排序
date: 2018-01-05 09:50:15
tags: javaScript-Array
categories:
- 前端基本问题
- javaScript
---
**1.数组倒序**  **Array.reverse()**

示例：

```javascript
var values = [1,2,3,4,5];
values.reverse();
console.log(values) //5,4,3,2,1
```

**2.数组排序**  **Array.sort()**

示例：

```javascript
function compare(value1,value2) {
    if (value1<value2) {
        return 1;
    } else if (value1>value2) {
        return -1;
    } else {
        return 0;
    }
}

var values = [0,1,5,10,9];
values.sort(compare);
console.log(values); //10, 9, 5, 1, 0
```