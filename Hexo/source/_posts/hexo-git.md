---
title: hexo-git
date: 2016-06-03 14:54:58
categories: 2016
tags: [2016, git, hexo]   #yaml语法,用逗号+空白区隔 sep=', '
---
### git clone -b source 分支备份.md源文件
```scala
git clone -b source *.io hexo-github5

cd Hexo/    // ***/Hexo (source) // 必须在Hexo目录下，安装hexo包
npm install -g hexo-cli  // 安装hexo
npm install              //安装依赖包--需要package.json文件
npm install hexo-server --save
npm install hexo-deployer-git   // 用git部署插件
npm install hexo-generator-feed --save //RSS插件
// no hexo init after first use
hexo -v    //hexo: 3.2.0

hexo g
hexo server -i 127.0.0.1 -p 5000
hexo d
history > 2016-0602-log.txt

git branch -av //显示分支
gitk --all&    //GUI显示
git push origin source:source //备份源文件
```
#### Hexo/themes/modernist/ 主题目录
```java
写作 .md
配置 Hexo/_config.yml
```