---
title: 在Github Pages上部署Jekyll+Tailwindcss的模版
lang: zh
permalink: /
---

> Github Pages现在已经[默认使用Actions进行部署](https://github.blog/2022-08-10-github-pages-now-uses-actions-by-default/)，因此理论上任何静态网站框架都可以使用Actions进行部署，而不再需要像以前那样部署到新的分支。当然，部署到分支的方法还是可以使用的。

本项目是基于Jekyll+Tailwindcss如何在Github Pages上进行部署的模版，分别可以使用Actions部署或传统分支部署的方式。

## 前提

- 你已经使用Jekyll+Tailwindcss在本地创建了自己的网站
- 这个网站在本地运行正常
- 你的环境和下方的环境相似
- 你已经有一个Github帐号

## 环境

- Jekyll v4.3.2
- Tailwindcss v3.2.7
- Node.js v18.14
- ruby v3.1.2

*上述版本`xxx.yyy.zzz`中，如果`xxx`是一样的，理论上不会有任何问题。*

## 发布到Github Pages

下列方式二选一，当你再次向你的主分支推送后，将自动编译和部署你的网站到Github Pages。

### 使用Actions进行部署

第一步：将[gh-pages-with-actions.yml](https://github.com/guox/jekyll-tailwind-starter/blob/main/.github/workflows/gh-pages-with-actions.yml)复制到你的项目`/.github/workflows/`目录下。

第二步：设置Github Pages Source为**Github Actions**

![Github Pages Source: Actions](/assets/images/ghpages-source-action.png)

### 使用部署到分支

第一步：将[gh-pages-from-branch.yml](https://github.com/guox/jekyll-tailwind-starter/blob/main/.github/workflows/gh-pages-from-branch.yml)复制到你的项目`/.github/workflows/`目录下。

第二步：设置Github Pages Source为**Deploy from a branch**，分支选择**gh-pages**

![Github Pages Source: from a branch](/assets/images/ghpages-source-branch.png)

*你不需要提前创建gh-pages分支，当你推送`gh-pages-from-branch.yml`到Github仓库后，会自动创建gh-pages分支。*

## 源码和demo

<https://github.com/guox/jekyll-tailwind-starter>

## 许可

MIT




