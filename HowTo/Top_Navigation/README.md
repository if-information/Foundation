### Demo
![](../../images/top-navigation.gif)

[w3schools链接](https://www.w3schools.com/howto/howto_js_topnav.asp)

### Bullet Points
* 导航栏中的 `a` 元素进行了浮动布局, 使用 `overflow: hidden` 清除浮动.
* `a` 元素设置为 `display: block`, 保证内边距正常显示.
* `:hover` 伪类的使用.


### Reference
* [CSS display](https://developer.mozilla.org/zh-CN/docs/Web/CSS/display)
* [CSS overflow](https://developer.mozilla.org/zh-CN/docs/Web/CSS/overflow)
* [CSS float](https://developer.mozilla.org/zh-CN/docs/CSS/float)
* [CSS 伪类](https://developer.mozilla.org/zh-CN/docs/Web/CSS/Pseudo-classes)
* [CSS :hover](https://developer.mozilla.org/zh-CN/docs/Web/CSS/:hover)


### Code
```html

<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Top Navigation</title>
<style>
body {
margin:0;
}

/* 获取属于topnav类的所有元素 */
.topnav {
  overflow: hidden; /* 清除浮动 */
  background-color: #333;
}

/* 获取属于topnav类的元素里面的所有a子元素 */
.topnav a {
  float: left;    /* 浮动 */
  display: block; /* 成为块元素盒 */
  color: #f2f2f2;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
  font-size: 17px;
}

/* 获取属于topnav类的元素里面的所有a子元素的鼠标悬停状态 */
.topnav a:hover {
  background-color: #ddd;
  color: black;
}

/* 获取属于topnav类的元素里面的所有a子元素, 同时这些a元素属于active类 */
.topnav a.active {
    background-color: #4CAF50;
    color: white;
}
</style>
</head>
<body>

<div class="topnav">
  <a class="active" href="#home">Home</a>
  <a href="#news">News</a>
  <a href="#contact">Contact</a>
  <a href="#about">About</a>
</div>

<div style="padding-left:16px">
  <h2>Top Navigation Example</h2>
  <p>Some content..</p>
</div>

</body>
</html>
```