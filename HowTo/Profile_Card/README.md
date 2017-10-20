![](profilecard.gif)

![](profile_require.png)

代码清单
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
    <style>
        .card {
            box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
            max-width: 300px;
            margin: auto;
            text-align: center;
 
            font-family: arial;
        }
 
        .container {
            padding: 0 16px;
        }
 
        .container::after {
            content: "";
            clear: both;
            display: table;
        }
 
        .title {
            color: grey;
            font-size: 18px;
        }
 
        button {
            border: none;
            outline: 0;
            display: inline-block;
            padding: 8px;
            color: white;
            background-color: #000;
            text-align: center;
            cursor: pointer;
            width: 100%;
            font-size: 18px;
        }
 
        a {
            text-decoration: none;
            font-size: 22px;
            color: black;
        }
 
        button:hover, a:hover {
            opacity: 0.7;
        }
    </style>
</head>
<body>
 
<h2 style="text-align:center">User Profile Card</h2>
 
<div class="card">
    <img src="images/team2.jpg" alt="John" style="width:100%">
    <div class="container">
        <h1>John Doe</h1>
        <p class="title">CEO & Founder, Example</p>
        <p>Harvard University</p>
        <div style="margin: 24px 0;">
            <a href="#"><i class="fa fa-dribbble"></i></a>
            <a href="#"><i class="fa fa-twitter"></i></a>
            <a href="#"><i class="fa fa-linkedin"></i></a>
            <a href="#"><i class="fa fa-facebook"></i></a>
        </div>
 
        <!-- button 即便设置为display: block, width值设置为auto依然还是保持内联元素的特性, 内容有多宽就多宽, 不会自动扩展. -->
        <p><button>Contact</button></p>
    </div>
</div>
 
</body>
</html>

```