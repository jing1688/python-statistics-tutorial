# Python 統計學教室

一個可直接部署到 GitHub Pages 的 Python 統計學教學網站骨架。

## 網站內容

- 課程首頁
- 13 個章節頁面
- 每頁共用章節導覽
- 每頁自動產生「本頁目錄」
- 手機版側邊選單
- 上一章／下一章切換
- 預留觀念、程式碼、範例、練習題與重點整理區塊

## 專案結構

```text
python-statistics-tutorial/
├─ index.html
├─ .nojekyll
├─ README.md
├─ assets/
│  ├─ css/
│  │  └─ style.css
│  └─ js/
│     └─ site.js
└─ chapters/
   ├─ ch01.html
   ├─ ch02.html
   ├─ ...
   └─ ch13.html
```

## 本機預覽

直接開啟 `index.html` 即可。

也可以在專案資料夾執行：

```bash
python -m http.server 8000
```

再開啟瀏覽器進入：

```text
http://localhost:8000
```

## 部署到 GitHub Pages

1. 建立新的 GitHub repository。
2. 將本專案所有檔案上傳到 repository 根目錄。
3. 進入 `Settings` → `Pages`。
4. 在 `Build and deployment` 將 Source 選為 `Deploy from a branch`。
5. Branch 選擇 `main`，資料夾選擇 `/ (root)`。
6. 儲存後等待 GitHub Pages 完成部署。

## 編輯教材

每章教材位於 `chapters/chXX.html`。

網站章節名稱與導覽列設定位於：

```text
assets/js/site.js
```

共用外觀設定位於：

```text
assets/css/style.css
```
