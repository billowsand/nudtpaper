# 国防科学技术大学论文模版 
这个版本是从https://github.com/liubenyuan 的那里克隆的，做了如下相关改进：

1. 增加了对于mac系统的支持，支持mac下的宋体，楷体和黑体，同时mac下的等宽字体使用Manaco。
2. 修改了代码宏包，使用minted作为代码宏包，可以使用多套代码高亮主题，同时支持对于代码的编号和建立目录索引。
3. 支持了texlive 2014，解决了一些bug。


由于使用了Minted代码高亮宏包，需要安装Python环境，并且通过pip install Pygments安装Pygments宏包才可以运行。

## 在windows下安装Pygments宏包

1. 下载和安装python2.7，安装时选择加载环境变量 https://www.python.org/ftp/python/2.7.8/python-2.7.8.msi
2. 下载setuptools https://pypi.python.org/pypi/setuptools
3. 解压后进入setuptools的目录运行：python setup.py install
4. 下载pip，https://pypi.python.org/pypi/pip
5. 解压后进入pip的目录运行：python setup.py install
6. 在环境变量中加入：C:\Python27;C:\Python27\Scripts
7. 重启终端，运行pip install Pygments

运行过程中遇到asccii code问题在出问题的python文件中加入下面代码：
```
import sys
reload(sys)
sys.setdefaultencoding('gbk')
```



## 使用什么模板

### Windows
windows下的同学可以使用Ctex或者texlive 2014，分别使用下面的版本

ctex：https://github.com/liubenyuan/nudtpaper
texlive：https://github.com/billowsand/nudtpaper/tree/patch-1
会用Python的同学可以考虑这个模板，有很好的代码优化：
texlive：https://github.com/billowsand/nudtpaper

### Mac，Linux
mac下的同学使用MacTex作为latex版本，mac下的python是自带的，可以直接通过pip安装代码高亮包，所以建议使用这个版本
https://github.com/billowsand/nudtpaper

## 使用什么编辑器
很多人搞不清楚编辑器和latex的关系，Latex就相当于你在电脑上安装了gcc，像写C程序一样需要使用一个编辑器去编辑Latex代码，所以好的编辑器可以协助你高效工作。

### windows
Winedit是最好用的Latex编辑器，也只有在windows下可以使用。但记住要使用8.0以上的版本，否则无法打开。

### mac，linux

这两个平台建议使用sublimeText+LatexTools

使用方法参考这篇文档：http://www.readern.com/sublime-text-latex-chinese-under-mac.html


## 关于PDF图片的问题
使用visio画图时插入Latex中出现空白的问题是因为导出的PDF格式有问题，需要在visio导出时使用“符合PDF/A标准”，不能包含visio的多余信息

## 关于字体的问题

一般大家只要安装了adobe的三个中文otf字体都没有什么问题。

希望大家有什么问题可以反馈给我，及时更新。


