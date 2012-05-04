gvimIM (vim IMproved)
=============

Vim官网版只提供有限的功能，因为Vim的作者鼓励开发者独自进行编译，其中许多实用的功能并未打开。

在没有任何配置文件的情况下，Vim相比其它文字编辑器并没有明显优势，在中文环境下甚至有很多体验问题，如使用非等宽字体，中英输入法切换，gvim菜单撕不下来，光标跟随等问题，这些问题常常导致初学者放弃使用Vim，而官方解决这些问题的速度也不容乐观，这些都严重影响这个优秀编辑器在中国的推广。  

另外简单说来，Vim本身就像是个优秀的进口发动机，我们必须要搭配一些优秀的配件（插件），再进行本地化改良，才能让它发挥最大的效用。

本项目旨在解决上述问题，为Vim爱好者提供更合中国人习惯的，功能完善体贴的Vim，并降低Vim的使用门槛，它主要做以下工作：

* 提供全中文的体验（俗称汉化，实际上Vim的国际化支持已经非常好了，只是需要有人整理一下）
* 提供增强配置文件（vimrc）
* 集成并维护常用插件
* 对官方没及时解决的bug修改及时修改源码予以解决
* 提供完善的文档以及小工具
* 绿色化，下载就能用

项目维护者: <http://t.qq.com/michalliu>

使用之前
-----------------------
1. 推荐安装[python 2.7](http://python.org/getit/)，以便启用vim与python集成，否则有些插件不能正常工作
2. 为了获得最佳体验，请手动安装misc\fonts下的Menlo.ttc
3. 路径不要含有中文，否则会引起菜单报错及主菜单乱码问题

集成插件列表
-----------------------

请参阅misc/docs目录，以获得这些插件的详细文档。

1. jshint,jsruntime

    javascript静态语法检查与运行器
    
        :JSHintUpdate 检查语法
        :RunJS 运行javascript代码
        :RunJSBlock 运行部分javascript代码，如:RunJSBlock 1,3 运行1-3行的代码
        :RunHtml 运行Html代码
        :RunHtmlBlock 运行部分Html代码
   
2. [pyflakes](http://www.vim.org/scripts/script.php?script_id=2441)

    python静态语法检查 
   
3. statusline

    增强vim状态条 statusline
   
4. [load_template](http://www.vim.org/scripts/script.php?script_id=2957)

    模板加载
    
        :LoadTemplate
    
5. [NERD_commenter](http://www.vim.org/scripts/script.php?script_id=1218)

    支持多种类型文件的快速注释
    
        \cc 注释单行
        \cm 注释多行
    
6. [css_color](http://www.vim.org/scripts/script.php?script_id=2150)

    把css中的颜色定义显示为真实颜色
    
7. [Matrix](http://www.vim.org/scripts/script.php?script_id=1189)

    很酷的黑客帝国屏保
    
        :Matrix
    
8. [TeTrls](http://www.vim.org/scripts/script.php?script_id=172)

    用vim快捷键操作的俄罗斯方块，适合初学者练习指法
    
        \te 开始游戏，游戏启动稍慢，请耐心等待
        <h>;<l>;<j>;<k>; 移动
        <Space> 放下
        <Esc>获取<q> 退出
    
9. 增加9种额外的优秀配色方案

    分别是_zenburn;ir_black;pyte;railscasts;rdark;tango2;twilight;_
    
        :color {name}
        
10. [vimtweak](http://www.vim.org/scripts/script.php?script_id=687)

    [vimtweak](https://github.com/mattn/vimtweak)在windows下允许gVim.exe获得窗口半透明及全局置顶的效果，屏幕分辨率低的时候可以籍此避免窗口切换。
    
        :SetAlpha 200 窗口透明度为200
        :SetTopMost 1 窗口总在最前

特别感谢
-----------------------
vim中文文档 <http://vimcdoc.sourceforge.net/>

