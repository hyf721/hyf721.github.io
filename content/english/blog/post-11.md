---
title: "在 Windows 上安裝 Gemini CLI"
date: 2025-06-27T17:30:00+08:00
draft: false

# post thumb
image: "images/post/post-3.jpgx"

# meta description
description: "Gemini CLI"

# taxonomies
categories:
  - "無聊當有趣"
tags:
  - "Photos"

# post type
type: "post"
---
Step1：安裝 Node.js (和 npm)

Gemini CLI 是基於 Node.js 運行的，並且會透過 npm（Node Package Manager）來安裝。  
先安裝 Node.js。下載 Node.js 安裝程式：  
前往 Node.js 官方網站：https://nodejs.org/en/download/  
下載 LTS (長期支援) 版本，這通常是最穩定且推薦的版本。點擊 Windows Installer (.msi) 下方對應你系統位元（通常是 64-bit）的連結。  

![image](images/post/gemini1.png)

Step2：安裝 Gemini CLI

已經有了 Node.js 和 npm，可以輕鬆安裝 Gemini CLI 了。  
打開命令提示字元或 PowerShell。  
輸入安裝指令：  
> npm install -g @google/gemini-cli

步驟 3：運行 Gemini CLI 並登入  
輸入啟動指令：  
>gemini  

即可使用
圖示如下，跟網頁版一樣直接問吧

![image](images/post/gemini2.png)

/help 有熱鍵和  
Control-C 二次或 /quit 可離開  

![image](images/post/gemini3.png)