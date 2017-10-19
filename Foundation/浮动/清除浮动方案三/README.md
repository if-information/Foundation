## 清除浮动方案三

HTML代码:
```html
<div class="content">
    <div class="box1">Box1</div>
    <div class="box2">Box2</div>
    <div class="box3">Box3</div>

    <div class="clear-float"></div>
</div>

<div class="footer">Footer</div>
```

CSS代码:
```css
        .content {
            border: 1px solid orange;
        }

        .box1, .box2, .box3 {
            border: 1px solid red;
            width: 200px;
            height: 150px;
            float: left;
        }

        .footer {
            border: 1px solid blue;
            height: 100px;
        }
```

效果如下:
 
![](../../../images/float_around_3.png)


修改CSS代码如下: 
```css
        .content {
            border: 1px solid orange;
        }

        /* 清除浮动 */    
        .clear-float {
            clear: both;
        }

        .box1, .box2, .box3 {
            border: 1px solid red;
            width: 200px;
            height: 150px;
            float: left;
        }

        .footer {
            border: 1px solid blue;
            height: 100px;
        }
```