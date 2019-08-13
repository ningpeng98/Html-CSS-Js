#   JavaScript
##   1.	引用方式：
1.内部Js方式
​    在head标签体指定script标签
​    弊端：js代码与html代码混合使用
2.外部js方式
​    a.单独创建独立的以.js结尾的文件
​    b.导入js文件：在head标签体中，使用script（有标签体）指定src属性，加载外部js文件
## 2.	常用函数

document.write("xxxxxxxxx");——（“向浏览器输出内容”）
alert("yyyyyyyy");——（“对话提示框”）
## 3.	变量和数据类型

* js是一个弱类型语言，定义变量和对象都用var定义
* var可以定义任何数据类型的变量（变量的类型通过值来确定），var可以省略，但不建议
* 在js中，可以重复定义变量，后面定义的变量会覆盖前面定义的变量
### 3.1 数据类型

查看数据类型：typeof(变量名)
无论整数还是小数，都是number类型——>Number对象（js内置对象）
无论字符还是字符串，都是string类型——>String对象（js内置对象）
boolean类型——>Boolean内置对象
object类型——>Object;——>js中，Object代表所有对象的模板
##  4.	js类型转换函数
string——>整数：parseInt(变量名)；
string类型与number类型比较时，会默认转换为number类型
特点：在转换过程中，遇到非数值型时，停止转换
string——>小数：parseFloat(变量名)；
## 5.	js运算符

* 算术运算符：+，-，* ，/, %
* 比较运算符：==，<，<=，>，>=
* 逻辑运算符：逻辑非：！，逻辑与：&&，逻辑或：||
* 三目（三元）运算符：表达式？true结果：false结果；
* js作为弱类型语言，可以用1代表true，0代表false

##  6. js流程控制语句
1.顺序结构语句：
js代码依次由上而下加载
2.选择结构语句：
if语句：
if(表达式){

}
*   if表达式如果是number类型，非0，条件成立，否则条件不成立
*   如果是string类型，非空字符串条件成立，否则不成立
*   如果是boolean类型，true条件成立，false不成立
*   如果是object类型，非null条件成立，否则不成立
    3.循环结构语句：
    for,,while,do-while...
*   js中switch特点：
    1.switch语句结束条件
*   遇见break,条件结束
*   程序默认执行到末尾
    2.表达式可以是：string，number，boolean...
    **3.case后面的值可以是常量也可以是变量**
#####   for-in语句
格式：
```
for(var 变量名 in 数组对象/自定义对象){
    输出变量；
}
```
#####   with语句：
格式：
```
with(文档对象：如document){
   具体逻辑；    
}
```

