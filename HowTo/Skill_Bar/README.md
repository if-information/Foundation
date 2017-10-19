### Demo
![](../../images/skill_bar.png)

[w3schools链接](https://www.w3schools.com/howto/howto_css_skill_bar.asp)

### Bullet Points
* `box-sizing` 更改盒模型高度和宽度计算方式


### Reference
* [CSS box-sizing](https://developer.mozilla.org/zh-CN/docs/Web/CSS/box-sizing)

### Code
```html
<!DOCTYPE html>
<html>
<head>
<style>
* {box-sizing: border-box}

.container {
  width: 100%;
  background-color: #ddd;
}

.skills {
  text-align: right;
  padding-right: 20px;
  line-height: 40px;
  color: white;
}

.html {width: 90%; background-color: #4CAF50;}
.css {width: 80%; background-color: #2196F3;}
.js {width: 65%; background-color: #f44336;}
.php {width: 60%; background-color: #808080;}
</style>
</head>
<body>

<h1>My Skills</h1>

<p>HTML</p>
<div class="container">
  <div class="skills html">90%</div>
</div>

<p>CSS</p>
<div class="container">
  <div class="skills css">80%</div>
</div>

<p>JavaScript</p>
<div class="container">
  <div class="skills js">65%</div>
</div>

<p>PHP</p>
<div class="container">
  <div class="skills php">60%</div>
</div>

</body>
</html>
```