---
layout: post
title:  "基于M1的CocoaPods安装"
date:   2022-10-27 12:00:00 +0800
categories: cocoapods
---
1、打开App Store 安装Xcode

2、打开“访达”，左侧选择“应用程序”，打开“实用工具”，选中“终端”，右键选择“显示简介”，勾选“使用Rosetta打开”

3、更换源：

```
gem sources -l #查看源

gem sources --remove https://rubygems.org/ #删除源

gem sources --add https://gems.ruby-china.com/ #添加源
```
4、安装rvm 

```
rvm -v #查看rvm版本

curl -L get.rvm.io | bash -s stable

source ~/.bashrc

source ~/.bash_profile
```
5、安装homebrew 和 Command Line Tools

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
6、升级ruby

```
rvm list known #列出可安装版本

rvm install 3.0.0 #安装最新版本

rvm use 3.0.0 --default #设置默认版本
```
7、安装cocoapods

```
sudo gem install -n /usr/local/bin cocoapods
```
