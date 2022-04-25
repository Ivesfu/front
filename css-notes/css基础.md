网页分成三个部分：**结构**(HTML)，**表现**(css)，**行为**(JavaScript)

css：层叠样式表，网页实际上是一个多层的结构，通过css可以分别为网页的每一个层来设置样式而最终我们能看到只是网页的最上边一层
总之一句话，css用来设置网页中元素的样式

使用css来修改元素的样式
第一种方式(**内联样式**，行内样式)：
在标签内部通过style属性来设置元素的样式问题：使用内联样式，样式只能对一个标签生效，如果希望影响到多个元素必须在每一个元素中都复制一遍并且当样式发生变化时，我们必须要一个一个的修改，非常的不方便
注意:开发时绝对不要使用内联样式

第二种方式（**内部样式表**)
将样式编写到head中的style标签里，然后通过css的选择器来选中元素并为其设置各种样式
可以同时为多个标签设置样式，并且修改时只需要修改一处即可全部应用-内部样式表更加方便对样式进行**复用**。

第三种方式 (**外部样式表**)：最佳使用方式。
可以将CSS样式编写到一个外部的css文件中，然后通过link标签来引入外部的css文件，可以在所有网页中进行复用。

将样式编写到外部的css文件中，可以使用到**浏览器的缓存机制**，从而加快网页的加数速度，据高用户的体验。

~~~html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="./style.css">
    <!-- 通过link标签进行引用外部样式表 -->
</head>
<body>
    <p>fsdfas </p>
</body>
</html>
~~~

