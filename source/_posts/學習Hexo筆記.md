---
title: 學習Hexo筆記
date: 2024-05-29 14:42:52
tags: 
    - Hexo
    - blog
    - 架站
    - markdown
    - gitHub
---

安裝Hexo
---
1. 到Hexo官網文件區域 [連結](https://hexo.io/zh-tw/docs/)
2. 安裝前需要的軟體：
    - Node.js
    - Git
3. 透過終端機輸入程式碼安裝Hexo：
    ```
    npm install -g hexo-cli
    ```
4. 建立一個新資料夾，讓Hexo以此資料夾建立網站
    - hexo init '資料夾路徑'

5. 常用的指令：
    - **hexo new 文章名稱**
        *新增一篇文章*
    - **hexo server**
        *啟動伺服器*
    - **hexo clean**
        *清除快取*
    - **hexo generate**
        *生成靜態檔案*     
    - **hexo deploy**
        *部署*
        
        **重點**
        *通常在完成每次修改後，會依序輸入 clean -> generate -> deploy 三行指令，避免更新不完全：*
        ```
        $ hexo cl    // 清除之前建立的靜態檔案
        $ hexo g     // 建立靜態頁面
        $ hexo d     // 部署至 GitHub
        ```
    - **hexo new page about**
        *在source新增子資料夾，名稱為about*

6. 修改主題：
    - **theme**
        *這裡會放主題用的資料夾*
        1. 複製主題安裝連結(Install via git:)，新增landscape主題資料夾(預設為landscape)
        [樣式連結](https://github.com/hexojs/hexo-theme-landscape)
        ```
        git clone --depth 1 https://github.com/hexojs/hexo-theme-landscape themes/landscape
        ```
        2. 此時themes會新增一個landscape資料夾，尋找_config.yml，即可修改內容。
