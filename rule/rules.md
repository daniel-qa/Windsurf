# TEAMModelOS 專案規則

## 專案概述
- 全端企業級應用程式
- 後端：.NET Core
- 前端：Vue 3 + TypeScript

## 代碼風格

### 後端 (C#)
- 命名規範：
  - 類別：`PascalCase`
  - 方法：`PascalCase`
  - 變數：`camelCase`
  - 常數：`PascalCase`

### 前端 (Vue/TypeScript)
- 組件：`PascalCase`
- 變數/函數：`camelCase`
- 常數：`UPPER_SNAKE_CASE`
- 使用 Composition API 的 `<script setup>` 語法

## 專案結構

### 後端
- `Controllers/`: API 控制器
- `Models/`: 資料模型
- `Services/`: 業務邏輯
- `Filters/`: 過濾器
- `JsonFile/`: JSON 配置文件

### 前端 (ClientApp)
- `src/components/`: 共用組件
- `src/views/`: 頁面組件
- `src/api/`: API 封裝
- `src/utils/`: 工具函數
- `src/assets/`: 靜態資源

## 開發規範

### Git 提交規範
- 使用 Conventional Commits 規範
- 類型前綴：feat, fix, docs, style, refactor, test, chore

### 文檔要求
- 公開 API 必須有 XML 註解
- 複雜邏輯需添加註解說明
- 更新 README.md 記錄重要變更

## 測試要求
- 核心功能需包含單元測試
- API 需包含整合測試
- 前端組件需包含單元測試

## 安全規範
- 敏感信息必須使用環境變量
- 所有 API 默認需要認證
- 輸入數據必須驗證

## 部署規範
- 使用 Docker 容器化部署
- 區分開發/測試/生產環境配置
- 日誌集中管理

## 代碼審查
- 至少需要一個審核者
- 通過 CI/CD 流水線後才能合併
- 保持程式碼風格一致
