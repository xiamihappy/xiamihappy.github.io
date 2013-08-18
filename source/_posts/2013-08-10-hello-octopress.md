---
layout: post
title: "Hello Octopress"
date: 2013-08-10 17:48
comments: true
categories: octopress
---
### 安装环境  
	rvm install 1.9.3
	git clone git://github.com/imathis/octopress.git octopress
	cd octopress
	gem install bundle
	`rvmsudo` bundle install
	rake install  
### 本地预览
http://localhost:4000

	rake preview
	
### 部署到github

	rake setup_github_pages
    # 粘贴 刚才新建的 仓库地址：
    git@github.com:username/username.github.com.git
    rake generate
    rake deploy
##### 合并操作

	rake gen_deploy
	
##### 将源代码发布到source分支

	git add .
	git commit -m ""
	git push origin source
	or git checkout -b source
	
### 基本配置

修改 _config.yml中的相关配置，注意格式 配置项:＋空格＋参数，空格一定不能少，否则会报错。[^1]
[^1]: http://imwuyu.me/talk-about/configuring-octopress.html/

##### 自动打开文件/浏览器

编辑Rakefile

### 备注

* 在post文件中使用categories: [Ruby,Octopress]的形式为文章添加多个分类目录。
* `zshrc`  运行[ ]会有问题

```
alias rake="noglob rake"
rake "new_post[hello world]"
```


