VLCWikiForChinese
=================
##项目说明
本项目是[vlccchina](http://vlcchina.org/wiki)的官方wiki，主要来源是[VLC](http://wiki.videolan.org/Main_Page)wiki页面的翻译，以及[vlc中文社区](http://vlcchina.or)的志愿者的贡献。

##预备知识
git和github的基本使用，教程参考链接：

*   [github:help](https://help.github.com/articles/set-up-git)
*   [git和github在ubuntu下的使用](http://www.cnblogs.com/cocowool/archive/2010/10/19/1855616.html)
*   [git，gitflow，github学习心得](http://blog.csdn.net/yeahugo/article/details/7232380)

##项目内容
wiki的主要来源包括以下：

*   [VLC user guide](http://www.videolan.org/doc/vlc-user-guide/en/index.html)
*   [VideoLAN's Documentation](http://wiki.videolan.org/Documentation:Documentation)
*   [VLC Usage Documentation](http://wiki.videolan.org/Documentation:Play_HowTo)
*   [VLC Streaming Documentation](http://wiki.videolan.org/Documentation:Streaming_HowTo)
*   [VLC Streaming Documentation New](http://wiki.videolan.org/Documentation:Streaming_HowTo_New)
*   [The Hacker's Guide to VLC](http://wiki.videolan.org/Documentation:Hacker%27s_Guide)
*   [The VLC Modules Index](http://wiki.videolan.org/Documentation:Modules)
*   [enjoy The Architecture](http://www.enjoythearchitecture.com/vlc-architecture.html)

整体来看，VideoLAN的wiki组织比较松散，因此本项目致力于整合资源，以友好地方式回馈给开源社区。

##项目组织

以文件夹的形式组织章节展开翻译，最后汇总成html和pdf。具体的分布如下：

*   vlc-user-guide  
*   vlc-play-howto
*   vlc-streaming-howto
*   vlc-hacker-guide
*   vlc-modules-howto
*   vlc-arch-guide

分别对应于上面的`项目内容`。

##项目工作流程
###VLC开发小组成员
具有直接edit并commit的权限，工作流简述如下：

1、clone项目

    git clone git@github.com:hustcalm/VLCWikiForChinese.git

2、根据自己展开的工作建立分支，比如enjoythearchitecture的翻译，可以操作如下：

    git branch enjoythearchitecture
    git checkout enjoythearchitecture
3、 在新建分支进行翻译和编辑工作...

4、查看更改并提交，操作如下：
    
    git checkout master
    git merge enjoythearchitecture
    git branch -d enjoythearchitecture
    git diff
    git add .
    git commit -m 'yourcommentshere'
    git push

5、 查看项目的提交记录并更新本地repo

    git log
    git pull

###开源爱好者
如何你对本项目感兴趣，可以fork后进行pull request。

##项目管理
本项目的翻译基于纯文本，使用MarkDown标记语言，关于MarkDown的基本使用，请参考[Markdown语法说明](http://wowubuntu.com/markdown/)。

今后考虑使用Tex，Python、docutils和sphinx。

如果你有更好的建议，请给我们发送邮件。

**VLC开发小组**
