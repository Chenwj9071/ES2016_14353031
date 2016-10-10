### Lab2: DOL 实例分析&编程
#### 实验任务1：
**要求：**修改example2，让3个square模块变成两个  
**修改方式：**把example2.xml文件中的迭代次数设为2，即把N的值设为2.  
![修改](http://a1.qpic.cn/psb?/V12WF66N08IT25/PyM*SmwLnu9YLLgfXI5FyCrL81Xozeo0GpSdX8zz1*8!/m/dAwBAAAAAAAAnull&bo=qwLWAKsC1gABCS4!&rf=photolist&t=5)  
**运行结果**如下（sudo ant –f runexample.xml –Dnumber=2）：  
![runexample2](http://a4.qpic.cn/psb?/V12WF66N08IT25/TXhSub5HbzmEusr04LZI2W5Zxs2ep7J9U8dS8*c9o7Q!/m/dAsBAAAAAAAAnull&bo=PAKOATwCjgEBCS4!&rf=photolist&t=5)  
**系统架构图**（.dot）如下：  
![dot](http://a3.qpic.cn/psb?/V12WF66N08IT25/BkbEt2E4Ih8Ji1bdhoZlduh1vPuCuK4YDekFdqX4e0U!/m/dAoBAAAAAAAAnull&bo=1QJHANUCRwABCS4!&rf=photolist&t=5)  

#### 实验任务2：
**要求：**修改example1，使其输出3次方数  
**修改方式：**在square.c文件中把计算平方的表达式改成计算三次方（i = i * i * i）。  
![修改方式](http://a3.qpic.cn/psb?/V12WF66N08IT25/HpT5aAFtY1kS5xpHLKDVdA9iTxQ6VrwzyiuaDTQPJ9o!/m/dAoBAAAAAAAAnull&bo=kgFaAJIBWgABCS4!&rf=photolist&t=5  )  
**运行结果**如下（sudo ant –f runexample.xml –Dnumber=1）：  
![runexample1](http://a4.qpic.cn/psb?/V12WF66N08IT25/buJ5N2ZNIIGDCHYjyPj.BeD0gAU9YpllePQHHhGBSMU!/m/dHcBAAAAAAAAnull&bo=RgKUAUYClAEBCS4!&rf=photolist&t=5)  
**系统架构图**（.dot）如下：  
![dot](http://a3.qpic.cn/psb?/V12WF66N08IT25/p.ba4H2VztRvziElnR6xJC9q4UcKj*IAW5I1WQ2tnrY!/m/dNoAAAAAAAAAnull&bo=.wFGAPsBRgABCS4!&rf=photolist&t=5)  

### 实验感想
1.这一次实验课需要学习了解的内容比较多，但实验课上的讲解十分详细易懂，主要以example为例，分析讲解dol中一个实例的结构组成以及一些编码规范和实现细节。
2.在对所讲内容有所了解的基础上，实验任务十分简单，反而是安装打开dot文件的工具花费了一些功夫。
