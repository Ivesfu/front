css语法

`CSS`的基本语法：选择器 + 声明块
选择器：通过选择器可以选中页面中的指定元素，比如p的作用就是选中页面中所有的p元素
声明块：通过声明块来指定要为元素设置的样式，声明块由一个一个的声明组成，声明是一个名值对结构
一个样式名 对应一个样式值， 名和值之间以 : 连接，以 ; 结尾

+ 元素选择器
  作用：根据标签名来选中指定的元素
  语法：标签名`{}`
  例子：`p{} h1{} div{}`

+ `id`选择器
  作用：根据元素的id属性值选中一个元素
  语法:` #id属性值{}`
  例子: `#box{} #red{}`

+ `class`选择器，`class`是一个标签的属性，它和`id`类似，不同的是`class`可以重复使用，可以给一个标签指定多个类

+ 通配选择器，`*`，选择所有元素，优先级比较低。

  ~~~css
  /* 元素选择器 */
  h1{
      color: brown;
      font-size: x-large;
  }
  /* id选择器 */
  #red{
      color: red;
      font-size: medium;
  }
  #yellow{
      color: yellow;
      font-size: medium;
  }
  #blue{
      color:blue;
      font-size: medium;
  }
  #purple{
      color:purple;
      font-size: medium;
  }
  /* class选择器 */
  .black{
      color:black;
      font-size: medium;
  }
  /* 通配选择器 */
  *{
      font-size: larger;
      color:
  }
  ~~~

+ 样式的继承，我们为一个元素设置的样式同时也会应用到它的后代元素上，继承是发生在祖先后后代之间的，继承的设计是为了方便我们的开发，利用继承我们可以将一些通 用的样式统一设置到共同的祖先元素上，这样只需设置一次即可让所有的元素都具有该样式
  注意：并不是所有的样式都会被继承，比如背景相关的，布局相关等的这些样式都不会被继承。

