---
title: aboutData
date: 2018-01-31 15:08:29
tags: javaScript-Date()
categories:
- 前端基本问题
- Data类型
---

**`Date类型，基于Java.util.Date类基础上构建`**

**1-基本用法**

```javascript
var now = new Date()  //获取当前日期与时间
```

**2-Date.parse()**

​	Date.parse()接受一个表示日期的字符串参数，返回相应日期的毫秒数。如：

```javascript
Date.parse("1/31/2018") 	// 月/日/年
Date.parse("January 25,2018")	// 英文月名 日,年
Date.parse("Tue May 25 2018 12:12:12 GMT-0700") 	//英文星期几 英文月名 日 年 时:分:秒 时区
Date.parse("2018-02-13T00:00:00") 	//ES5 ISO 8601 扩展格式 YYYY-MM-DDTHH:mm:ss.sssZ
```

​	如传入字符串不能表示日期，则返回`NaN`，如果直接传给Date()，也会调用Date.parse()。则:

```javascript
var someDate = new Date("January 25,2018") 		//与上述例子等同
```

**3-Date.UTC()**

​	Date.UTC()的参数分别是年份、基于0的月份、月中的某一天、小时数、分钟、秒、毫秒数。只有年月是必须的。

```javascript
var y2k = new Date(Date.UTC(2000,0));		//GTM 时间 2000年1月1日午夜零时
var allFives = new Date(Date.UTC(2005,4,5,17,55,555)); 		//GTM 时间 2005年5月5日下午5:55:55
```

