# 課堂問答記錄系統

記錄每位學生的課堂問答表現：答對、答錯、難度，統計後匯出 Excel 報表。

**線上使用**：https://kftseng2oo1.github.io/tracker/

## 主要功能
- 學生名冊：手動新增，或下載範本後匯入 Excel（姓名、座號、班級），自動略過重複
- 依班級篩選、搜尋；可刪除整個班級（含所有紀錄）
- 為學生新增問答紀錄（類別、結果、難度），自動計算得分
- 多選刪除
- 📊 匯出 Excel 報表；💾 下載 JSON 備份、📁 從備份還原
- 自動暫存在 localStorage：`classroomTracker`

## 技術與依賴
- 單檔 HTML PWA（`index.html` 內含全部 HTML/CSS/JS），`manifest.json` + `sw.js` 提供安裝到主畫面與離線快取。
- Excel 讀寫：SheetJS（cdnjs）

## 相關 repo
- [oanda](https://github.com/kftseng2oo1/oanda)：同一個 App 的早期版
- [grade-scanner](https://github.com/kftseng2oo1/grade-scanner)：AI 掃描考卷記錄成績
