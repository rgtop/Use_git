# 相对完整的git操作

## 1、下载git 
去官网下载
## 2、安装git
差不多一直next
## 3、注册github账号
## 4、创建git仓库
在自己的硬盘下创建一个文件夹，我创建的是gitworkspace。
windows操作系统下进入gitworkspace,这个gitworkspace,我们可以将很多git版本库都放在里面。
点击鼠标右键 选择git bash here.第一次打开git bash 是需要输入用户名和邮箱
```
git config --global user.name "ccbgs"
git config --global user.email "cbbgs_cb@foxmail.com"
```
开始输入指令创建git版本库.创建的git_cbbgs用于git版本库
```
git init git_cbbgs
```
进入创建的版本库
```
cd git_cbbgs
```
## 将更新添加到版本库
在windows这个目录下任意创建一个文件a.txt（代替我们以后的项目文件）
```
git add a.txt
git commit -m "add a.txt"
```
git add . 这个点表示提交所有


# 上面的都是基础操作
我们在创建gitworkspace的基础上，我们将github上的项目拉取到自己的本地
## git拉取github仓库
我们准备拉取这个网址的仓库https://github.com/cbbgs/tcs
由于我们的文件夹下没有tcs这个版本库，故我们拉取时使用clone命令。
我们在具体的拉取时在网址的最后加入.git 最后可以添加一个分支，拉取分支。
```
git clone https://github.com/cbbgs/tcs.git
```
## 创建分支
我们将github的版本库进行更新，我可以创建一个新的文件夹，但是这个文件夹是一个分支。我文件夹就叫html。创建文件夹在这里先不要创建
### 1.创建分支
我们创建一个分支叫branch1
```
git branch branch1
```
### 2.切换到我们创建的分支
```
Git checkout branch1
```
### 3.创建文件夹 html
我们在这个创建html文件夹来模仿项目的一个模块文件夹。然后我们在html文件夹下创建一个A.java文件（模仿项目文件）.这一步就是在Windows磁盘下完成创建的下。

### 4.将我们更新的东西添加和提交到版本库
```
git add html
git commit -m "add html"
```
### 5.将我们更新的版本库更新到github
我们将这个更新的仓库上传到github时要注意用我们创建的分支上传 branch1。上传时会提示输入账号和密码
```
git push https://github.com/cbbgs/tcs.git branch1
```

到这里我们就模仿项目组成员利用git和github对项目进行分工更新








