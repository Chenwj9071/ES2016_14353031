### Lab4: 死锁
#### 实验流程：
1.Deadlock.java代码编写及编译（javac Deadlock.java）  
![Deadlock.java](http://a1.qpic.cn/psb?/V12WF66N08IT25/Wd55*mX6PzhP7Th3QIenQif*w9L9MvUB05vqpDg8Sys!/b/dPYAAAAAAAAA&bo=qQFTAakBUwEDACU!&rf=viewer_4)  
![Deadlock.java](http://r.photo.store.qq.com/psb?/V12WF66N08IT25/y9QPaoTMExPHXx7oVMUAgJhIymuAb4YRU5CJ9QRPVFo!/r/dLAAAAAAAAAA)  
2.windows系统下编写批处理文件Deadlock.bat并放到Deadlock.class文件目录下  
![Deadlock.bat](http://a3.qpic.cn/psb?/V12WF66N08IT25/O1jMwRdeP9ACQItg5kz99eagNahRU*WBp1g4nstnH4c!/m/dKoAAAAAAAAAnull&bo=KwGpACsBqQADCSw!&rf=photolist&t=5)    
3.运行Deadlock.bat文件，使Deadlock程序运行100遍，发生死锁时暂停  
运行结果如下，运行第69次时发生死锁：  
![runResult](http://a2.qpic.cn/psb?/V12WF66N08IT25/0qQ3VjioTYgO*pjA1GqT6Ng48ZdWfr*Zw6EYQOfqBxI!/b/dK8AAAAAAAAA&bo=JQJvASUCbwEDCSw!&rf=viewer_4)   
Deadlock程序运行时，流程如下图，a.methodA(b)的执行需要访问class B的代码段，b.methodB(a) 的执行需要访问class A的代码段，
当这两个处于不同线程的函数同时开始执行时，都会因为请求访问的代码段被占用而同时被阻塞，也就是进入了循环等待，死锁产生。
死锁是否会产生取决于count和线程t等待调度的时间  
![流程](http://a1.qpic.cn/psb?/V12WF66N08IT25/0gEtIMLn5ECLQRIjq4PlmDSZTXv0vWjHEyIjEdLgG*o!/m/dMgAAAAAAAAAnull&bo=TQGCAU0BggEBCS4!&rf=photolist&t=5)  


#### 产生死锁的四个**必要条件**：
1.互斥条件：一个资源只能同时被一个进程访问  
2.请求与保持条件：一个进程因请求资源而被阻塞时不释放已获得的资源  
3.非抢占：不能强行剥夺进程已获得的资源  
4.循环等待：若干进程之间形成一种头尾相接的循环等待资源关系  


