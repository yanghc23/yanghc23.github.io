## 1 逻辑测试

![[Pasted image 20230814143417.png]]

### 1.1 %in%
是唯一不进行一一对比的运算符。
作用：
	测试其左边的值是否出现在其右边的对象之中

```r
1 %in% c(3,4,5)
## FALSE FALSE FALSE
c(1,3) %in% c(3,4,5)
## FALSE TRUE
```

*比较两个对象是否相等时应该使用双等号== ，单等号和<-一样*


## 2 布尔运算符
[[## 6.2 Booleans|python 的布尔]]

![[Pasted image 20230814152418.png]]

## 3 环境

R 的环境储存类似于计算机的文件储存

![[Pasted image 20230814164906.png]]

## 4 操作 R 环境
利用 R 提供的一些辅助函数
### 4.1 environment () 
查看当前工作环境
### 4.2 as. environment
接受一个环境名称作为输入，并返回该名称所对应的环境

![[Pasted image 20230814165835.png]]

![[Pasted image 20230814165922.png]]

### assign ()
将对象存储到某个特定环境当中。
用法：
	1. 提供新对象的名称（字符串格式作为输入）
	2. 提供新对象的取值
	3. 提供想要存储的环境名称
```r
assign("new","Hello Global",envir = globalenv())

globalenv()$new
	##"Hello Global"
```
## 4.3 作用域规则


![[Pasted image 20230814170305.png]]

## 闭包
将对象从全局放在运行环境中去

--- 

## S3 系统
三个组成部分：
1. 属性，尤其是 class 属性
2. 泛型函数
3. 方法

attr 接受两个参数：一个 R 对象和某个属性的名称（字符串形式）