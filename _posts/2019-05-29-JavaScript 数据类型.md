#### JavaScript 数据类型

```
JavaScript 数据类型有字符串值，数值，布尔值，数组，对象

typeof 来确定 JavaScript 变量的类型, 返回变量或者表达式的类型; 
typeof 运算符把对象、数组或 null 返回 object
```



#### 1. 字符串值

```
var a = 'abc'; => typeof a是string
```

#### 2. 数值

```
var a = 123 => typeof a是number
```

#### 3. 布尔值

```
布尔值只有两个 true / false

var a = true => typeof a 是boolean
```

#### 4. 空值

```
空值与 undefined 不是一回事, 空的字符串变量既有值也有类型, typeof 返回 string。

var a = '';  => 值是 ""，类型是 string
```

#### 5. Undefined 

```
在 JavaScript 中，没有值的变量，其值是 undefined。typeof 也返回 undefined。

var a;
typeof a => 值是 undefined，类型是 undefined
```


#### 6. Null

```
null 的数据类型是对象, 通过设置值为 null 清空对象, typeof 返回 object。

var obj = null;  => 值是null, 类型是 object
```

#### 7. undefined 与 Null 的区别

```
1. undefined类型只有一个值 即undefined; 当声明的变量还未被初始化时，变量的默认值为undefined

2. Null类型也只有一个值 即null; null用来表示尚未存在的对象，常用来表示函数企图返回一个不存在的对象

3. undefined 与 null 的值相等，但类型不相等

undefined == null => true
null === undefined => false
typeof undefined => undefined
typeof null => object
```

#### 8. 数组 / 对象

```
var obj = {} => typeof obj的值是object
var arr = [] => typeof arr的值是object
```

#### 9. 函数

```
typeof (function a () {}) => 值为function
```


