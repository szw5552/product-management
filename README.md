# Product Management

一個給 AI Agent 使用的產品管理技能，協助 PM 撰寫 PRD、規格文件、功能規劃與優先級排序。透過連結您團隊的真實來源文件（Notion、Confluence、Google Docs 等），讓 AI Agent 在每次產品工作時都有正確的背景資訊。

## 這是什麼

`SKILL.md` 是一個通用的產品管理技能框架，設計用來被您的組織客製化。它告訴 AI Agent：

- 何時啟動這個技能（撰寫 PRD、審查規格、討論優先級…）
- 去哪裡找您團隊的核心文件（產品原則、定位、季度計劃…）
- 如何輸出符合人類可讀、可分享的產品文件

## 安裝

```bash
npx skills add szw5552/product-management
```

安裝後技能會自動放到正確位置，無需手動複製檔案。

## 快速開始

### 1. 填入您的文件連結

安裝完成後，編輯 `SKILL.md`，將 `[YOUR_LINK_HERE]` 替換為您公司的實際文件 URL：

```markdown
1. 產品原則
   https://your-notion-or-docs-link
```

### 2. 使用模板作為備援

如果尚未有對應的外部文件，`templates/` 資料夾裡的模板會作為預設值。

## 包含內容

### 技能

| 檔案 | 說明 |
|------|------|
| `SKILL.md` | 通用產品管理技能（需客製化） |

### 模板

| 檔案 | 用途 |
|------|------|
| `templates/prd-template.md` | PRD 撰寫模板 |
| `templates/prd-review-rubric.md` | PRD 審查評分表 |
| `templates/product-principles.md` | 產品原則 |
| `templates/core-value-proposition.md` | 核心價值主張 |
| `templates/11-star-experience.md` | 11 星體驗框架 |
| `templates/product-positioning.md` | 產品定位 |
| `templates/how-we-build.md` | 我們如何建構產品 |
| `templates/prioritization-framework.md` | 優先級排序框架 |
| `templates/product-research-bets.md` | 產品研究賭注 |
| `templates/quarterly-plan.md` | 季度計劃 |

### 範例

`examples/factory/` 展示了 Factory 如何將通用技能配置為使用 Notion 文件的實際範例，可作為您客製化的參考。

## 客製化建議

- 只需替換文件連結，技能的行為邏輯不需要改動
- 如果您的團隊有特殊的 PRD 格式，更新 `templates/prd-template.md` 即可
- 季度計劃和研究賭注變動頻繁，建議連結到會持續更新的外部文件，而非靜態模板
