
# 安装环境
**首先声明，我用的是ubuntu20.04。**
既然要用到jekyll，我们就先需要把jekyll装好，但是jekyll也需要依赖：
```
sudo apt-get ruby-full						//这个是jekyll需要的依赖，为了完整性我选择了full
```
然后我们先进行下一步。
# 新建一个库
在github上新建一个库，命名为`你的git用户名.github.io`。

进入`setting`,下翻到`github page`,修改`source`,这是你的个人博客的资源文件。你可以先点击

`https://user.name.github.io/`看看默认的页面。

**这也就是你之后的个人博客的网址。**

![示例](https://img-blog.csdnimg.cn/2020120522150425.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl81Mjc5NjI3Mg==,size_16,color_FFFFFF,t_70#pic_center)
在本地新建一个你的本地git仓库，你可以先`git clone <你自己的资源仓库的url>`，然后把里面

的文件都清空。

`tip:`别把`.git`给删了！！！
# clone一个喜欢的jekyll模版
你可以在类似[jekyllthemes](jekyllthemes.org)这类网站中找一个自己喜欢的Jekyll模版，然后进入它的资

源仓库，把他的URL复制下来。之后在本地新建一个文件夹用来暂时存放这个主题。
```
mkdir /路径
cd /路径
git clone <url>
```
好了，现在你已经把这个主题`clone`下来了，现在你要做的就是把除`.git`以外的文件全部转

移到你用来连接你自己的远程git仓库的本地git仓库里去。
# 开始正题
运行以下命令
```
bundle jekyll
```
经过漫长的等待，你的就只差最后一步了。
```
git push <origin> <分支>
```
把这些资源文件推送到你的远程git仓库用来存储资源文件的分支里去。

**打开之前github分配给你的网址，见证奇迹吧~**

`tip:`如果没有变化，请耐心等一等。
# 修改_config.yml文件
我们推送之后，毕竟还是别人的模版。但是你可以在此时你的本地git仓库找到这个文件，对

其进行部分修改。这样可以改变网页上模版留有的信息。因为每个模版的配置文件内容不

同，我这里就不做演示了。

以我自己的模版为例，里面有个_post文件，就是用来存放`.md`的博客的。这个应该很多模版

都会有，你可以自己找找看，或者看看模版作者留的说明。然后修改细节，你的个人博客就

搭建完成了。

