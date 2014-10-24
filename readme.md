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
'''
import sys
reload(sys)
sys.setdefaultencoding('gbk')
'''


