# qiuge-design

收錄優秀的 App 與軟體設計，供人與 Agent 在設計任務中查找和借鑑。每份案例是一張設計卡片：**問題、做法、為什麼有效、借鑑要點。**

```text
qiuge-design/
├── AGENTS.md          # 唯一的規則文件：查找、收錄、寫作原則、標籤
├── template.md        # 設計卡片模板
├── cases/
│   └── <product>-<flow>/
│       ├── case.md
│       └── 01-xxx.png
└── patterns/          # 3 張以上卡片出現同一做法時再歸納
```

- **查找**：`rg -n '^(title|tags):' cases` 列出全部卡片，或依標籤、關鍵字搜尋。詳見 [AGENTS.md](AGENTS.md)。
- **收錄**：複製 [template.md](template.md) 到 `cases/<product>-<flow>/case.md`，截圖放同一目錄。
- **追蹤來源**：[枯白設計分享的收錄清單與每日追蹤](sources/kubai087.md)，包含 999 小技巧系列、歷史覆蓋範圍與待補資料。

## 讓其他專案的 Agent 使用

在該專案的 `AGENTS.md` 或 `CLAUDE.md` 加入：

> 進行介面、互動流程或設計方案相關工作前，先閱讀 `/Users/feature/code/qiuge-design/AGENTS.md`，搜尋相關設計卡片並參考。引用時附卡片路徑與借鑑的具體做法。
