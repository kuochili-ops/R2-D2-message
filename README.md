𓃥 白六 R2-D2 全息廣播 (R2-D2 Holographic Broadcast)
一款基於 WebGL (Three.js) 開發的 3D 星際大戰 R2-D2 全息動態廣播網頁應用程式。提供高質感的立體全息投影視覺效果、自動動態字級排版、流暢的登場動畫與一鍵自動錄影導出功能。
🔗 線上展示 App URL：https://kuochili-ops.github.io/R2-D2-message/
✨ 核心特色與功能
 * 🎬 經典登場動態動畫
   * R2-D2 後傾伸出第三隻腳滑行進場 ➔ 中央減速停靠 ➔ 收回第三隻腳恢復直立 ➔ 轉正面向螢幕並開啟全息投影。
 * 📐 動態全息投影與對齊
   * 動態字級適應：依據文字長度自動調整字體大小與 Canvas 解析度（字少字大、字多字小）。
   * 自動計算與防切字：根據文字實際測量寬高比例自動生成 3D 全息平面與光錐幾何，保證文字不被裁切。
   * 底邊無縫貼合：投影光錐三角形底邊左右端點嚴絲合縫貼合文字兩端。
 * 🎨 雙模式與色彩自訂
   * 支援多行文字自動輪播（每一行 3 秒平滑切換）。
   * 提供天空藍、紫羅蘭、翡翠綠、琥珀黃等四種光錐全息配色切換。
 * 🎥 一鍵自動自動化錄影
   * 點擊錄影後自動重啟進場動畫，並完整輪播一遍輸入的所有訊息，播畢後自動結束並匯出 .webm 高畫質影片檔。
 * 📱 行動端與響應式優化
   * 支援 UI 面板點擊外部（click / touchstart）自動收合。
   * 控制工具列置底，提供無遮擋的最佳視覺視角。
🛠️ 技術棧 (Tech Stack)
 * 前端框架：HTML5, CSS3, JavaScript (ES6 Modules)
 * 3D 引擎：Three.js (WebGL)
 * 模型載入：GLTFLoader
 * 鏡頭控制：OrbitControls
 * 媒體錄製：HTML5 MediaRecorder API
📦 本地開發與部署 (Local Setup)
 * 複製專案庫
   git clone https://github.com/kuochili-ops/R2-D2-message.git
cd R2-D2-message

 * 放置 3D 模型檔案
   請確保根目錄下包含 R2-D2 的 GLTF/GLB 模型檔案：
   * ./r2-d2_animated.glb
 * 啟動本地伺服器
   由於 Three.js 載入外部 GLB 模型與 ES Modules 需要 CORS 環境，請使用本地 HTTP 伺服器開啟（例如 VS Code 的 Live Server 或 Python 內建伺服器）：
   python3 -m http.server 8000

   瀏覽器造訪 http://localhost:8000 即可預覽。
📄 著作權與模型致謝 (Attribution & License)
本專案之 3D 模型資源來自 Sketchfab，遵照創用 CC 姓名標示-非商業性-相同方式分享 4.0 國際授權條款 (CC BY-NC-SA 4.0) 使用。
 * 3D 模型名稱："R2-D2 (Animated)"
 * 模型來源 URL：https://skfb.ly/6pHQo
 * 原作者：StarWars-Universe
 * 授權條款：CC Attribution-NonCommercial-ShareAlike (CC BY-NC-SA 4.0)
