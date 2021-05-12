# this

函数调用时，除了传入函数的显示参数外，还传入了 arguments / this 两个参数。JS 函数中的 this 依赖于函数的调用方式。

- 作为方法调用，this 表示当前实例
- 作为函数调用，this 表示全局对象 (浏览器中的 window ) ，这点可以理解为全局函数是 window 的一个方法
- 作为构造器进行调用，this 表示新建的实例
- 通过 apply() / call() 方法进行调用，this 表示传入的参数

## bind this

## 柯里化 currying

## 缓存记忆

这个是真的挺厉害的。

## 函数包装

## 即时函数

## 循环中的即时函数
