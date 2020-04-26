___python解释器___  
当我们编写Python代码时，我们得到的是一个包含Python代码的以.py为扩展名的文本文件。要运行代
码，就需要Python解释器去执行.py文件。

由于整个Python语言从规范到解释器都是开源的，所以理论上，只要水平够高，任何人都可以编写
Python解释器来执行Python代码（当然难度很大）。事实上，确实存在多种Python解释器。

CPython:当我们从Python官方网站下载并安装好Python 3.x后，我们就直接获得了一个官方版本的解释
器：CPython。这个解释器是用C语言开发的，所以叫CPython。在命令行下运行python就是启动CPython
解释器。
CPython是使用最广的Python解释器。教程的所有代码也都在CPython下执行。

IPython:IPython是基于CPython之上的一个交互式解释器，也就是说，IPython只是在交互方式上有所
增强，但是执行Python代码的功能和CPython是完全一样的。好比很多国产浏览器虽然外观不同，但内
核其实都是调用了IE。
CPython用>>>作为提示符，而IPython用In [序号]:作为提示符。

PyPy:PyPy是另一个Python解释器，它的目标是执行速度。PyPy采用JIT技术，对Python代码进行动态
编译（注意不是解释），所以可以显著提高Python代码的执行速度。
绝大部分Python代码都可以在PyPy下运行，但是PyPy和CPython有一些是不同的，这就导致相同的Py
thon代码在两种解释器下执行可能会有不同的结果。如果你的代码要放到PyPy下执行，就需要了解
PyPy和CPython的不同点。

Jython:Jython是运行在Java平台上的Python解释器，可以直接把Python代码编译成Java字节码执行。

IronPython:IronPython和Jython类似，只不过IronPython是运行在微软.Net平台上的Python解释器
，可以直接把Python代码编译成.Net的字节码。

___python环境安装___   
针对各位程序猿朋友来讲，大家常规使用的操作系统主要集中在Linux和Windows，python的安装针对
两种不同的系统安装方式是不一样的。下面将针对Linux(Ubuntu16.04)、Windows10作为初始环境进行
python安装介绍:   
1、Ubuntu   
其实针对当前时间点Ubuntu官方更细的系统来看，大家是不需要通过手动对系统进行python开发环境
安装的，目前发布的Ubuntu操作系统在安装完成后似乎都是携带python开发环境的，之前是只存在pyth
on2的环境，现在好像python2和python3是都具备的，所以在此不做过多的介绍。   
2、Windows10   
和Ubuntu不同的是，Windows10是需要大家手动安装python环境的。首先大家进入
python[下载地址](https://www.python.org/downloads/release/python-350/)下载应用程序，下载完
成后大家就可以像安装常规软件一样对其进行安装了(傻瓜式的点击即可)，需要注意的是，大家在
进行安装的同时需要将界面上将python添加到系统环境变量的位置选上，免得后面在手动进行系统
环境变量设置。否则大家进入CMD之后键入python，系统将会提示这不是系统可识别的命令。

