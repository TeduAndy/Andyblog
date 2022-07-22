---
title: hexo-部屬靜態頁面到-github
date: 2022-07-22 08:35:32
category: Blog-Hexo框架
---

## GitHub 產生站點專案

<br>




## hexo 專案 設置部分

#### <font color='e59911'>1. hexo 部屬前需安裝的套件</font>
```bash
npm install hexo-deployer-git --save
```

<br>

#### <font color='e59911'>2. 修改根目錄的_config.yml檔案</font>
```yml
# Deployment
## Docs: https://hexo.io/docs/one-command-deployment
deploy:
  type: "git" // 類別請寫 git
  repo: https://github.com/username/username.github.io.git // github專案位置
  branch: master  // 上傳到此專案的哪一個分支，通常都是 master 
```

<br>

#### <font color='e59911'>3. 輸入指令部屬上傳</font>

+ **每次部屬請進行三步驟**
```bash
hexo clean        // 清除之前建立的靜態檔案
hexo generate     // 建立靜態頁面
hexo deploy       // 部署至 GitHub
```