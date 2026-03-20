---
title: "為Hugo網頁加入Disqus留言板"
date: 2025-06-26T14:30:00+08:00
draft: false

# post thumb
image: "images/post/post-3.jpgx"

# meta description
description: "Liva Hugo 主題簡單加入留言功能"

# taxonomies
categories:
  - "Github網站筆記"
tags:
  - "Photos"

# post type
type: "post"
---
參考Hahow課程，Github免費架站術！輕鬆打造個人品牌，第四章單元二。

https://avnet.business.hahow.in/classroom/VL13FwO_LVgCkcWsKTPsSA

步驟一：

先去Disqus官網 https://disqus.com/

申請帳號，去開一個新的Site

https://disqus.com/admin/create/

![image](images/post/d1.png)

步驟二：

點選 I don’t see my platform listed, install manually …

拉到最下面，點選 configure

![image](images/post/d2.png)

![image](images/post/d3.png)

Website URL 填入自己的網站

Language 選 Chinese (Taiwan) 然後 Next

![image](images/post/d4.png)

我選 Balanced，然後 Complete Setup

![image](images/post/d5.png)

步驟三：

到程式碼裡加Disqus設定

到 EXAMPLESITE/config/_default/hugo.toml

填入Disqus short name

可以在Disqus，Sites -> Edit Settings 裡面找到

![image](images/post/d6.png)

![image](images/post/d7.png)

步驟四：

檢查文章設定有無Disqus設定

到 Themes/layouts/_default/single.html

![image](images/post/d8.png)

我選的Liva Hugo 主題default有內建，加入Shortname 即可生效。

生效後要將網頁上傳後才能看到，local 本地端僅有Disqus描述，看不到留言板

![image](images/post/d9.png)
