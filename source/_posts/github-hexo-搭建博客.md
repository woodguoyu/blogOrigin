---
title: github Hexo 搭建博客并使用 nexT主题 & 绑定域名
date: 2018-08-14 21:07:43
tags: [Hexo]
categories: 
- Hexo 
---
本篇适用于小白，你可以get到以下功能
---
> - 使用github & hexo 创建自己的博客
> - 更换 nexT 主题
> - 增加各样的功能（字数统计，阅读时间，分类，标签，站内搜索,阅读次数，头像，评论区 ，百度 google bing 站点收录 等等）
> - 绑定自己的域名
## github 篇
---
>在此假设你已经有了 [ <icon class='iconfont gy-github-fill'></icon> 前往 github 账号](https://github.com/) 

## github New repository //新建仓库
### 进入代码库创建页面：
![](http://pdm19dogd.bkt.clouddn.com/%E5%B1%8F%E5%B9%95%E5%BF%AB%E7%85%A7%202018-08-18%20%E4%B8%8B%E5%8D%889.45.20.png)
### 创建仓库名称，**仓库名为 xxxx.github.io **, “xxxxx” 一定要与自己的 github 账户一致！！！下图为例
![](http://pdm19dogd.bkt.clouddn.com/%E5%B1%8F%E5%B9%95%E5%BF%AB%E7%85%A7%202018-08-18%20%E4%B8%8B%E5%8D%8810.34.39.png)
创建完毕后页面自动跳转如下页面，此时访问 xxxx.github.io（你自己的主页），404。需要第三部操作，开启 GitHub Pages（[什么是GitHub Pages](https://help.github.com/articles/what-is-github-pages/) )）
![](http://pdm19dogd.bkt.clouddn.com/%E5%B1%8F%E5%B9%95%E5%BF%AB%E7%85%A7%202018-08-18%20%E4%B8%8B%E5%8D%8810.05.41.png)
### 点击 Settings,进入页面，下拉 找到 GitHub Pages ，会发现如下图所示，意思是你当当前的仓库内容为空，所以默认为 disabled 状态
![](http://pdm19dogd.bkt.clouddn.com/%E5%B1%8F%E5%B9%95%E5%BF%AB%E7%85%A7%202018-08-18%20%E4%B8%8B%E5%8D%8810.35.08.png)
为了证明下自己的站点可以打开，只需要增加一个 index.html 文件即可，方式多样，比如利用 Choose a theme,选择 github 提供的一个主题模板，会自动生成一些文件来让项目自动启动 GitHub Pages。
![](http://pdm19dogd.bkt.clouddn.com/%E5%B1%8F%E5%B9%95%E5%BF%AB%E7%85%A7%202018-08-18%20%E4%B8%8B%E5%8D%8810.35.23.png)
我默认选择了第一个，只是为了验证站点能否打开。这个随便，后面会被我们自己创建的 hexo 项目覆盖掉，提交后，再次访问 xxxx.github.com ,就能看到下面的界面，说明项目木问题
![](http://pdm19dogd.bkt.clouddn.com/%E5%B1%8F%E5%B9%95%E5%BF%AB%E7%85%A7%202018-08-18%20%E4%B8%8B%E5%8D%8810.37.11.png)

## 什么是 Hexo？

>Hexo 是一个快速、简洁且高效的博客框架。Hexo 使用 Markdown（或其他渲染引擎）解析文章，在几秒内，即可利用靓丽的主题生成静态网页。
## 安装 Hexo
<icon class='iconfont gy-tuding'></icon>[点我进入Hexo 手册](https://hexo.io/zh-cn/docs/)
>仔细阅读文档，严格安装文档操作
## 创建 **本地** 博客站点
>在此默认成功安装 Hexo

### 本地初始化项目
>hexo init  hexo  // hexo 是项目名称，这个随意 

 ![01](http://pdm19dogd.bkt.clouddn.com/%E5%B1%8F%E5%B9%95%E5%BF%AB%E7%85%A7%202018-08-17%20%E4%B8%8B%E5%8D%8811.01.47.png)
### 本地项目启动 // 预览
>hexo g  //g是generetor的缩写，生成博客<br>
>hexo s  //s是server的缩写，启动服务

项目成功启动后是酱紫的

 ![02](http://pdm19dogd.bkt.clouddn.com/%E5%B1%8F%E5%B9%95%E5%BF%AB%E7%85%A7%202018-08-17%20%E4%B8%8B%E5%8D%8811.14.50.png)
 默认情况下 启动的是 localhost:4000     4000端口
 
 若端口被占用，会出现下图所示。 可使用 自定义端口命令
 >hexo s -p 5500

 ![01](http://pdm19dogd.bkt.clouddn.com/%E5%B1%8F%E5%B9%95%E5%BF%AB%E7%85%A7%202018-08-17%20%E4%B8%8B%E5%8D%8811.10.54.png)

打开浏览器 输入 http://localhost:xxxx/  
### 安装并配置 nexT 主题
1.  在终端窗口下，定位到 Hexo 站点目录下。使用 Git checkout 代码：
```
git clone https://github.com/iissnan/hexo-theme-next themes/next
```
2. **启用主题** ：打开 站点配置文件 _config.yml（nexT 主题配置也有 _config.yml 配置文件，切忌弄混乱）， 找到 theme 字段，并将其值更改为 next。hexo s 启动服务（上有所述），预览。
```
theme: next
```
3. 主题配置

[nexT 主题配置文档](http://theme-next.iissnan.com/getting-started.html)

建议仔细阅读文档，官方文档叙述很奈斯，enjoy

4. 站点配置文件 _config.yml，安装自己的站点配置 repo 字段
```json
deploy:
  type: git
  repo: https://github.com/woodguoyu/woodguoyu.github.io.git
  branch: master
```
5. 发布至 github，执行以下命令行
``` 
1. hexo clean
2. hexo g (generate)
3. hexo d (deploy)
```
发布完毕，打开自己的 xxxx.github.io ，查看。可能不能马上同步，等几分钟也是可以的。



Enjoy One Min 

 ![01](http://pdm19dogd.bkt.clouddn.com/818D4A76FDD69E3C5B08EECAF605232D.gif)

one min latter

 ![](http://pdm19dogd.bkt.clouddn.com/E9E57D902747D46CEBD4A0877139C676)

### 添加自己的博客文章
1. 在终端窗口下，定位到 Hexo 站点目录下
```
hexo new post '文章名称'
```
生成文档在  **博客/source/_post/文章名称.md**，hexo 会自动编译markdown 文件

2. 编辑文档
3. 重新发布
``` 
1. hexo clean
2. hexo g (generate)
3. hexo d (deploy)
```

整个过程走下来，尤其是配置 nexT 主题各个功能。问题倒是不少，遇到的纸老虎后续会添加进去，如若看到，尽可能少走弯路。

 ![](http://pdm19dogd.bkt.clouddn.com/F1310DB9A6960654E4282F4C2A786AE6)













>待续

<link rel="stylesheet" href="https://at.alicdn.com/t/font_798158_wn4udd6bx9.css">