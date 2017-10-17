### Demo
![](../../images/notes.png)

[w3schools链接](https://www.w3schools.com/howto/howto_css_notes.asp)


### Bullet Points
* `border` 属性的使用


### Code
```html
<!DOCTYPE html>
<html>
<head>
<style>

/* 元素选择器, 选择所有的 div 元素 */
div {
    margin-bottom: 15px;
    padding: 4px 12px;
}

/* 类选择器, 选择属于 danger 类的所有元素*/
.danger {
    background-color: #ffdddd;
    border-left: 6px solid #f44336;
}


.success {
    background-color: #ddffdd;
    border-left: 6px solid #4CAF50;
}

.info {
    background-color: #e7f3fe;
    border-left: 6px solid #2196F3;
}


.warning {
    background-color: #ffffcc;
    border-left: 6px solid #ffeb3b;
}
</style>
</head>
<body>

<h2>Notes</h2>
<div class="danger">
  <p><strong>Danger!</strong> Some text...</p>
</div>

<div class="success">
  <p><strong>Success!</strong> Some text...</p>
</div>

<div class="info">
  <p><strong>Info!</strong> Some text...</p>
</div>

<div class="warning">
  <p><strong>Warning!</strong> Some text...</p>
</div>

</body>
</html>

```
