# JY Li Portfolio

個人作品集網站，使用純 HTML、CSS、JavaScript 製作多頁式靜態網站，預計部署至 GitHub Pages。整體視覺定位為暗色科技風：深藍黑背景、白色與灰白文字、青藍色發光強調，適合作為履歷延伸作品集。

## 目前網站架構

| 頁面 | 定位 | 狀態 |
|---|---|---|
| `index.html` | 首頁，包含固定 Navbar、左圖右文 Hero、四大圓形入口 | 已完成第一版 |
| `projects.html` | 作品集總覽頁，提供作品入口與精簡專案介紹 | 已重製為總覽頁 |
| `project-pa360.html` | 作品一「360 度績效互評系統」獨立作品詳細頁 | 已完成第一版 |
| `project-pa360-cloud.html` | 作品二「PA360 雲端部署實作：AWS EC2 × Docker」獨立作品詳細頁 | 待製作 |
| `learning-journey.html` | 學習歷程頁 | 待製作 |
| `research.html` | 研究方向頁 | 待製作 |
| `resume.html` | 履歷頁 | 待製作 |

## 本階段重要架構決策

1. 首頁「作品集」入口不直接進入作品一，而是導向 `projects.html`。
2. `projects.html` 不再放作品一的完整長篇介紹，已改為「作品集總覽頁」。
3. `projects.html` 新版結構為：頁面標題區、三個圓形作品入口、三張專案總覽卡片、Footer。
4. 完整作品內容改放獨立詳細頁：
   - 作品一：`project-pa360.html`
   - 作品二：`project-pa360-cloud.html`
5. `project-pa360.html` 已依 `360_度績效互評系統作品詳細頁規格_v_1.md` 定義為獨立作品詳細頁。
6. 作品詳細頁上方需有「← 返回作品集總覽」連結，且 Navbar 的「作品集」需維持 Active 狀態。

## 目前相關規格文件

以下規格文件位於專案根目錄 `C:\Users\may\Documents\New project`：

- `個人作品集網站首頁規格書_v_1.md`：定義首頁架構、Navbar、Hero、四大圓形入口與暗色科技風視覺方向。
- `作品集總覽頁規格書_v_1.md`：定義 `projects.html` 作為作品集總覽頁，包含三個圓形作品入口與三張精簡作品卡片。
- `360_度績效互評系統作品詳細頁規格_v_1.md`：定義 `project-pa360.html` 作為作品一完整詳細頁，包含專案簡介、GitHub、YouTube、架構圖、截圖、角色流程、功能、技術與學習收穫。

## 目前完成狀態

已完成：

- 首頁 `index.html` 第一版。
- 作品集總覽頁 `projects.html` 重製完成。
- 作品一詳細頁 `project-pa360.html` 第一版完成。
- 共用 Navbar 與手機版漢堡選單。
- 暗色科技風共用視覺樣式。
- 桌機、平板、手機基本 RWD。
- `projects.html` 已連到：
  - 作品一：`project-pa360.html`
  - 作品二：`project-pa360-cloud.html`
- 作品三已在 `projects.html` 顯示為「規劃中」與 disabled 狀態。

待製作 / 待確認：

- `project-pa360-cloud.html` 尚未建立。
- 作品二「PA360 雲端部署實作：AWS EC2 × Docker」詳細頁規格書尚待撰寫。
- `learning-journey.html` 尚未建立。
- `research.html` 尚未建立。
- `resume.html` 尚未建立。
- 第三作品尚未確認主題與詳細頁規格。

## Placeholder 與待替換素材

個人照片目前使用：

```text
assets/images/profile-placeholder.svg
```

正式個人照片建議放置於：

```text
assets/images/profile.jpg
```

作品一 `project-pa360.html` 目前預留素材：

```text
assets/images/projects/pa360-system-architecture.png
assets/images/projects/pa360-login.png
assets/images/projects/pa360-student-evaluation.png
assets/images/projects/pa360-teacher-evaluation.png
assets/images/projects/pa360-admin-analysis.png
```

其他待替換內容：

- 作品一 GitHub Repository URL：目前在 `project-pa360.html` 中為 `href="#"`。
- 作品一 YouTube Embed URL：目前在 `project-pa360.html` 中 iframe `src=""`。
- 作品二詳細頁連結已在 `projects.html` 保留為 `project-pa360-cloud.html`，但檔案尚未建立。

## 檔案結構

```text
portfolio/
├── index.html
├── projects.html
├── project-pa360.html
├── README.md
├── css/
│   ├── style.css
│   ├── home.css
│   ├── projects.css
│   ├── project-detail.css
│   └── responsive.css
├── js/
│   └── main.js
└── assets/
    └── images/
        ├── profile-placeholder.svg
        └── projects/
```

## CSS 分工

- `css/style.css`：全站基礎樣式、色彩變數、Navbar、按鈕。
- `css/home.css`：首頁 Hero 與首頁四大圓形入口。
- `css/projects.css`：作品集總覽頁，以及部分作品展示共用樣式。
- `css/project-detail.css`：獨立作品詳細頁補充樣式，例如返回總覽連結、詳細頁標題與收束區塊。
- `css/responsive.css`：共用 RWD 與首頁 RWD。

## JavaScript

- `js/main.js`：手機版 Navbar 漢堡選單開合。

## 本機預覽

若在 `portfolio` 資料夾啟動靜態伺服器，可使用：

```text
http://127.0.0.1:8000/index.html
http://127.0.0.1:8000/projects.html
http://127.0.0.1:8000/project-pa360.html
```

## 下一步建議工作順序

1. 依據 `作品集總覽頁規格書_v_1.md` 檢查 `projects.html`，確認總覽頁結構、文案與 RWD 是否符合規格。
2. 檢查 `projects.html` 是否正確連到 `project-pa360.html`，並確認作品三保持規劃中狀態。
3. 規劃並撰寫作品二「PA360 雲端部署實作：AWS EC2 × Docker」詳細頁規格書。
4. 依作品二規格建立 `project-pa360-cloud.html`。
5. 補齊作品一圖片、系統架構圖、YouTube 展示影片與 GitHub 連結。
6. 接續製作 `learning-journey.html`、`research.html`、`resume.html`。
