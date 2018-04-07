# selenium

* 一个基于selenium的web自动化测试框架
* 从以前所写的automation_demo里面分离出来。(https://github.com/afantishui/python_automation_demo)

## 所需组件

* selenium （https://pypi.python.org/pypi/selenium#downloads）
* Python3  （https://www.python.org/downloads/）
* PyCharm  （https://www.jetbrains.com/pycharm/download/）
* 浏览器驱动（IE,Chrome,Firefox，在tools目录下）

## 环境搭建
* python3.6+selenium 2.45+chrome55.0+chromedriver2.8(多次报错中能调试的组合)
*  a.安装Python 
*  b.配置环境变量
*    修改我的电脑->属性->高级->环境变量->系统变量中的PATH为:
*    变量名：PATH
*    变量值：;C:\Python35;C:\Python35\Scripts;（根据实际安装目录路径修改）
*  c.安装selenium
*    通过pip 安装
*    cmd进入Python目录：
*    C:\Users\fnngj>python3 -m pip install selenium 
*    通过下载包安装
*    或者直接下载selenium包：https://pypi.python.org/pypi/selenium
*    解压，cmd进入目录:C:\selenium\selenium2.53.5> python3 setup.py install
*  d.安装Chrome driver
*  e.安装IE driver
*    selenium的版本要与IEDriver版本对应
*    http://selenium-release.storage.googleapis.com/index.html
*    http://blog.csdn.net/zyl26/article/details/51011073
*    这两个加载驱动直接放到Python安装目录中，安装目录配置环境变量（C:\Python35;C:\Python35），使用的版本要与浏览器版本对应
*  f.HTMLTestRunner.py文件放在Python\Python\Lib目录下面（这是Python3的）

## 简单调试代码：
* 谷歌浏览器打开
*  from selenium import webdriver
*  driver = webdriver.Chrome()
*  driver.get("https://www.baidu.com")
*  print(driver.title)
* 用IE浏览器打开：
*  from selenium import webdriver
*  driver = webdriver.Ie()
*  driver.get("https://www.baidu.com")
*  print(driver.title)

## 插件安装
* fireBug
* 火狐浏览器(32版本，不能太高) 工具栏-->附件组件-->下载fireBug-->安装后点击右键查看元素
* firepath(安装与使用 同上)

## 基本功能
* 封装一下webdriver的基本方法，在framework\base_page.py
* 简单的Log类，输出日志
* 使用unittest进行测试用例管理
* HTMLTestRunner 测试报告




