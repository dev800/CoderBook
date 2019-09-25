# JavaScript面试常见基本知识点

> 前端工程师最基础的部分，需要掌握

## 变量和类型

1. `JavaScript`规定了几种语言类型

   ```javascript
   // Undefined
   // Null
   // Boolean
   // String
   // Number
   // Symbol (ES6新加的)
   // Object
   // BigInt (ES10增加，目前已被最新的Chrome支持)
   ```

1. `JavaScript`对象的底层数据结构是什么

1. `Symbol`类型在实际开发中的应用、可手动实现一个简单的`Symbol`

1. `JavaScript`中的变量在内存中的具体存储形式

1. 基本类型对应的内置对象，以及他们之间的装箱拆箱操作

1. 理解值类型和引用类型

1. `null`和`undefined`的区别

   ```javascript
   /*
   	// undefined
   	- undefined类型表示未定义，它的值只有一个：undefined
   	- 任何变量赋值前都是undefined类型，值为undefined（而不是null）
   	- undefined是一个变量，而非一个关键字
   	- 需要表达这个值，可以用全局变量undefined，或者void运算
   	
   	// null
   	- 只有一个值，就是null
   	- 表示空值，是关键字，可以放心使用null关键字来获取null值
   */
   
   parseInt(undefined) // NaN
   parseInt(null) // NaN
   ```

1. 至少可以说出三种判断`JavaScript`数据类型的方式，以及他们的优缺点，如何准确的判断数组类型

1. 可能发生隐式类型转换的场景以及转换原则，应如何避免或巧妙应用

1. 出现小数精度丢失的原因，`JavaScript`可以存储的最大数字、最大安全数字，`JavaScript`处理大数字的方法、避免精度丢失的方法

## 原型和原型链

1. 理解原型设计模式以及`JavaScript`中的原型规则
1. `instanceof`的底层实现原理，手动实现一个`instanceof`
1. 实现继承的几种方式以及他们的优缺点
1. 至少说出一种开源项目(如`Node`)中应用原型继承的案例
1. 可以描述`new`一个对象的详细过程，手动实现一个`new`操作符
1. 理解`es6 class`构造以及继承的底层实现原理

## 作用域和闭包

1. 理解词法作用域和动态作用域
1. 理解`JavaScript`的作用域和作用域链
1. 理解`JavaScript`的执行上下文栈，可以应用堆栈信息快速定位问题
1. `this`的原理以及几种不同使用场景的取值
1. 闭包的实现原理和作用，可以列举几个开发中闭包的实际应用
1. 理解堆栈溢出和内存泄漏的原理，如何防止
1. 如何处理循环的异步操作
1. 理解模块化解决的实际问题，可列举几个模块化方案并理解其中原理

## 执行机制

1. 为何`try`里面放`return`，`finally`还会执行，理解其内部机制
1. `JavaScript`如何实现异步编程，可以详细描述`EventLoop`机制
1. 宏任务和微任务分别有哪些
1. 可以快速分析一个复杂的异步嵌套逻辑，并掌握分析方法
1. 使用`Promise`实现串行
1. `Node`与浏览器`EventLoop`的差异
1. 如何在保证页面运行流畅的情况下处理海量数据

## 语法和API

1. 理解`ECMAScript`和`JavaScript`的关系
1. 熟练运用`es5`、`es6`提供的语法规范，
1. 熟练掌握`JavaScript`提供的全局对象（例如`Date`、`Math`）、全局函数（例如`decodeURI`、`isNaN`）、全局属性（例如`Infinity`、`undefined`）
1. 熟练应用`map`、`reduce`、`filter` 等高阶函数解决问题
1. `setInterval`需要注意的点，使用`settimeout`实现`setInterval`
1. `JavaScript`提供的正则表达式`API`、可以使用正则表达式（邮箱校验、`URL`解析、去重等）解决常见问题
1. `JavaScript`异常处理的方式，统一的异常处理方案
