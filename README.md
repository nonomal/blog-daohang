# 中文博客列表导航项目 v1.0.4 向后端进发！☺

![forks](https://img.shields.io/github/forks/zh-blogs/blog-daohang) ![starts](https://img.shields.io/github/stars/zh-blogs/blog-daohang) ![license](https://img.shields.io/github/license/zh-blogs/blog-daohang)
## 1.0.4新功能：博客在线提交
最近，技术组开发出了博客在线提交功能。各位站长可以在 https://zhblogs.ohyee.cc/manager/join/ 直接提交自己的博客网站。       
其它功能还在开发中。


## 这个项目是什么？
我们这个项目立志要链接全部的中文独立博客。    
本项目的在线地址是https://zhblogs.ohyee.cc/ ，你可以直接在网页中点击链接进行串门，也可以根据列表调查中文独立博客的共性。        
各位大佬可以从 https://zhblogs.ohyee.cc/go 随机访问博客。          
为了更好地获取来源博客（相关博客推荐功能正在开发），请各位站长将指向本导航的链接换为`https://zhblogs.ohyee.cc/?from=你的博客域名`，例如`https://zhblogs.ohyee.cc/?from=www.yayu.net`。 
我们并没有强制站长添加链接，以上是指对站长自愿添加的链接的建议。   
我们之后会向上游库提交它们没有收录的博客网站，互通有无。（一些有附带条件的上游库，比如`十年之约`，我们将不会提交）

## 项目如何发现博客？
1. 根据超链接，我们可以从种子博客中找到十多个不等的网站地址，这些地址中符合要求的会自动成为新的种子博客。理论上来说，博主不需要提交网址，就能被我们发现。  
2. 我们同时也会使用一些上游库。


## 如何支持该项目？
1. 如果网站名称或地址出现更换或博客失效，请提个 issue。        
2. 可以为本项目做宣传，让更多人知道本项目。         
3. 程序员可以帮忙实现本项目的功能目标，其他人可以加入我们共同维护地址库，代码类事务目前交由 @OhYee 进行管理。   

## 博客收录标准是什么？
1. 是中文网站（在 html 开头声明`lang="zh"`[^1]）。
2. 是博客网站[^2]且有3篇及以上的公开博文（企业官网发布的为了搜索引擎优化的文章不在博文范围内[^3]）。
3. 具有博客网站的基本属性：
    1. 具有主观性和知识积累性，尊重科学、公认事实、约定俗成和伦理道德，在给出依据和尊重他人的前提下挑战权威者除外。
    2. 具有独立性和自主性，拥有独立域名（可以证明博客使用的域名的所有权，github.io类型除外）。
    3. 具有交互性，提供评论功能或提供博主的个人联系方式。

在收录博客网站时，我们会以非专业的角度评定网站是否符合收录标准，不能排除存在疏漏的可能性。      
任何人可以根据博客收录标准对任一博客的收录资格提出异议。

## 博客网站还需要注意什么细节？
为了方便程序和人工维护列表，请各位网站修一下下面的细节：
1. 在头部用link标签指向rss（在导航栏用一个rss图标链接也行），或通过告诉我们你使用的网站程序让我们尝试该程序默认的feed地址。（一些没声明的网站我们会用/feed,/atom.xml去试，非常累。并且你的声明是有些订阅器搜索feed地址的基石）
2. 用generator告诉我们你的网站使用的程序（不需要版本号）。
3. 尽量不要用js之类的做防复制，我们人工添加网站的时候都是用复制粘贴。防复制的方法防君子不防小人。 

[^1]: 在实际操作中，我们有遇到错标成en的博客，我们也会将其收录。（我们会尝试向站长发送邮件建议站长修正）
[^2]: 根据浙江大学李恒的硕士学位论文《博客写作行为影响因素研究》，博客是个人新型的网络出版和交流工具。它是一个个人网站，不同的博客站点可通过链接建立联系．博客的内容由众多个性化表达的帖子组成，不同的帖子按照时间先后倒序排列，帖子的形式可以是文字、影音、图片或链接，或多种形式的结合。对于组织(群体)博客(如情侣博客、团体博客和企业博客)，本项目也会将其送至项目组讨论。
[^3]: 因为一些原因，一些博客需要经过项目组讨论，例如 https://github.com/zh-blogs/blog-daohang/issues/9 。  

## 本仓库有关文档

[规范文档](https://github.com/zh-blogs/zh-blogs-documentation)

[开发文档](doc/develop.md)
