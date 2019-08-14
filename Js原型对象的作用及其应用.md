#  Js原型对象的作用及应用
####    原型对象：Prototype
如果在内置对象创建了一个原型对象，那么原型对象中追加的方法会自动追击到内置对象中
*   作用：

1. 在js的所有内置对象中都存在prototype原型属性
2. 在js的内置对象的原型属性中，追加方法，那么该方法会自动追加到内置对象中
3. js的原型属性最终的目的是给内置对象追加方法

*   使用方式：
```
function Array(){
    //创建一个原型对象
    this.prototype(原型属性) = new Prototype();
    //自动追加
    this.seach = function(target){
        ...
    }
}
function Prototype(){
    this.seach = function(taget){
        ...
    }
}
```
*   简写方式：
```
this.内置对象.prototype{
    额外追加的方法
}
```
*   实例：
```
this.Array.prototype.search=function(target){
	for(var i = 0 ; i < this.length; i++){
			if(this[i] ==target){
				return i ;
			}
		}
		return -1 ;
}

//追加max方法
this.Array.prototype.max = function(){
	//定义参照物
	var max = this[0] ;
	for(var i =1 ;i <this.length;i++){
		if(this[i]>max){
			max =this[i] ;
		}
	}
	return max ;
}

	//定义一个数组
var arr =[10,78,15,21,65] ; //new Array{具体元素} ;
//调用方法
var index = arr.search(15) ;
document.write("当前元素第一次出现的索引是:"+index+"<br/>") ;
var max = arr.max() ;
document.write("当数组中的最大值是:"+max+"<br/>") ;
```