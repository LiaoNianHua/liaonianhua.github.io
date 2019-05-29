## JavaScript含义

```
JavaScript 是属于 HTML 和 Web 的编程语言在 HTML 中， 
JavaScript 代码必须位于 <script> 与 </script> 标签之间。

旧的 JavaScript 例子也许会使用 type 属性：<script type="text/javascript">
type属性不是必需的。JavaScript 是 HTML 中的默认脚本语言
```

#### 1. JavaScript的引入

##### (1) JavaScript 函数被放置于 HTML 页面的 <head> 或 <body> 部分

```
把脚本置于 <body> 元素的底部，可改善显示速度，因为脚本编译会拖慢显示

<body>
  <script>
    function fn () {
      document.getElementById("demo").innerHTML = "内容已经被更改"
    }
  </script>
</body>
```

##### (2) 外部脚本

```
<script src="myScript.js"></script>

优势 ① 分离了HTML和代码
     ② 使HTML和JavaScript更易于阅读和维护
     ③ 已缓存的JavaScript文件可加速页面加载
```


#### 2. JavaScript 关键词

```
var => 定义变量, 所有的变量必须以唯一的名称来标识 这些唯一的名称称为标识符
```


#### 3. JavaScript 注释

```
双斜杠 // 或 /* 与 */ 之间的代码被视为注释。
```


#### 4. JavaScript 对大小写敏感

```
变量 lastName 和 lastname，是两个不同的变量 

var lastName = "ABC"
var lastname = "ABC"
```


#### 5. 一条语句，多个变量

```
var a = 1, b = 2, c = 3; => 用逗号隔开
```


#### 6. 重复声明 JavaScript 变量


```
如果再次声明某个JavaScript变量 它的值不会丢

var a = 1
var a 

a => 1
```

#### 7. 函数的调用

```
1. 普遍方法 调用fn()

function fn () {
  var str = "你好"
  return str
}

2. 把整个function(){}赋值给fn, fn()调用得到值

var fn = function () {
  var str = "你好"
  return str
} 


3. 直接调用function(){}, 再把得到的值赋值给fn
var fn = function () {
  var str = "你好"
  return str
}()

```

#### 8. 转义字符 \ 

```
\' => '
\" => "
\\ => \
```

