# vue-training

This template should help get you started developing with Vue 3 in Vite.

## Recommended IDE Setup

[VSCode](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur) + [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin).

## Customize configuration

See [Vite Configuration Reference](https://vitejs.dev/config/).

## Project Setup
## 全局安裝Vue CLI，Vue CLI 是 Vue.js 官方提供的命令行工具
```sh
npm install
npm install --global @vue/cli
```

### Compile and Hot-Reload for Development
### 用本地伺服器來即時加載網頁，用於編譯
```sh
npm run dev
```

### Compile and Minify for Production
### 用於將源代碼打包、編譯、優化
```sh
npm run build
```

### Github push
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/wl02264122/Muramasa.github.io.git
git push -u origin main

gh-pages

### 建立並切換到 gh-pages 分支：
git checkout -b gh-pages
### 將 dist 目錄的內容添加到暫存區
git add dist/
### 提交變更到 gh-pages 分支
git commit -m "Add dist for GitHub Pages"
### 推送到遠端的 gh-pages 分支
git push origin gh-pages

### 如果你之前已經有了 gh-pages 分支，你可以使用以下命令直接切換到 gh-pages 分支，然後再進行上述的 git add、git commit、git push 步驟：

git checkout gh-pages

### 簡化
### 1.在主目錄下執行 npm run build。
### 2.執行以下 Git 指令：
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/wl02264122/Muramasa.github.io.git
git push -u origin main

### 接下來，直接切換到 gh-pages 分支，將 dist 目錄的內容添加到暫存區，並推送到 GitHub： 
git checkout -b gh-pages
git add dist/
git commit -m "Add dist for GitHub Pages"
git push origin gh-pages