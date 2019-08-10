##  1.	HTML表单标签
form
​    actiom:向后台服务器提交的地址URL（访问服务器）
​    method:向后台的提交方式
 ###    1.	应用场景
 注册，登录等
 ###    2.	表单标签：form
 ```
 属性：
 1.action:提交后台地址
 2.method:提交方式
 3.js时间编程：onsubmit事件：表示提交是否成功，提交成功返回true,否则返回false
 常用：get,post
 ```
 **get提交方式（浏览器默认）：**
 1.将用户信息提交到地址栏上
 2.提交的数据大小有限（不超过4kb）
 3.不适合提交敏感数据：如密码（提交密码是需要加密）
 **post提交方式：**
 1.数据不会提交到地址栏上
 2.提交的数据大小无限制
 3.适合提交敏感数据（密码需要特定加密）
###    3.	表单标签分类：
####    表单项：  
#####   input标签：
文本输入框,密码框,日期框,文件上传,隐藏域,按钮（普通按钮，提交按钮）,单选按钮,复选框
```
input标签：
type = "test"：文本输入框
type = "password"：密码输入框
type = "radio"：单选按钮
type = "checkbox"：复选框
type = "date"：H5提供的日期组件
type = "tel"：电话，H5提供的日期组件（内容只能为数字）
type = "file"：上传文件
type = "button"：普通按钮，必须指定value属性
type = "submit"：提交
type = "reset"：重置按钮
type = "hidden"：隐藏域（可以用于参数传递）
```
#####   select标签：
```
option:下拉菜单（应用于省市联动）
```
例：
```<select>
    <option value="选择">请选择</option>
    <option value="陕西省">陕西省</option>
    <option value="广东省">广东省</option>
    <option value="山西省">山西省</option>
</select>
下拉菜单
```
#####   textarea标签：文本域（可用于写文本）

## 2.	框架标签
frame
1.一个frame中包含一个html页面
2.如果框架结构有2个或2个以上的页面组成，称为frameset:框架集
3.farmset不能和body共存
4.farm属性：src——链接包含的html
5.farmset属性：
*   rows=“num1,num2,num3”:(从上往下看)横向划分，每一个部分(frame)占整体的部分（百分比）
*   cols“num1,num2,num3”:(从左往右看)每一个部分(frame)占整体的部分（百分比）