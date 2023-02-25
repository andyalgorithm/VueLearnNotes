# Vue的简介



```javascript
function Vue (options) {
  if (process.env.NODE_ENV !== production' && !(this instanceof Vue) ) {
    warn('Vue is a constructor and should be called with the `new` keyword')
  }
  this._init(options)
}
```

**总结**

- vue 本质上就是一个用 Function 实现的 Class，然后在它的原型 prototype 以及它本身上扩展了一系列的方法和属性。
- Vue 不用 ES6 的 Class 去实现的原因：按功能区分，把功能扩展分散到多个模块中去实现，然后挂载中 vue 的原型 prototype 上，也有在 Vue 这个对象本身上。
- 而不是在一个模块里实现所有，这种方式是用 Class 难以实现的。这么做的好处是非常方便代码的维护和管理。