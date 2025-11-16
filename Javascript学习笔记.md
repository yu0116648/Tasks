# Javascript学习笔记

## 基础语法

### 变量声明

var name=“John”；

let age=25；        //变量，可以重新赋值

const PI=3.14;       //常量，不可重新赋值

### 数据类型

#### 原始类型

* let str ="hello";
* let num=42;
* let bool=ture;
* let undef=null
* let sym=Symbol("id");

### 引用类型

* let obj={name："John",age:25};
* let arr=[1,2,3];
* let func=function(){return"Hello";};

## 函数

### 函数定义

* 函数声明：

​                       function add(a,b){

​					   return a+b;}

* 函数表达式：

  ​                const multiply=function(a,b){

  ​                return a*b;}

* 箭头函数：

    			  const divide=(a,b)=>a/b;

### 参数处理

* 默认参数：

  function greet(name="Guest"){

  ​       return 'Hello,${name}!';

  }

* 剩余参数;

  function sum(...numbers){

  ​      return numbers.reduce((acc,curr)=>acc+curr,0);

  }

## 数组方法

const numbers=[1,2,3,4,5];

* 遍历: numbers.forEach(num=>console.log(num));
* 映射：const doubled=numbers.map(num=>num*2);
* 过滤：const even =numbers.filter(num=>num%2===0);
* 查找：const found=numbers.find(num=>num>3);
* 包含检查：const hasThree= numbers.include(3);