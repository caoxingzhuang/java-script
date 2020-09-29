#### **###js是世界上最流行的语言之一，是一种运行在客户端的脚本语言**

***

![](F:\caoxingzhuang\js基础\images\Snipaste_2020-08-18_09-42-44.png)

***

![](F:\caoxingzhuang\js基础\images\Snipaste_2020-08-18_10-16-44.png)

***

ECMA:规定了js的编程语法和基础核心知识，是所有浏览器共同遵守的一套js语法工业标准

***

#### js输出语句：

alert（弹出框）  console.log(打印框)    prompt（输入框）

#### 变量：

存放数据的容器，本质：空间，变量名。用来存储数据

###### 使用步骤：

1.声明变量  2.赋值   var age;

***

##### 命名规则

![](F:\caoxingzhuang\js基础\images\Snipaste_2020-08-18_11-49-36.png)

------



## 数据类型：

在计算机中，不同数据占用存储空间不同，于是定义了不同的数据类型，

## 变量的数据类型：

js是动态语言，变量的数据类型是可以变化的。

js的变量类型是只有程序运行过程中，根据等号右边的值来确定的。

## 简单数据类型：

1. 八进制 0-7   数字前面加0
2. 十六进制 0-9  数字前面加0x
3. NaN 非数字
4. isNaN  判断用户是否输入的数字  是返回false 不是返回true

![](F:\caoxingzhuang\js基础\images\Snipaste_2020-08-18_14-35-01.png)

***

### 字符串型 String 

- var num = "字符串单引号或者双引号"

1.   转义
2. ![](F:\caoxingzhuang\js基础\images\Snipaste_2020-08-18_15-19-27.png)

***

### 字符串拼接

1. var num = "字符串"+数字;  拼接效果，结果是字符串效果。数字和数字相加得到的是和。

2. var num = "字符串"'+变量名+'字符串'

   ***

   

### 布尔型（做判断）

1. true（参与加法运算当1来看）      false   （参与加法当0看）
2. 如果变量未给值   就是undefined   未定义数据类型
3. null  空值0

![](F:\caoxingzhuang\js基础\images\Snipaste_2020-08-18_16-22-32.png)

#### 检测数据类型（typeof）返回的结果都是以字符串输出  出来的

#### 转换数据类型：String强行转换  toString()

- var num = 10;         num=String(num);

***

#### 转换数字类型:        

- Number() 
-  parseint()不会保留小数
- parseFloat()保留小数
- 隐式转换   var a ='10';     a = a-0 ;     a = a % 13 只要比自己大   余数就是本身

#### 转布尔值:

- 字符串都为  true
- 0 NaN false  undefined  null  空字符串""-为false
- 取两次返   var a ="123";    console.log(!!a);

数据的转换中，我们经常用到的是将变量转换成字符串或数字。

转换成字符串要使用toString（），例 

```
`var` `married = ``false``;` `alert(married.toString());`` ` 
```

转换成数字时，有两种方法，parseInt() 转换成整数，parseFloat()转换成浮点数。

例：

```
`var` `test = parseInt(“blue”); ``//returns NaN` `var` `test = parseInt(“1234blue”); ``//returns 1234` `var` `test = parseInt(“22.5”); ``//returns 22` `var` `test = parseFloat(“1234blue”); ``//returns 1234` `var` `test = parseFloat(“22.5”); ``//returns 22.5`
```