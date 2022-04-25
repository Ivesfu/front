## strict 模式

`Javascript`语言设计之初，没有限制声明变量前必须加`var`，这点给编程增加了一定的隐患。

如果一个变量没有通过`var`声明就被使用，那么该变量就自动被声明为全局变量。

在**同一个页面的不同的JavaScript文件**中，如果都不用`var`申明，恰好都使用了变量`i`，将造成变量`i`互相影响，产生难以调试的错误结果。

使用`var`申明的变量则不是全局变量，它的范围被限制在该变量被申明的函数体内（函数的概念将稍后讲解），同名变量在不同的函数体内互不冲突。

为了避免这种隐患，在后续更新的`Javascript`标准中增加了`strict`模式。在strict模式下运行的JavaScript代码，强制通过`var`申明变量，未使用`var`申明变量就使用的，将导致运行错误

在`strict`模式下，声明变量时变量前必须加`var`。

具体`eg code`：

~~~javascript
'use strict';
var a = 4;//行*
a = a + 3;
console.log(a);//such like that debug in console
~~~

`Ps`：如果浏览器支持`strict`模式，在行*处去掉`var`会报`ReferenceError`错误。