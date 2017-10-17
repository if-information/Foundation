### Demo
![](../../images/pagination.gif)

[w3schools链接](https://www.w3schools.com/howto/howto_css_pagination.asp)

### Bullet Points
* `a` 元素使用浮动布局.
* `transition` 过渡特性使用.
* `:not` 伪类的使用.
* `&laquo;` `&raquo;` 实体字符使用. 

### Reference
* [CSS transitions](https://developer.mozilla.org/zh-CN/docs/Web/CSS/CSS_Transitions/Using_CSS_transitions)

### Code
```html
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<style>
.pagination a {
    color: black;
    float: left;
    padding: 8px 16px;
    text-decoration: none;
    transition: background-color .3s;
}

.pagination a.active {
    background-color: #4CAF50;
    color: white;
}

.pagination a:hover:not(.active) {
    background-color: #ddd;
}
</style>
</head>
<body>

<h2>Pagination</h2>
<p>Responsive pagination with hover effects:</p>

<div class="pagination">
  <a href="#">&laquo;</a>
  <a href="#">1</a>
  <a class="active" href="#">2</a>
  <a href="#">3</a>
  <a href="#">4</a>
  <a href="#">5</a>
  <a href="#">6</a>
  <a href="#">&raquo;</a>
</div>

</body>
</html>

```