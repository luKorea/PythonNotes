# 今日内容

1. 计算机初步认识
2. 解释器的安装
3. IDE安装，编辑代码的软件： Pycharm
4. python入门
5. 交作业：博客/git

# 内容详细

## 1. 计算机的初步认识

![1553653532498](C:\Users\oldboy-python\AppData\Roaming\Typora\typora-user-images\1553653532498.png)

问题

- 常见的操作系统
  - win
    - xp
    - win7
    - win10
    - window server
  - linux
    - centos，图形化界面差
    - ubuntu , 个人开发（图形化比较好）
    - redhat，企业级
  - mac，办公/装逼（入职之前看看mac怎么玩，mac）
- 学习变成语言
  - 安装 解释器/编译器/虚拟机
  - 学习语法

## 2. 解释器安装

1. 下载解释器

   - python 2.7.16 （2020年官方不在维护）
   - python 3.6.8 （推荐）

2. 安装 python 3.6.8
   ![1553654813243](C:\Users\oldboy-python\AppData\Roaming\Typora\typora-user-images\1553654813243.png)

3. 检查python 3.6.8是否安装成功

4. ![1553654949421](C:\Users\oldboy-python\AppData\Roaming\Typora\typora-user-images\1553654949421.png)

5. 添加环境变量，以便于以后快速找到python解释器
   ![1553655345583](C:\Users\oldboy-python\AppData\Roaming\Typora\typora-user-images\1553655345583.png)

   ![1553655538355](C:\Users\oldboy-python\AppData\Roaming\Typora\typora-user-images\1553655538355.png)

6. 重新打开终端并运行python解释器
   ![1553655666481](C:\Users\oldboy-python\AppData\Roaming\Typora\typora-user-images\1553655666481.png)

7.  安装python2.7.16

   ![1553657249633](C:\Users\oldboy-python\AppData\Roaming\Typora\typora-user-images\1553657249633.png)
   ![1553657277239](C:\Users\oldboy-python\AppData\Roaming\Typora\typora-user-images\1553657277239.png)

   





## 3. 第一个脚本（一个文件）

- 打开电脑终端， 功能键+R
- 输入命令： 解释器路径     脚本路径（建议 .py 后缀）

```
print('你好')
```

## 4. 编码

1. 初识编码

   - ascii， 英文，8为表示一个东西，2**8
   - unicode，万国码，32位表示一个东西，2**32
   - utf-8，给unicode压缩，用尽量少的位数表示一个东西，以8个位为单位。

2. python解释器编码

   - py2：ascii , 在文件头部加： 

     ```
     # -*- coding:utf-8 -*-
     print('你好')
     ```

   - py3：utf-8

3. 文件编码

   建议：编写文件时，保存文件要用  utf-8 格式。
   以什么编码保存，就要用什么编码方式打开，否则出现乱码。

## 5. 上午内容回顾

- 计算机基础
- 安装环境
  - 环境变量
  - 多环境共存
- 编码
  - ascii ，8位 = 1字节
  - unicode，32位=4字节
  - utf-8，最少用1字节=8位，最多用4字节=32位表示。 中文：3字节=24位表示。
- 编码 + 解码 一致。
- python
  - py2默认解释器编码：ascii
  - py3默认解释器编码：utf-8

## 6. 解释器

文件：a.py 

```
#!/usr/bin/env python  在Linux中指定解释器的路径
# -*- coding:utf-8 -*-

print('你好')
```

运行： 解释器   文件路径 

在linux上有一种特殊的执行方法：

- 给文件赋予一个可执行的权限
- ./a.py  自动去找文件的第一行 =  /usr/bin/env/python  a.py

## 7. 输出

```
print(你想要输出的东西)
```

特殊：

- py2： print "你好"
- py3： print('你好')

## 8. 数据类型

```
'alex' / "李杰" / ''' asdf ''' / """ dfsf """ , 一般称为字符串。
666 ， 一般称为数字/整形。
True / False , 一般称为 布尔类型。
```

1. 字符串
   - 单引号
   - 双引号
   - 三引号
2. 整型
3. 布尔类型

## 9. 变量

```
content = '钓鱼要钓刀鱼，刀鱼要到岛上钓。'
content = 666
print(content)
```

变量的要求：
1. 变量名只能包含：字母/数字/下划线

2. 数字不能开头

3. 不能是python的关键字。
  [‘and’, ‘as’, ‘assert’, ‘break’, ‘class’, ‘continue’, ‘def’, ‘del’, ‘elif’, ‘else’, ‘except’, ‘exec’, ‘finally’, ‘for’, ‘from’, ‘global’, ‘if’, ‘import’, ‘in’, ‘is’, ‘lambda’, ‘not’, ‘or’, ‘pass’, ‘print’, ‘raise’, ‘return’, ‘try’, ‘while’, ‘with’, ‘yield’]

