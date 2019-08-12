##  Js中自定义对象四种方式
####    1 类似JAVA有参构造方式：
1.定义对象：
```
function 对象（属性[age]）{
    追加属性；
    如（this.age = age）[this代表当前对象的地址值的引用]
    追加方法；
    如（this.hello = function(){
        alter("Hello!");
    }）
    
}
```
2.创建对象：
```
var 对象名 = new 对象（属性实际值）
```
####    2  类似JAVA无参构造方式：
1.定义对象：
```
function Person(){
    
}
```
2.创建对象：
```
var per = new Person();
```
3.追加属性：
```
per.name = "张三"；
per.age = 22;
```
4.追加方法：
```
per.hello = function(){
    alter("Hello!");
}
```
####    3  利用js中的模板对象：Object
1.创建对象：
```
var per = new Object();
```
2.追加属性：
```
per.name = "张三"；
per.age = 22;
```
3.追加方法：
```
per.hello = function(){
    alter("Hello!");
}
```
####    4  字面量值的方式（json）
格式：
```
{
    "key1":value1，      //value可以是任何类型
    "key2":value 

}
```
例：
```
var per = {
    "name":"张三"，
    “age":20,
    "hello" :function(){
        alter("Hello!");
    }
};
```





## 原型对象：Prototype

如果在内置对象创建了一个原型对象，那么原型对象中追加的方法会自动追击到内置对象中