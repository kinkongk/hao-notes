## Waht?
---
* 存放一些平时用 Kindle 4 读书时利用 highlight、note、share 操作时保存的文本
* Kindle 会在``documents``目录下生成``My Clippings.txt``文件
* 写了个简单的 Python 脚本``kindle-clippings.py``处理了一下，按照书名进行分类
* 计划定期导出``My Clippings.txt``（其实还有``My Clippings.mbp``文件，供Kindle用的）文件，在本地进行简单处理成``Markdown格式``并同步到 Github 中，否则该文件会越来越占空间，不利处理


## Update 2012-05-03
---
1. 每次执行 ``kindle-clippings.py`` 脚本时以当天日期新建文件夹（例如 ``2012-05-03``）存放生成的 .md 文件
2. kindle 中某些文档是用 ``Send To Kindle`` 或者邮箱推送的``Personal Documents``，此时可能不希望公开邮箱
3. kindle 在 hightlight、note、share 时都保存了具体的时间点，如果不希望公开读书的具体时间（很可能你很晚还在读书 ;-），如下图：

#### 修改前 

![](https://github.com/haolloyin/hao-notes/raw/master/kindle-clippings/images/clippings1.png)

#### 修改后

![](https://github.com/haolloyin/hao-notes/raw/master/kindle-clippings/images/clippings2.png)


## FIXME
---
- ``kindle-clippings.py`` **line 36**，第一个 clip 的书名有个空格？？？所以会被略去，坑爹的bug！！！