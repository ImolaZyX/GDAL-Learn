## GDAL+VS配置及第一个程序

### 1.GDAL+VS配置

在已经装好Visual Studio 的前提下，下载老师提供的gdal头文件，lib包和dll文件，然后开始新建工程添加代码，以下是代码截图

[![iGTFVU.png](https://s1.ax1x.com/2018/10/07/iGTFVU.png)](https://imgchr.com/i/iGTFVU)

[![iGTVPJ.png](https://s1.ax1x.com/2018/10/07/iGTVPJ.png)](https://imgchr.com/i/iGTVPJ)

将gdal头文件和lib文件放置在工程目录下，并且将dll文件放置在Release目录下之后，编译运行得出正确的结果

[![iGobb8.png](https://s1.ax1x.com/2018/10/07/iGobb8.png)](https://imgchr.com/i/iGobb8)

以及生成的两幅图，左为jpg格式，右为tif格式

[![iGTZG9.jpg](https://s1.ax1x.com/2018/10/07/iGTZG9.jpg)](https://imgchr.com/i/iGTZG9)

### 2.遇到的问题及解决方法

遇到的问题主要是编译器的配置问题

（1）在Windows10操作系统中，文件操作都正确的情况下，Visual Studio 2017不能够识别lib库，编译时报错以至于运行出错。一直未找到针对性解决方案，只能安装老师推荐的VS2010。

（2）在Visual Studio 2015环境下，创建windows命令行程序键入代码后，尝试用第三方库管理插件NuGet安装gdal库，结果运行报错。之后更改为从老师给的库中下载gdal库，将其放置于项目根目录下后，编译通过。