4. 建议：
  - 见名知意： name = "alex"   age= 18 
  - 用下划线连接：alex_dad = "吴佩其"  

  补充：AlexDad = '吴佩其' （驼峰式命名）

## 10. 综上练习题

```
# 第一题
age = 18
new_age = age + 1 
print(new_age)

# 第二题
name = "alex"
new_name = name + ' sb'
print(new_name)

# 第三题
age = "666"
new_age = age + "666"
print(new_age)

# 第四题
age = "666"
new_age = age + 666 
print(new_age) # 报错


# 第五题
age = 6
new_age = age * 2
print(new_age) 

# 第六题(特殊)
name = "alex"
new_name = name * 2
print(new_name) 

# 第七题
age = 18
value = age >= 19
print(value)

# 第八题
_ = 9 
_9 = 9
9name = 'alex'
True = 9
print = 666 
```



## 11. 输入

```python
user_name = input("请输入你的姓名:")
message = user_name + " 烧饼"
print(message)
```

注意：

- input输入得到的内容永远是字符串。
- py版本区别：
  - py2： name = raw_input('请输入姓名')
  - py3： name = input('请输入姓名')

示例：

```
user_name = input("请输入你的姓名:")
password = input("请输入你的密码:")

content = "你的用户名是：" + user_name + "; 你的密码是：" + password
print(content)
```

## 12 .注释

```
# 单行注释

"""
多行注释
"""
```

## 13. 条件判断

1. 初级条件语句

   ```
   # 请实现一个功能：让用户输入性别，如果是 男，则输出：再见；如果是 女：则输出 来呀来呀；
   
   gender = input("请输入性别：")
   """
   如果是男生：打印再见
   否则：打印来呀来呀
   """
   
   if gender == "男":
   	print('再见')
   else:
   	print('来呀来呀')
   ```

2. elif 条件

   ```
   # 请实现一个功能：让用户输入性别，如果是 男，则输出：再见；如果是 女：则输出 来呀来呀；如果是 人妖：找alex去，他也是。否则：滚
   
   gender = input("请输入性别：")
   """
   如果是男生：打印再见
   否则：打印来呀来呀
   """
   
   if gender == "男":
   	print('再见')
   elif gender == '女':
   	print('来来来')
   elif gender == '人妖':
   	print('找alex去，他也是')
   else:
   	print('滚')
   print('end')
   ```

3. 最简单

   ```
   gender = input("请输入性别：") # 女
   
   if gender == "男":
   	print('再见')
   ```

4. 练习题

   ```
   # 第一题：让用户输入一个数字，猜：如果数字 > 50,则输出：大了； 如果数字 <= 50 ,则输出：小了。
   num = input('请输入一个数字')
   number = int(num)
   if number > 50:
   	print('大了')
   else:
   	print('小了')
   	
   	
   # 第二题：用户名密码登陆
   username = input('请输入用户名：')
   password = input('请输入密码：')
   
   if username == 'alex' and password == "oldboy" : 
   	print('欢迎登陆')
   else:
   	print('用户名或密码错误')
   
   ```



##  14. 今日总结

- 计算机基础（图）
- 解释器的安装
  - py2 & py3 共存，如找到不是自己想要的环境。
- 编码
  - 三种编码区别
  - 用什么保存就用什么打开，硬盘上永远保存的是01010101
  - py2 & py3 
- 输出
- 数据类型
  - 字符串
  - 整形
  - 布尔值
- 变量
- 输入
- 注释
- 条件语句
- 赠送：
  - number = int("666")
  - result  = ''xxx''== 'alex' and 213== '123'  # False
- 提醒：
  - 金山打字通
  - 英文不会
  - 错误笔记



## 15. pycharm安装和使用

安装：

使用：

1. 
   ![1553680080216](C:\Users\oldboy-python\AppData\Roaming\Typora\typora-user-images\1553680080216.png)

2. 创建文件
   ![1553680206964](C:\Users\oldboy-python\AppData\Roaming\Typora\typora-user-images\1553680206964.png)

3. 运行
   ![1553680299250](C:\Users\oldboy-python\AppData\Roaming\Typora\typora-user-images\1553680299250.png)

4. 字体大小
   ![1553680394504](C:\Users\oldboy-python\AppData\Roaming\Typora\typora-user-images\1553680394504.png)

5. 打开其他项目
   ![1553680636484](C:\Users\oldboy-python\AppData\Roaming\Typora\typora-user-images\1553680636484.png)

6. 快速打开文件所在的文件夹

   ![1553680697771](C:\Users\oldboy-python\AppData\Roaming\Typora\typora-user-images\1553680697771.png)



# 今日安排

1. 自己写一个笔记 （typroa） md格式。
2. 作业
   - 找自己会的做。
   - 讨论问题。
3. 找同桌提问



















































