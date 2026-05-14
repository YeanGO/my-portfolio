# JY Li Portfolio

個人作品集網站第一版，使用純 HTML、CSS、JavaScript 開發，可直接部署至 GitHub Pages。

## 目前作業階段

已完成：

- 首頁 Home Page 第一版
- 作品集 Projects 頁面基本框架
- 第一個完整作品區塊：`01｜360 度績效互評系統`
- 共用 Navbar 與手機版漢堡選單
- 暗色科技風視覺樣式
- 桌機、平板、手機基本 RWD

尚未完成：

- 學習歷程頁：`learning-journey.html`
- 研究方向頁：`research.html`
- 履歷頁：`resume.html`
- 作品集後續第二、第三個專案區塊
- 實際個人照片、專案影片與系統截圖素材

## Pages

- `index.html`：首頁
- `projects.html`：作品集頁，目前已完成 360 度績效互評系統作品區塊
- `learning-journey.html`：預留連結，尚未建立
- `research.html`：預留連結，尚未建立
- `resume.html`：預留連結，尚未建立

## Structure

```text
portfolio/
├── index.html
├── projects.html
├── css/
│   ├── style.css
│   ├── home.css
│   ├── projects.css
│   └── responsive.css
├── js/
│   └── main.js
├── assets/
│   └── images/
│       ├── profile-placeholder.svg
│       └── projects/
└── README.md
```

## CSS 分工

- `css/style.css`：全站基礎樣式、色彩變數、Navbar、按鈕
- `css/home.css`：首頁 Hero 與四大圓形入口
- `css/projects.css`：作品集頁與 360 度績效互評系統作品區塊
- `css/responsive.css`：共用 RWD 與首頁 RWD

## JavaScript

- `js/main.js`：手機版 Navbar 漢堡選單開合

## Placeholder 素材

個人照片目前使用：

```text
assets/images/profile-placeholder.svg
```

正式個人照片建議放置於：

```text
assets/images/profile.jpg
```

360 度績效互評系統目前預留：

```text
assets/images/projects/pa360-system-architecture.png
assets/images/projects/pa360-login.png
assets/images/projects/pa360-student-evaluation.png
assets/images/projects/pa360-teacher-evaluation.png
assets/images/projects/pa360-admin-analysis.png
```

其他待替換內容：

- GitHub Repository URL：目前在 `projects.html` 中為 `href="#"`
- YouTube Embed URL：目前在 `projects.html` 中 iframe `src` 尚未填入

## 本機預覽

若在 `portfolio` 資料夾啟動靜態伺服器，可使用：

```text
http://127.0.0.1:8000/index.html
http://127.0.0.1:8000/projects.html
```

## 下一步建議

1. 補上正式個人照片。
2. 補上 360 度績效互評系統的 GitHub Repository URL。
3. 補上 YouTube 系統操作展示影片 Embed URL。
4. 加入系統架構圖與四張代表性系統截圖。
5. 接續製作學習歷程、研究方向與履歷頁。
