# 网站解释

## _data文件夹

### contact.yml

是用来显示首页中的联系人人信息的，暂存为我的

### feature.json

是用来调整主页下部那三个图片及其文字的，可用性较强。

暂修改，中文测试通过

### menu.yml

看起来是用来当导航栏的，可修改成中文。

- service修改成技术文章
- team修改成团队
- about可以删去或者修改成Wiki
- Contact修改成联系我们，并给出一些事件描述
- 然后将team的权重和service互换。
- footer中Home改成主页
- Contact改成联系我们。
修改完成。

### seo.yml

一个用来搞搜索优化的；

SEO是英文Search Engine Optimization的缩写，中文译为“搜索引擎优化”。简单地说，SEO是指从自然搜索结果获得网站流量的技术和过程。更严谨些的定义可以表述为：SEO是指在了解搜索引擎自然排名机制的基础上，对网站进行内部及外部的调整优化，改进网站在搜索引擎中的关键词自然排名，获得更多流量，从而达成网站销售及品牌建设的目标

### social.yml

一些社交账号，可修改，暂时不知道如何增加。


## _includes

看起来挺复杂的，而且有诸多声明，暂且不知道如何更改。

### main-menu.html
中有一句{% assign mainmenu = site.data.menus.main | sort: 'weight'  %}

看起来是可以根据weight修改前后的，之后可以试试。可以参考menu.yml中定义来看。

和mobile八九不离十。


### google-analytical

直呼看不懂，似乎和SEO有关；

内部查看，应该没有什么大问题

### main-menu-mobile

{}是Liquid语法，这个不急着学。

### social.html

{%% }看起来应该是一个用来免除繁重声明工作的语句。
这么一看，里面很多都可以理解了。
里面用来写知乎啊github啊之类的东西。

### call.html

应该是引入一些东西，如果被定义，则引入这些。看起来那个修改后的contact就是它的功劳。

的确，加入！后就变成了contact！

这个部件的意义在于联系模块的分析。这些class应该是用来sass样式控制的。

### footer.html
类似

### hamburger.html
搜索之后发现大有来头。hamburger网页是里面那个三道杠的东西，由于其和汉堡很像，而且十分贴切用户使用习惯。

在mobile中使用。

### header.html
看起来像导航栏，其纳入了main-menu和hamburger，

sub-footer看起来像是尾部的。

## _layout

看起来就复杂、看起来需要结合F12，以及前面的include查看。
但是目前仍然不知道各种声明和class的作用。

### default
是专门的页面，就是本身页面的。日后的整体修改都可以参照此页面。
使用Liquid语法，

页面的控制代码都是控制布局的，所以是layout，没有什么更改的必要，。

### home
修改只输出6个轻轻松松。

其余的等到后面修改。

## images

所有图片出自于此，理论上修改此处图片即可达到更改效果。

问题有二：

1. 此处是否是源图片，是的

2. 名字是否重要？没有那么重要，和前面引用一致即可。