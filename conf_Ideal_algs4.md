# 配置 算法（第四版）IntelliJ IDEA环境

***
## 系统配置：win10

### 1、原料
* [官网](https://algs4.cs.princeton.edu/code/)下载源代码`algs4.jar`代码库


* 以及测试用例**algs4-data.zip**
***
### 2、解压缩
* 将**algs4-data**解压缩到指定目录，最好是直接存放在将来所建项目的out文件夹中，out文件夹保存的是编译文件**.class**文件

![图片1](https://github.com/lucklydog/lucklydog.github.io/blob/master/img/%E5%9B%BE%E7%89%871.png?raw=true)

* 将**algs4.jar**库函数保存在所安装java的目录里，如：`C:\Program Files\Java\jdk1.8.0_191\jre\lib\ext\algs4.jar`

![图片2](https://github.com/lucklydog/lucklydog.github.io/blob/master/img/%E5%9B%BE%E7%89%872.png?raw=true)
***
### 3、配置环境变量
> **此电脑**
>>**属性**
>>>**高级系统设置**
>>>>**环境变量**（用户变量中的path，系统变量中的path，以及新增一个CLASSPATH环境变量,路径为上述**algs4.jar**的路径）
>
>**Click ok three times**

![图片3](https://github.com/lucklydog/lucklydog.github.io/blob/master/img/%E5%9B%BE%E7%89%873.png?raw=true)

***
### 4、配置IDEA
### 导入jar：
**file**--->**Project Structure**--->**Modules**---->**Dependencis**--->**+**--->**JARS or directories**--->**添加algs4.jar的路径**--->**ok**

![图片4](https://github.com/lucklydog/lucklydog.github.io/blob/master/img/%E5%9B%BE%E7%89%874.png?raw=true)

***
### 5、利用idea编译java程序
* 1、编译好的class文件会默认保存在**out**文件夹中，正是上述所说将**algs4-data**中的测试数据存放的地方


* 2、你也可以使用**Terminal**终端来进行编译，编译的文件路径为**../src/<项目文件夹>**文件，命令为`javac XX.java`,编译后的class文件默认是在**src/<项目文件夹>**中，不是在out文件夹中！

![图片5](https://github.com/lucklydog/lucklydog.github.io/blob/master/img/%E5%9B%BE%E7%89%875.png?raw=true)

***
### 6、执行class文件

在执行文件的时候需要注意一点，就是由于我们的项目都是有package的，需要回退到你项目的那个目录才能执行class文件

而且class文件的文件名要为**<项目名称>.<类名>**

例如：`java Sort.Example`

![图片6](https://github.com/lucklydog/lucklydog.github.io/blob/master/img/%E5%9B%BE%E7%89%876.png?raw=true)

***

### 7、注意事项
**通过Idea的Terminal终端可能不会随时更新环境变量，记得配置完环境变量要重启IDEA！**



