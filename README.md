# 中文博客列表导航项目 v1.0.4 向后端进发！☺
## 1.0.4设计功能：站长平台、管理后台和博客统计
*管理后台*
> 个人的建议：可以使用爬虫爬取+人工审核的方式会稍微好一点。     
> 可以由爬虫收集一些关键词，和一些站点截图。然后提交给人工，人工再从收集到的关键词里手动勾选1~5个标签。      
> 人工审核过程尽量用web显示，优化布局。控制一个站点的审核时长尽量在1分钟以内。人工或许压力会小很多。       
> asforest 2022.03.31

我们之前在维护博客地址库时是直接修改data.json的，费时费力~~（已经吓跑好多人了）~~。希望代码组可以尽早开发出后台。      

*站长平台*

站长在验证自己的站长身份后，可以对于自己的网站数据进行修改、向我们申请存档~~还可能有活动~~。希望代码组可以尽早开发出站长平台。

*博客统计*

我们之后会对博客网站的程序、“死亡”日期、域名变更等等进行记录，并且对程序等信息项绘制统计图表。希望代码组可以尽早开发······

*随机友链*

开往有一个无缝接力，地址是https://github.com/volfclub/travellings#-%E6%97%A0%E7%BC%9D%E6%8E%A5%E5%8A%9B-%CE%B2- ，可以开发出类似的功能方便串门。

*博客分类*

这个想法从我们项目组群的一个建议开始。

> OhYee 2022/3/16
> 
>就我点 travelling 的体验来说，我更希望可以随机到我想看的分类的博客里（甚至具体到技术领域）

目前，标签搜索已经被开发出来，欢迎大家提出建议。    
我们现在正在进行博客标签的添加和指定标签随机跳转工作。

*博客订阅*

我们会开发出opml格式的地址库，供其他项目和组织使用。另外，我们考虑爬取博客的rss，来实现一个页面订阅全列表博客的文章。

*其它想法*

有一些1.0.3剩下的想法，我写在https://github.com/zh-blogs/blog-daohang/blob/main/todo.md 了，希望······

## 说明
我们立志要链接全部的中文独立博客。    
本项目的在线地址是https://zhblogs.ohyee.cc/ ，你可以在网页中点击链接进行串门、交换友链，也可以调查中文独立博客的共性。        
各位大佬可以从https://zhblogs.ohyee.cc/go.html 随机访问博客。        
我们会不定期手动将列表中的博客进行存档。    
为了更好地获取来源博客，请各位站长将指向本导航的链接换为`https://zhblogs.ohyee.cc/?from=你的博客域名`，例如`https://zhblogs.ohyee.cc/?from=www.yayu.net`。 
我们没有强制站长添加链接，以上是指对站长自愿添加的链接的建议。   
我们之后会向上游库提交它们没有收录的博客网站，互通有无。（一些有附带条件的上游库，比如`十年之约`，我们将不会提交）

## 项目如何发现博客
根据超链接，我们可以从种子博客中找到十多个不等的网站地址，这些地址中符合要求的会自动成为新的种子博客。     
理论上来说，博主不需要提交网址，就能被我们发现。  
我们同时也会使用一些上游库（随机排序，排序不带有任何含义）。
| 名称      | 网址 | 是否使用|
| ----------- | ----------- | -------|
| timqian/chinese-independent-blogs      | https://github.com/timqian/chinese-independent-blogs    | 没用完|
| 博客志   | http://www.jetli.com.cn/    | 用完了|
| 中文独立博客导航   | https://www.blogwall.cn/nav/    | 没|
| 博客联盟   | https://blorg.cn/    | 没|
| BLOS'空间   | https://c.sady0.com/   | 用完了|
| BlogFinder   | https://bf.zzxworld.com/  | 没用|
|TUNA Blogroll   | https://github.com/tuna/blogroll | 没|
|bloghub   | https://github.com/shidenggui/bloghub/blob/master/backend/assets/blogs-original.csv | 没|
|十年之约   | https://www.foreverblog.cn/blogs.html | 没用完|
|  BlogRoll  |https://github.com/NUAA-Open-Source/BlogRoll |没|

## 如何支持该项目
1. 如果网站名称或地址出现更换或博客失效，请提个 issue。        
2. 可以为本项目做宣传，让更多人知道本项目。         
3. 程序员可以帮忙实现本项目的功能目标，代码类事务目前交由 @OhYee 和 @Mabbs 进行管理。       
### 博客收录标准
1. 是中文网站（在 html 开头声明`lang="zh"`[^1]）。
2. 是博客网站[^2]且有3篇及以上的公开博文（企业官网发布的为了搜索引擎优化的文章不在博文范围内[^3]）。
3. 具有博客网站的基本属性：
    1. 具有主观性和知识积累性，尊重科学、公认事实、约定俗成和伦理道德，在给出依据和尊重他人的前提下挑战权威者除外。
    2. 具有独立性和自主性，拥有独立域名（可以证明博客使用的域名的所有权，github.io类型除外）。
    3. 具有交互性，提供评论功能或提供博主的个人联系方式。

在收录博客网站时，我们会以非专业的角度评定网站是否符合收录标准，不能排除存在疏漏的可能性。      
任何人可以根据博客收录标准对任一博客的收录资格提出异议。 

[^1]: 在实际操作中，我们有遇到错标成en的博客，我们也会将其收录。（我们会尝试向站长发送邮件建议站长修正）
[^2]: 根据浙江大学李恒的硕士学位论文《博客写作行为影响因素研究》，博客是个人新型的网络出版和交流工具。它是一个个人网站，不同的博客站点可通过链接建立联系．博客的内容由众多个性化表达的帖子组成，不同的帖子按照时间先后倒序排列，帖子的形式可以是文字、影音、图片或链接，或多种形式的结合。对于组织(群体)博客(如情侣博客、团体博客和企业博客)，本项目也会将其送至项目组讨论。
[^3]: 因为一些原因，一些博客需要经过项目组讨论，例如 https://github.com/zh-blogs/blog-daohang/issues/9 。  

## 数据开发说明
data.json中关于数据的说明:

1. `name`指博客网站的名称（一些较长的备用名会放在一句话介绍）
2. `url`指博客网站的网址（不一定是首页）
3. `tag`指博客网站的标签
4. `sign`指博客网站的一句话介绍(有一些没找到，会放空）
5. `status`指博客的状态（可能不准）
6. `feed`指博客的订阅地址（多个地址会填feed 2.0）
7. `gen`指博客使用的程序（还没加）

建议调用本仓库中的data.json，因为这个文件一直在更新。
