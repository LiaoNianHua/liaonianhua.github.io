## JavaScript 字符串方法

#### 1. 获取字符串的长度

```
str.length => 字符串的长度
```

#### 2. 返回字符串中指定文本首次出现的索引位置

```
str.indexOf() => 返回字符串中指定文本首次出现的索引位置 未找到返回-1
```

#### 3. 指定文本在字符串中最后一次出现的索引

```
str.lastIndexOf() => 指定文本在字符串中最后一次出现的索引 未找到返回-1
```

#### 4. 提取部分字符串

##### (1) slice(start, end) 提取字符串的某个部分并在新字符串中返回被提取的部分

```
str.slice(start, end)

=> 返回值 返回一个新的字符串，包含从 start 到 end(不包括该元素)

=> start必须, 规定从何处开始选取。如果是负数，那么它规定从字符尾部开始算起的位置 
   也就是说，-1 指最后一个元素，-2 指倒数第二个元素，以此类推
   
=> end可选, 规定从何处结束选取, 如果没有指定该参数，那么切分的数组包含从 start    
   到数组结束的所有元素
```


##### (2) substring(start, end) 方法用于提取字符串中介于两个指定下标之间的字符

```
str.substring(start, end) 

=> 返回一个新的字符串，包含从 start 到 end(不包括该元素) 跟slice(start, end)类似

=> start必须, 一个非负的整数, 规定从何处开始选取。

=> end可选, 一个非负的整数, 规定从何处结束选取,  
   如果省略该参数，那么返回的子串会一直到字符串的结尾
```

##### (3) substr(start, length) 方法可在字符串中抽取从 start 下标开始的指定数目的字符

```
str.substr(start, length) 

=> 一个新的字符串

=> start必须,  规定从何处开始选取。如果是负数，那么它规定从字符尾部开始算起的位置 
   也就是说，-1 指最后一个元素，-2 指倒数第二个元素，以此类推
   
=> length可选, 如果省略该参数，那么返回的子串会一直到字符串的结尾
```

#### 5. 替换字符串内容

##### (1) str.replace() 用另一个值替换在字符串中指定的值， 默认只替换首个匹配

```
var str = 'Please visit Microsoft and Microsoft'
var str1 = str.replace('Microsoft', 'W3C')

=> str1的值Please visit W3C and Microsoft 只替换第一个Microsoft
```

##### (2) str.replace() 对大小写敏感

```
var str = 'Please visit Microsoft and Microsoft'
var str2 = str.replace('MiCrosoft', 'W3C')

=> str2的值不会改变 还是Please visit Microsoft and Microsoft, 
   因为replace()对大小写敏感, 找不到MiCrosoft字符串
```

##### (3) str.replace() 执行大小写不敏感的替换 请使用正则表达式 /i（大小写不敏感)

```
var str = 'Please visit Microsoft and Microsoft'
var str3 = str.replace(/MiCrosoft/i, 'W3C')

=> str3的值Please visit W3School and Microsoft, 使用了正则表达式对大小写不敏感, 
   只替换第一个Microsoft
```

##### (3) str.replace() 替换所以匹配到的元素 使用正则表达式的 /g 标志（用于全局搜索）

```
var str = 'Please visit Microsoft and Microsoft'
var str3 = str.replace(/Microsoft/g, 'W3C')

=> str3的值Please visit W3C and W3C, 使用了正则表达式对所有的Microsoft进行替换
```


#### 6. 大小写的转换

```
1. str.toUpperCase() => 把字符串转换为大写
2. str.toLowerCase() => 把字符串转换为小写
```


#### 7. concat() 方法 连接两个或多个字符串

```
var str = 'hello'
var str2 = 'world'
var str3 = str.concat(str2)
var str4 = str.concat('', str2) => str + ' ' + str2

=> str3的值是helloworld。 为了书写好看, 建议str4代码值为hello world
```

#### 8. str.trim() 删除字符串两端的空白符

```
var str = '   hello world  '
str.trim() => 值为hello world, 但IE8及IE8以下不兼容
```

#### 9. charAt(index) 提取字符串字符

```
返回字符串中指定下标（位置）的字符串

var str = 'hello world'
str.charAt(0) => H
```

#### 10. str.split() 把字符串转换为数组

```
var str = 'hello world'
str.split('') => 以空格为分隔符 分割成数组
```


