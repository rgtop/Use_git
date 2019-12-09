# git的相关操作

## 在本地建立好文件之后用命令将添加到版本库
```
git add .
git commit -m "我的提交"
```
git add . 是将所有的文件都添加到版本库 
git add -file.txt 是将file.txt文件添加
git commit -m "我的提交" 是提交到版本库  -m或者--message 是信息 " "双引号中的的内容是提交的备注

## 克隆仓库
```
git clone git_cbbgs git1
```
## 拉取githup上的项目
当本地没有相应的项目文件夹时，用clone
```
git clone https://github.com/cbbgs/tcs.git

```
有相应的文件是用pull
```
git pull https://github.com/cbbgs/tcs.git
```

## 上传到github
注意，上传到githup时一定要是pull或者clone下来的项目，再上传回去才可以
```
git push https://github.com/cbbgs/tcs.git
```

