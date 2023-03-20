## Git如何远程传送数据
git init
git add .
git commit -m "first commit"
git remote add origin https://...
git remote -v 查看连接情况
git remote rm origin 删除已连接
git config --global user.email "...@***.com"
git config --global user.name "************"
git push -u origin main
## Git上传大文件
git lfs install
git lfs track 目标文件/全部文件 *
git add .gitattributes
git commit -m "push pre file by lfs"
git remote add origin https://...
git push origin main
git add 目标文件/全部文件 *
git commit -m "push big file by lfs"
git push origin main
## 更新github文件
与上面操作类似

1.本地更新好博客内容
2.添加更新文件
git add  "新文件名称"
3.提交到缓存区域
git commit -m "update"  
4.从本地仓库或本地分支获取并集成(整合)
git pull origin master
5.如果过程中出现‘please enter a commit message…’,首先按下esc退出键然后输入 ：wq即可
6.push到远程master分支上
git push -u origin master
7.刷新页面就可以看见更新文件
————————————————
## 删除github文件
在github上只能删除仓库,却无法删除文件夹或文件, 所以只能通过命令来解决

首先进入你的main文件夹下, Git Bash Here ,打开命令窗口

$ git –help 帮助命令
$ git pull origin main 将远程仓库里面的项目拉下来
$ dir  查看有哪些文件夹
$ git rm −r –cached  target  删除target文件夹 
$ git commit -m ‘删除了target’ 
$ git commit -m '说明'提交到版本库中即可。  提交,添加操作说明 
$ git push -u origin main 将本次更改更新到github项目上去

操作完成.

注:本地项目中的target文件夹不收操作影响,删除的只是远程仓库中的target, 可放心删除

每次增加文件或删除文件，都要commit 然后直接 git push -u origin master，就可以同步到github上了

### 接下来，分享一下上传本地项目到Github的步骤：
1.在命令行中，输入“git init”，使Test文件夹加入git管理；
2.输入“git add .”（不要漏了“.”），将Test文件夹全部内容添加到git。
3.输入“git commit -m "first commit"”（“git commit -m "提交信息"”）
4.输入“git remote add origin https://github.com/DawenZeng/Test.git”，连接你的guthub仓库。

5.输入“git push -u origin master”，上传项目到Github。这里会要求输入Github的账号密码，按要求输入就可以。

由于新建的远程仓库是空的，所以要加上-u这个参数，等远程仓库里面有了内容之后，下次直接使用“git push origin master”就可以。

6.注意：如果你勾选了Initialize this repository with a README（就是创建仓库的时候自动给你创建一个README文件），那么到了第5步你将本地仓库内容推送到远程仓库的时候就会报一个failed to push some refs to https://github.com/DawenZeng/Test.git的错：

这是因为新创建的那个仓库里面的README文件不在本地仓库目录中，这时我们可以通过以下命令先将内容合并以下：

$ git pull --rebase origin master

再

$ git push origin master

第六步：README.md 里添加项目简介和图片的方法：

例如：我在我的 dotvim 文件夹下一个 screenshots 目录，在该目录里有一个 vim-screenshot.jpg 截图。那么添加链接的方式如下

 ![image](https://github.com/DawenZeng/dotvim/raw/master/screenshots/vim-screenshot.jpg)
或
 ![image](/dotvim/raw/master/screenshots/vim-screenshot.jpg)
———————