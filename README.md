# Video Editing Workflow

一套可獨立使用的 Codex skill，用於整理影片素材、規劃剪輯、建立 AI 輔助粗剪、混剪動畫與實拍，並檢查成片品質。

**版本：** 1.0.0（2026-10-17）

## 適用工作

- 大量素材盤點與候選鏡頭整理
- 依故事、旁白句 ID 與鏡號規劃時間軸
- 使用 AI 建立可追溯、可人工修正的粗剪草案
- 生成式影片的角色／場景連續性和鏡頭組接
- Remotion 等程式化動畫與 DaVinci Resolve 等剪輯軟體的素材交接
- 旁白、字幕、音效、配樂、片頭片尾和成片驗收

本 skill 把 AI 用於素材檢索、候選鏡頭、時間軸草稿及重複操作。AI 的剪輯結果仍須人工確認鏡頭是否合用、故事是否連貫、音畫是否正確，並播放成片驗收。

## 安裝

將此 repo 複製到 Codex skills 目錄：

```text
<CODEX_HOME>/skills/video-editing-workflow/
```

至少需要 `SKILL.md`。保留 `references/` 可查閱三份字幕的分析摘要與企劃／剪輯交接規格。重新整理技能清單或重新開啟 Codex 後即可使用。

## 與 multichannel-video-workflow 搭配

`multichannel-video-workflow` 負責頻道、選題、查證、腳本、品牌與分鏡；本 skill 接手素材整理、鏡頭選擇、時間軸、混剪及驗收。兩者共用鏡號、旁白句 ID、素材來源、品牌核定路徑與輸出檢查資料。若只是企劃、腳本或既有圖卡影片，不需要完整剪輯流程。

## 工具與來源

DaVinci Resolve、MCP、Remotion、LibTV 和生成式影片平台都是可替換工具。使用前應核對目前官方說明、版本、方案、授權、MCP 發布者及實際可用操作。本 skill 不假設不同工具可直接讀寫彼此的專案檔，也不承諾影片示範中的速度或品質結果。

方法整理自使用者提供的三份 SRT 字幕：LibTV 導演台教程、DaVinci＋Codex／Claude 剪輯實測、Remotion＋DaVinci 動畫流程。時間碼摘要和限制見 [`references/three-video-editing-analysis.md`](references/three-video-editing-analysis.md)；企劃交接和品質檢查見 [`references/editing-workflow-methods.md`](references/editing-workflow-methods.md)。字幕檔名中的「2026年11月最新」晚於分析日期 2026-10-17，因此不把檔名當作已驗證的發布日期。

## 檔案

```text
video-editing-workflow/
├── README.md
├── SKILL.md
├── VERSION
└── references/
    ├── editing-workflow-methods.md
    └── three-video-editing-analysis.md
```

此 repo 未附 LICENSE 檔；公開可見不代表授予複製或再散布權利。
