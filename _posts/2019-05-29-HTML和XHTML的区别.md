#### XHTML是以XML格式编写的HTML

XHTML与 HTML相比最重要的区别

```
1. 文档结构
  (1) XHTML的DOCTYPE是强制性的
  (2) <html>中的 XML namespace 属性是强制性的
  (3) <html><head><title><body>都是强制性的

2. 元素语法
  (1) 元素必须始终关闭
  (2) 标签必须小写
  (3) 必须有一个根元素
  (4) 必须被正确的嵌套
  
3. 属性语法
  (1) 属性必须小写
  (2) 属性值必须用引号包围
  (3) 属性最小化也是禁止的
```


```
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">

<html xmlns="http://www.w3.org/1999/xhtml">
  <head>
    <title>Title of document</title>
  </head>
  <body>
    ......
  </body>
</html>
```


#### 如何从 HTML 转换到 XHTML

```
1. 向每张HTML页面的第一行添加XHTML <!DOCTYPE>
2. 向每张页面的 html 元素添加 xmlns 属性
3. 关闭所有空元素
4. 所有的元素以及属性都小写
5. 为所有属性值加引号

```
