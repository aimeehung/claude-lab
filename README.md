# Aimee Graphic Design — Landing Page

Aimee 平面設計工作室的個人作品集形象網站，以單一頁面介紹設計服務、精選作品與聯繫方式。

## 網站功能

- **導覽列（Nav）**：固定於頁面頂端（sticky），帶有毛玻璃效果，可快速跳至「作品」、「合作流程」與「與我聯繫」。
- **主視覺（Hero）**：品牌標語「讓品牌被看見，也被記住。」、個人簡介、行動按鈕，以及經驗／專案數／合作品牌等數據。
- **精選作品（Selected Work）**：三張作品卡片，涵蓋品牌識別、編輯排版與包裝設計。
- **聯繫區塊（Contact）**：邀請潛在客戶聯絡合作。
- **動態效果**：頁面載入淡入動畫，以及捲動到區塊時的淡入效果（IntersectionObserver）。
- **RWD 響應式設計**：
  - 960px 以下：作品改為兩欄排列。
  - 680px 以下（手機版）：作品改為單欄、縮小標題字級、調整間距、隱藏次要導覽連結，並確保觸控目標至少 44px 高、頁面不會出現水平捲動。
- **無障礙**：支援 `prefers-reduced-motion`，偏好減少動態的使用者會關閉動畫。

## 使用技術

- **HTML5**：語意化標籤（`nav`、`section`、`footer` 等）。
- **CSS3**：CSS 變數（Custom Properties）、Flexbox、CSS Grid、`@media` 媒體查詢、`@keyframes` 動畫、`backdrop-filter`、漸層背景。
- **Google Fonts**：Inter、Noto Sans TC、Cormorant Garamond。
- 少量原生 JavaScript 用於捲動淡入效果（無任何框架或建置工具）。

## 如何開啟

本專案為純靜態網頁，不需安裝任何套件：

1. 下載或 clone 此專案：
   ```bash
   git clone https://github.com/aimeehung/claude-lab.git
   ```
2. 進入資料夾，直接用瀏覽器開啟 `index.html`：
   - **macOS**：在 Finder 中雙擊 `index.html`，或於終端機執行 `open index.html`
   - **Windows**：在檔案總管中雙擊 `index.html`，或執行 `start index.html`
   - 也可以將 `index.html` 直接拖曳到 Chrome、Safari、Edge 或 Firefox 視窗中。
3. 想預覽手機版效果，可在瀏覽器開啟開發者工具（Chrome：`Cmd/Ctrl + Shift + I`），切換至裝置模擬模式（`Cmd/Ctrl + Shift + M`）。

> 註：字體由 Google Fonts 載入，需連網才能顯示完整字型。

## 檔案結構

```
claude-lab/
├── index.html   # Landing Page（HTML + 內嵌 CSS）
├── note.txt     # 筆記
└── README.md    # 專案說明
```
