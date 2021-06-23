# 将3DEC5.2的结果导入Tecplot360进行后处理(3DEC2Tecplot)
This is used to output the model information of 3DEC5.2  into the input format of Tecplot360((3DEC2Tecplot))

## 1.3DEC2Tecplot360

跟UDEC一样，我将以前在网上搜集到的转换脚本进行了改写，同样发现了原脚本中的应力输出是错误的，在新脚本中进行了更正。

此脚本目前可以输出以下变量：

1. 节点位移（X,Y,Z,MAG）
2. 节点速度（X,Y,Z,MAG）
3. 单元应力（SXX,SYY,SZZ,SXY,SXZ,SYZ,SIG1,SIG2,SIG3,MISES）

我在新脚本中进行了详细的注释，便于有其他输出需求的小伙伴进行改写扩充。


## 2.测试对比模型

在3DEC中进行了一个简单边坡模型的计算，模型如下：

![](https://image.geomatlab.com/image/20210623210042.png)

将模型计算的位移，速度，应力等进行输出测试，使用Tecplot360 进行读取对比。（测试使用的是**Tecplot 360 EX 2017R3**版本）



## 3.对比结果



### **MESH**

![](https://image.geomatlab.com/image/20210623210013.png)

![](https://image.geomatlab.com/image/20210623214455.png)



### **YDISP**

![](https://image.geomatlab.com/image/20210623210438.png)

![](https://image.geomatlab.com/image/20210623212926.png)



### **ZDISP**

![](https://image.geomatlab.com/image/20210623210546.png)

![](https://image.geomatlab.com/image/20210623213003.png)



### **DISP-MAG**

![](https://image.geomatlab.com/image/image-20210623210628344.png)

![](https://image.geomatlab.com/image/20210623212804.png)

### **YVEL**

![](https://image.geomatlab.com/image/20210623210812.png)

![](https://image.geomatlab.com/image/20210623213129.png)

### **VEL-MAG**

![](https://image.geomatlab.com/image/20210623210849.png)

![](https://image.geomatlab.com/image/20210623213206.png)



### **SYY**

![](https://image.geomatlab.com/image/20210623210654.png)

![](https://image.geomatlab.com/image/20210623213554.png)



### **SIG3**

![](https://image.geomatlab.com/image/20210623210719.png)

![](https://image.geomatlab.com/image/20210623214151.png)

### **SIG1**

![](https://image.geomatlab.com/image/20210623211136.png)

![](https://image.geomatlab.com/image/20210623214121.png)

### **MISES**

![](https://image.geomatlab.com/image/20210623210738.png)

![](https://image.geomatlab.com/image/20210623214411.png)

