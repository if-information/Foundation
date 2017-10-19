### Demo
![](../../images/button-group.gif)

[w3schools链接](https://www.w3schools.com/howto/howto_css_button_group.asp)

### Bullet Points
* `cursor` 特性使用.
* `button` 使用float布局, 使用 `:after` 清除布局.
* `:not` 伪类使用.
* `:last-child` 伪类使用.

### Reference
* [CSS cursor](https://developer.mozilla.org/zh-CN/docs/Web/CSS/cursor)
* [CSS :not](https://developer.mozilla.org/zh-CN/docs/Web/CSS/:not)
* [CSS :last-child](https://developer.mozilla.org/zh-CN/docs/Web/CSS/:last-child)

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
    float: left; /* Float the buttons side by side */
}

/* 清除浮动 (clearfix hack) */
.btn-group:after {
    content: "";
    clear: both;
    display: table;
}

.btn-group button:not(:last-child) {
    border-right: none; /* 避免双边框 */
}

/* Add a background color on hover */
.btn-group button:hover {
    background-color: #3e8e41;
}
</style>
<body>

<h1>Button Group</h1>

<div class="btn-group">
  <button>Apple</button>
  <button>Samsung</button>
  <button>Sony</button>
</div>

</body>
</html>

```