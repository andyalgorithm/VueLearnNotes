# 基本运算

`Math.max(a, b)`

`Math.min(a, b)`



### 排序

```js
// 从小到大排序
var arr = [6, 4, 1, 8, 2, 11, 23];
arr.sort(function(a,b){return a - b;});
```



### 求数组中最大值

```js
var arr = [6, 4, 1, 8, 2, 11, 23];
console.log(Math.max.apply(null, arr))
```

ES6最新用法

```js
var arr = [6, 4, 1, 8, 2, 11, 23];
console.log(Math.max(...arr))
```



