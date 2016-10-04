### DOL框架描述
DOL是一个允许程序自动或半自动地映射到多处理器图形架构平台的**框架层**，由三部分组成：
* **DOL应用编程接口：** DOL定义了一组用于分布式编程、图形平台并行应用的计算和通信的程序，应用程序开发者可以使用这些程序接口而不用关心底层的实现细节。
* **DOL功能仿真：** 为程序员测试应用程序提供了一个功能仿真框架，基于应用程序的功能验证，可在应用层获得程序的性能参数。
* **DOL映射优化：** 计算一组应用程序到图形架构平台的优化映射。

### DOL安装笔记
1. 首先下载DOL程序包，[下载地址](http://www.tik.ee.ethz.ch/~shapes/downloads/dol_ethz.zip)，并解压到要安装的文件夹。
2. 之前已配置好Java环境。
3. 安装ant，指令：**sudo apt-get install ant** 。
4. 将解压好的Systemc文件放到根目录下的systemc-2.3.1文件夹，在命令行窗口进入这个文件夹并新建一个临时文件夹obidir(**mkdir obidir**)并进入（**cd obidir**），然后运行configure (**../configure CXX=g++ --disable-async-updates**) 。  
![enter description here](http://a2.qpic.cn/psb?/V12WF66N08IT25/4oShW5HAVK4Ysd4ItHEpIDuA8K4.A8z7JcdOOhfGRbY!/m/dLEAAAAAAAAAnull&bo=6gFVAeoBVQEDCSw!&rf=photolist&t=5)
5. 编译systemc：（**sudo make install**）,完成后记录当前工作路径。    
![enter description here](http://a1.qpic.cn/psb?/V12WF66N08IT25/OJf03WgzNYgjcrHxWJ9JlOqY0sR9qeJfRi6CWfjURNs!/b/dLEAAAAAAAAA&bo=xAF7AMQBewADACU!&rf=viewer_4)
6. 编译DOL：进入dol文件夹（**cd ../dol**）,按要求修改build_zip.xml文件。然后编译（**ant -f build_zip.xml all**）,成功后结果如下：  
![enter description here](http://a3.qpic.cn/psb?/V12WF66N08IT25/kI3WByJ9Pvlsm5*PnEMPI7hdUQuEBF8YqjSnGVz7e10!/b/dPgAAAAAAAAA&bo=jwFAAY8BQAEDACU!&rf=viewer_4)
7. 进入build/bin/mian路径下，运行例子（**ant -f runexamble.xml -Dnumble=1**），结果如下：
![enter description here](http://a2.qpic.cn/psb?/V12WF66N08IT25/GIqAcAz7Tofc*dGCuUxCfsAIHLj5Y12B8Ryy9Hq2X0c!/b/dK8AAAAAAAAA&bo=GwFNARsBTQEDACU!&rf=viewer_4)  
流程图  
![流程图](http://a2.qpic.cn/psb?/V12WF66N08IT25/UtVE0Q39QHkZBqWA20mR7iTZeXKvLZHmqTIc6IlSqvo!/m/dP0AAAAAAAAAnull&bo=JAJeACQCXgADCSw!&rf=photolist&t=5)

### 实验心得
1. 上学期在操作系统课程中安装过虚拟机并配置了Ubuntu系统，以及配置了pintos系统和Java环境等，积累了一定经验，配置dol时省了不少工作，过程比较顺利，也没有遇到奇怪的问题。
2. 虽然顺利配置好了，但对于这个东西有什么用还不是特别了解，期待后面的实验。
