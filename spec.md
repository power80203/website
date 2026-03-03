個人品牌入口網站技術規格書 (Personal Brand Site SPEC)
一、 專案願景 (Project Vision)

    定位： 建立一個具備「機器可理解性 (Machine-Readable)」的個人專業入口，將技術作品與影響力資產化。

    核心理念： Medium 是平台，GitHub 是作品，個人網站是**「數位實體 (Digital Entity)」**。

二、 技術架構 (Technical Stack)
組件	建議方案	備註
SSG 引擎	Hugo	追求極速生成與乾淨的 HTML 結構。
部署環境	GitHub Pages	與 CI/CD 流程高度整合，支持 Action 自動部署。
DNS / 安全	Cloudflare	提供 SSL、網域信箱與邊緣運算加速。
數據分析	GA4	建立回饋機制，追蹤「技術關鍵字」轉化率。
互動層	Tally.so / Calendly	處理聯繫表單與預約系統。
三、 視覺與色彩計劃 (Visual & Color Palette)

採用 「Deep Data Stream (深邃數據流)」 配色，模擬 IDE 開發環境，強調資料工程師的專業嚴謹。

    核心色彩 (CSS Variables):

        背景 (--bg): #0D1117 (GitHub Dark) — 營造專注感。

        主色 (--primary): #58A6FF (數據青) — 用於連結、導航與技術標籤。

        強調色 (--accent): #D29922 (警告金) — 用於 Call to Action (CTA)，如「預約諮詢」。

        文字 (--text): #C9D1D9 (珍珠白) / #8B949E (霧面灰)。

    視覺風格 (UI Style):

        排版： 採用等寬字體 (Monospace) 處理技術關鍵字。

        結構： 極簡邊框 (#30363D)，避免多餘的陰影與裝飾，強調「數據結構美感」。

四、 核心功能規格 (Core Functional SPEC)
1. 語義化 SEO (Semantic SEO)

    JSON-LD Person Schema: 在所有頁面注入結構化資料。

        需定義 jobTitle: Data Team Lead。

        需定義 knowsAbout: Data Engineering, ETL, Apache Airflow, Python, SQL Server。

        需連結 sameAs: 你的 Medium、GitHub、LinkedIn 帳號。

    技術關鍵字對齊： Slug (URL) 與文章標題需嚴格對齊語義（如：/posts/airflow-etl-optimization）。

2. 資產整合 (Asset Integration)

    GitHub Repository Showcase: 透過 GitHub API 或靜態卡片展示核心開源項目（如 core-library 或 workout-app）。

    Medium Sync: 建立一個精選文章索引頁，將流量導向 Medium，但將「SEO 權重」留在個人網域。

3. 轉化路徑 (Conversion Path)

    聯繫表單： 整合專業網域信箱 (e.g., contact@datafox.tw)。

    預約系統： 在「關於我」或頁尾嵌入 Calendly，直接開啟諮詢窗口。