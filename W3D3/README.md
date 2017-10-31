## 知识点

> * 鼠标的`keyup` 事件
> * `input` 元素中的值如何过去 (`value`属性)
> * JS字符串常用方法 `upUpperCase()`
> * JS字符串常用方法 `index()`
> * JS字符串常用方法 `split()`




## 演示Demo1
![](../images/filter_list.gif)

[代码清单](../HowTo/Filter_List/)



## 演示Demo2
![](../images/filter_element.gif)

尝试将JavaScript部分写出来
```html
<!DOCTYPE html>
<html>
<style>
    .filterDiv {
        float: left;
        background-color: #2196F3;
        color: #ffffff;
        width: 100px;
        line-height: 100px;
        text-align: center;
        margin: 2px;
        display: none;
    }

    .show {
        display: block;
    }

    .container {
        margin-top: 20px;
        overflow: hidden;
    }
</style>
<body>

<h2>Filter DIV Elements</h2>

<input type="radio" onclick="filterSelection('all')" name="category" checked> Show all<br>
<input type="radio" onclick="filterSelection('cars')" name="category"> Cars<br>
<input type="radio" onclick="filterSelection('animals')" name="category"> Animals<br>
<input type="radio" onclick="filterSelection('fruits')" name="category"> Fruits<br>
<input type="radio" onclick="filterSelection('colors')" name="category"> Colors<br>

<div class="container">
    <div class="filterDiv cars">BMW</div>
    <div class="filterDiv colors fruits">Orange</div>
    <div class="filterDiv cars">Volvo</div>
    <div class="filterDiv colors">Red</div>
    <div class="filterDiv cars animals">Mustang</div>
    <div class="filterDiv colors">Blue</div>
    <div class="filterDiv animals">Cat</div>
    <div class="filterDiv animals">Dog</div>
    <div class="filterDiv fruits">Melon</div>
    <div class="filterDiv fruits animals">Kiwi</div>
    <div class="filterDiv fruits">Banana</div>
    <div class="filterDiv fruits">Lemon</div>
    <div class="filterDiv animals">Cow</div>
</div>

<script>
    // 尝试写出JavaScript逻辑代码
    
    
</script>

</body>
</html>

```
