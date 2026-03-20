---
title: "為Hugo網頁 增加favicon"
date: 2025-06-27T15:30:00+08:00
draft: false

# post thumb
image: "images/post/post-3.jpgx"

# meta description
description: "favicon 如何修改與增加"

# taxonomies
categories:
  - "Github網站筆記"
tags:
  - "Photos"

# post type
type: "post"
---
favicon指的是Favorites Icon(我的最愛圖示)。  
可以顯示在瀏覽器我的最愛的小圖示，也是顯示在瀏覽器分頁的小圖示 
目前使用的是 Liva Hugo 的主題，  
新版本(2025年6月)的設定擺在layouts/partials/head.html 裡面  

設定是
![image](images/post/faviconpage.png)

這邊要注意的是，我試了很久，png檔案不吃，帶png檔會顯示不出來，一定要使用ico檔。  
去找了一個Github圖，再轉成.ico檔後終於可以正常顯示。  
我這邊設定檔名favicon2.ico要擺進static/images/

效果如下
![image](images/post/faviconpage2.png)

![image](images/post/faviconpage3.png)

分頁上的亦同
