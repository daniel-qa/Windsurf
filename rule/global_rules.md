# 基本設定
- 使用繁體中文進行對話

# 專案架構
## 技術棧
- Vue 3
- Element Plus
- Vue I18n

## 代碼規範
### 風格指南
- 使用 Composition API 的 setup 語法
- 響應式數據：
  - 基本類型：使用 `ref`
  - 物件/陣列：使用 `reactive`

### 命名規範
- 組件：`PascalCase`（例如：`UserProfile.vue`）
- 變數/函數：`camelCase`
- 常量：`UPPER_CASE`

# 專案結構
```
/src
  /components    # 共用組件
  /views         # 頁面視圖
  /utils         # 工具函數
  /api           # API 封裝
  /assets
    /styles      # 樣式文件
```

# 開發工具
## 核心套件
- 時間處理：`dayjs`
- HTTP 請求：封裝的 `$api`
- 表單驗證：Element Plus 驗證規則
