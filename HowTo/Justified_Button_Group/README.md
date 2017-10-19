### Demo
![](../../images/justified_button_group.gif)

[w3schools链接](https://www.w3schools.com/howto/howto_css_button_group.asp)

### Bullet Points
* `width` 使用百分比值, 父元素的宽度的百分比, 实现宽度动态变化
* `button` 使用浮动布局, 使用 `:after` 清除浮动. 
* `:not` `:last-child` 伪类使用. 

### Code
```html
<!Doctype html>
<html>
<style>
.btn-group button {
    background-color: #4CAF50; /* Green background */
    border: 1px solid green; /* Green border */
    color: white; /* White text */
    padding: 10px 24px; /* Some padding */
    cursor: pointer; /* Pointer/hand icon */
    float: left; /* 浮动 */
}

/* 清除浮动 (clearfix hack) */
.btn-group:after {
    content: "";
    clear: both;
    display: table;
}

.btn-group button:not(:last-child) {
    border-right: none; /* Prevent double borders */
}

/* Add a background color on hover */
.btn-group button:hover {
    background-color: #3e8e41;
}
</style>
<body>

<h1>Justified Button Group</h1>

<p>Two buttons in a group:</p>
<div class="btn-group" style="width:100%">
  <button style="width:50%">Apple</button>
  <button style="width:50%">Sony</button>
</div>

<p>Three buttons in a group:</p>
<div class="btn-group" style="width:100%">
  <button style="width:33.3%">Apple</button>
  <button style="width:33.3%">Samsung</button>
  <button style="width:33.3%">Sony</button>
</div>

<p>Four buttons in a group:</p>
<div class="btn-group" style="width:100%">
  <button style="width:25%">Apple</button>
  <button style="width:25%">Samsung</button>
  <button style="width:25%">Sony</button>
  <button style="width:25%">HTC</button>
</div>

</body>
</html>

```