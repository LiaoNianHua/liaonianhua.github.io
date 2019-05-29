## Javascript数字方法

#### 1. 数字和字符串相加

```
JavaScript 的加法和级联（concatenation）都使用 + 运算符。 数字用加法。字符串用级联

数字和字符串相加 = 字符串

var x = '10'
var y = 10
var z = x + y

=> z的值为1010, 数据类型为string
```


#### 2. 数字和字符串数字运算

```
所有数字运算中，JavaScript 会尝试将字符串转换为数字

数字和字符串相减/乘/除 = 数字

var x = '10'
var y = 10
var z1 = x - y
var z2 = x * y
var z3 = x / y

=> z1、z2、z3的值为0、100、1, 数据类型为number
```

#### 3. NaN - 非数值

##### (1) 尝试用一个非数字字符串进行除法会得到 NaN

```
NaN 属于 JavaScript 保留词，指示某个数不是合法数

var x = 100
var y = 'apple'
var z = x / y

=> z的值就是NaN即 Not a Number
```

##### (2) 在数学运算中使用了 NaN，则结果也将是 NaN

```
var x = NaN
var y = 1
var z = x + y

=> z的值 NaN
```

##### (3) NaN与字符串相接

```
var x = NaN
var y = '1'
var z = x + y

=> z的值 NaN1
```

##### (4) isNaN() 来确定某个值是否是数

```
var x = 100
var y = 'apple'
var z = x / y
isNaN(z) => true
```

##### (5) NaN 是数，typeof NaN 返回 number

```
typeof NaN; => number
```


#### 4. 数值可以是对象

```
通常 JavaScript 数值是通过字面量创建的原始值：var x = 123
但是也可以通过关键词 new 定义为对象：var y = new Number(123)
var z = new Number(123)

1. x == y => true, 仅仅判断数值是否是相等
2. x === y => false, x的类型是number, y的数据类型是object 
3. y == z => false, y、z的数据类型是object, 对象无法进行对比
```

#### 5. 数值方法

##### 1. num.toString()

```
num.toString()以字符串返回数值 数据类型string

var num = 123
num.toString() => 123 数据类型string
```

##### 2. num.toFixed() 方法

```
num.toFixed() 返回字符串值，保留几个小数

var num = 1.234
num.toFixed(2) => 1.23 数据类型string
```

#### 3. valueOf() 以数值返回数值

```
在 JavaScript 内部使用 valueOf() 方法可将 Number 对象转换为原始值
```


#### 6. 全局 JavaScript 方法 把变量转换为数值

##### (1) 强制转换为数值型

```
1. Number('1.23') => 1.23 数据类型number
2. Number(true) => 1 数据类型number
3. Number(false) => 0 数据类型number
4. Number('abc') => NaN 即 Not a Number, 数据类型number
```

##### (2) 解析其参数并返回整数

```
1. parseInt('1.23') => 1 => number型
2. parseInt(false) => NaN 即 Not a Number, 数据类型number
3. parseInt('abc') => NaN 即 Not a Number, 数据类型number
```

##### (3) 解析其参数并返回浮点数

```
1. parseFloat('1.23') => 1.23 => number型
2. parseFloat(false) => NaN 即 Not a Number, 数据类型number
3. parseFloat('abc') => NaN 即 Not a Number, 数据类型number
```

