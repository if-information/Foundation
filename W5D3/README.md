## 知识点

> * jQuery 基础

## jQuery 基础知识点清单
问题| 解决方案| 代码清单|
---- |----| ----|
如何把jQuery添加到HTML页面| 使用 `link` 元素导入保存在网站Web服务器或有个CDN上的jQuery库文件. 再添加一个 `script` 元素存放我们编写的jQuery代码| 1|
如何动态决定是导入jQuery 1.x还是2.x版本| 使用条件注释| 2|
如何获取页面元素| 传递一个CSS选择器给$(或jQuery)函数| 3, 4, 10|
如何重命名$函数| 使用 `noConflict` 方法| 5, 6|
如何等到DOM就绪之后才执行我们的jQuery脚本| 在全局的 `document` 变量上注册 `ready` 事件处理函数或者传递给$函数一个函数并把我们的脚本包含在这个函数中| 7, 8|
如何控制 `ready` 事件的触发时机| 使用 `holdReady` 事件| 9|
如何控制页面元素的选取范围| 为$函数提供上下文参数| 11, 12|
如何得到创建jQuery对象时使用的上下文| 读取 `context` 属性| 13|
如何使用 `HTMLElement` 对象生成jQuery对象| 把 `HTMLElement` 对象用作$函数的参数| 14|
如何遍历jQuery对象包含的元素| 把jQuery对象当成数组处理或者使用 `each` 方法| 15, 16|
如何得到jQuery对象中指定顺序号的元素| 使用 `index` 或 `get` 方法| 17 ~ 19|
如何同时对jQuery对象中包含的多个元素执行同一个操作| 在这个jQuery对象上直接调用jQuery方法| 20|
如何对一个jQuery结果集执行多个操作| 链式调用这些方法| 21 ~ 23|
如何处理事件| 使用jQuery事件处理函数| 24|

## jQuery基础知识代码清单
详见 Chapter 05 目录中代码清单


## jQuery选择元素知识点清单
问题| 解决方案| 代码清单|
---- |----| ----|
如何选取更多元素| 使用 `add` 方法| 1|
如何从结果集中得到某一个元素| 使用 `first` `last` 或 `eq` 方法| 2|
如何从结果集中截取一个子集| 使用 `slice` 方法| 3|
如何过滤结果集从而得到一个子集| 使用 `filter` 或 `not` 方法| 4, 5|
如何根据选中元素是否拥有后代元素过滤结果集| 使用 `has` 方法| 6|
如何在一个结果集中再进行一次选择| 使用 `map` 方法| 7|
如何判断结果集中至少有一个元素符合指定条件| 使用 `is` 方法| 8|
如何得到上次选择的结果| 使用 `end` 方法| 9|
如何得到上次结果集与本次结果集的合集| 使用 `addBack` 方法| 10|
如何得到选中元素的子元素或者后代元素| 使用 `children` 方法和 `find` 方法| 11 ~ 13|
如何得到选中元素的父元素| 使用 `parent` 方法| 14|
如何得到选中元素的一系列祖先元素| 使用 `parents` 方法| 15|
如何得到某一个祖先元素| 使用 `parentsUntil` 方法| 16, 17|
如何得到离自己最近的匹配选择器参数或者具体元素的祖先元素| 使用 `closest` 方法| 18, 19|
如何得到离自己最近的定位祖先元素| 使用 `offsetParent` 方法| 20|
如何得到选中元素的兄弟元素| 使用 `sublings` 方法| 21, 22|
如何得到选中元素之前或之后的兄弟元素| 使用 `next` `prev` `nextAll` `prevAll` `nextUntil` 或 `prevUntil` 方法| 23|

## jQuery选择元素代码清单
详见 Chapter 06 目录中代码清单

