### 简介
建造者模式用于将**复杂对象**的**构建**和**表示**分离，使得相同的构建过程可以 创建 不同的表示。  
建造者模式适用于：  

* 对象的各个组成部分的构建顺序**稳定**
* 对象的构建过程可以**独立于**对象的组成部分，也独立于组成部分的装配方法
* <span style="color:red">**当一个构造方法有多个参数时，需要考虑建造者模式** </span>   

---

### 角色

* Builder  
一个抽象类或接口。该接口声明：*构建对象的各个组成部分的方法以及返回被构建的产品对象的方法*。**Builder不会涉及到构建<span style="color:green">过程</span>**  
* ConcreteBuilder   
实现Builder接口。每个具体建造者对应于对象的一种**表示**   
* Director   
负责定义对象的各个组成部分的构建顺序
* Product    
要创建的**复杂对象**

---

## UML类图  

![builder.png](http://timd.cn/content/images/2017/07/builder.png)