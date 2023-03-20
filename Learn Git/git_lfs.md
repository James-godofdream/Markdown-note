## 安装 Git LFS
##### 1. 有三种简单的方式来安装 Git LFS：

a. 用你最喜欢的软件包管理器来安装它。git-lfs 软件包在 Homebrew，MacPorts，dnf 和packagecloud中都是可用的；或者

b. 从项目网站下载并安装Git LFS；

c. 安装 Sourcetree，它是捆绑了 Git LFS 的一个免费的 Git GUI 客户端。

##### 2. 一旦安装好了 Git LFS，请运行 git lfs install 来初始化 Git LFS（如果你安装了 Sourcetree，可以跳过此步骤）：

$ git lfs install
Git LFS initialized.
你只需要运行 git lfs install 一次。为你的系统初始化后，当你克隆包含 Git LFS 内容的仓库时，Git LFS 将自动进行自我引导启用。

## 使用Git LFS
cd upload #进入名为upload的文件夹，提前将要上传的大文件放入该文件夹下
git init #创建本地仓库环境
git lfs install #安装大文件上传应用
git lfs track * #追踪要上传的大文件，*表示路径下的所有文件
git add .gitattributes #添加先上传的属性文件(要先上传属性文件，不然有可能失败)
git commit -m "pre" #添加属性文件上传的说明
git remote add origin https://github.com/Youpeng-Zhang/MOP.git #建立本地和Github仓库的链接
git push origin master #上传属性文件
git add * #添加要上传的大文件，*表示路径下的所有文件
git commit -m "Git LFS commit" #添加大文件上传的说明
git push origin master #上传大文件




## 创建一个新的 Git LFS 仓库
要创建一个新的支持 Git LFS 的仓库，你需要在创建仓库后运行 git lfs install：

\# initialize Git
$ mkdir Atlasteroids
$ cd Atlasteroids
$ git init
Initialized empty Git repository in /Users/tpettersen/Atlasteroids/.git/
\# initialize Git LFS
$ git lfs install
Updated pre-push hook.
Git LFS initialized.   

## Git LFS 其他命令
显示当前被 lfs 追踪的文件列表
git lfs ls-files 

查看现有的文件追踪模式
git lfs track 

取消 git lfs 对某文件的追踪
git lfs untrack "\*xx.a" 

查看当前 git lfs 版本
git lfs version 

取消 LFS 的全局配置
git lfs uninstall