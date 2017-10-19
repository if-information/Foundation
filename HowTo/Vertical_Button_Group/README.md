### Demo
![](../../images/vertical_button_group.gif)

[w3schools链接](https://www.w3schools.com/howto/howto_css_button_group_vertical.asp)

### Bullet Points
* `button` 呈现为块元素
* `:not` `:last-child` 伪类使用

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
    width: 50%; /* Set a width if needed */
    display: block; /* 呈现块元素 */
}

.btn-group button:not(:last-child) {
    border-bottom: none; /* Prevent double borders */
}

/* Add a background color on hover */
.btn-group button:hover {
    background-color: #3e8e41;
}
</style>
<body>

<h1>Vertical Button Group</h1>

<div class="btn-group">
  <button>Apple</button>
  <button>Samsung</button>
  <button>Sony</button>
</div>

</body>
</html>

```