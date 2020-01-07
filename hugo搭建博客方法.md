# 如何用hugo搭建个人博客(已安装hugo为前提)
## step1
进入hugo官网，点击quickstart
## step2
用Cmder打开一个空目录，输入代码

```
hugo new site usersname.github.io
```

## step3
用code打开usersname.github.io，新建终端
输入代码
```
git init
git submodule add https://github.com/budparr/gohugo-theme-ananke.git themes/ananke
```

## step4
输入代码
```
hugo new posts/第一篇博客.md
```
进入VScode，在第一篇博客里输入你想写的东西，记得
```
darft:ture
```
改为
```
draft:false
```

## step5
在vscode里的 第一篇博客 的终端里输入代码
```
hugo server -D
```
在最后一行的http链接可以访问刚刚搭建的博客，查看是否有误

## step6
vscode终端里输入代码
```
hugo -D
```
生成public目录

## step7
接下来就要把博客上传到网上，在目录下创建.gitignore,添加/public/
然后在终端里输入代码
```
cd public
git init
git add .
git commit -m 第一次部署博客
```
## step8 
在GitHub新建repo，命名usersname.github.io
然后
```
git remote origin git@xxxx.github.io
git push -u master
```
OK，已经上传上GitHub了

## step9
进入setting，找到GitHub page，在custom domain输入自己的域名
save

# End






