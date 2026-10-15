# all-works｜完整作品一覽

大樹教練 2026-10-15 交辦：一頁看完做過的所有網頁／作品（不管有沒有上架），可搜尋人名。
**只給教練自己看，已加 noindex，不對外推廣。**

- 頁面：https://coach1973.github.io/all-works/
- `index.html`：頁面本體。開啟時即時讀取「大樹作品一覽（coach888）」與 GitHub 公開倉庫清單，再與 `data.json` 合併去重。
- `data.json`：GitHub 全部倉庫（含私有）＋策展名冊，由 `workspace/scripts/all_works_refresh.py` 產生。
  **事件觸發更新，沒有任何排程或輪詢**：策展上架完成、策展後台下架／重新上架／刪除、Claude Code 執行 `gh repo create` 的那一刻自動跑。
- 手動更新：`python3 ~/.openclaw/workspace/scripts/all_works_refresh.py`
