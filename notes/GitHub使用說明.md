---
title: GitHub 使用說明
tags: [GitHub, 筆記]
date: 2026-03-03
created: 2026-03-03T18:02:00+08:00
---

# GitHub 使用說明

## 📊 當前狀態

**GitHub CLI 已認證：** ✅  
**帳號：** jetannku-hash  
**Token：** 已使用 PAT（Personal Access Token）

---

## 🚀 我可以幫你做的事

### 倉庫管理

| 功能 | 指令 | 範例 |
|------|--------|------|
| **建立倉庫** | `gh repo create <name>` | `gh repo create "我的專案" --public` |
| **克隆倉庫** | `gh repo clone <repo>` | `gh repo clone owner/repo` |
| **查看倉庫** | `gh repo view <owner/repo>` | `gh repo view jetannku-hash/Test` |
| **列出倉庫** | `gh repo list --limit 10` | 列出你的 repositories |
| **刪除倉庫** | `gh repo delete <repo>` | 刪除指定 repository |

### Issues 管理

| 功能 | 指令 | 範例 |
|------|--------|------|
| **建立 Issue** | `gh issue create --title "標題"` | 建立新問題 |
| **列出 Issues** | `gh issue list --limit 10` | 查看問題清單 |
| **查看 Issue** | `gh issue view <number>` | 查看特定問題 |

### Pull Requests

| 功能 | 指令 | 範例 |
|------|--------|------|
| **建立 PR** | `gh pr create --title "標題"` | 建立 Pull Request |
| **列出 PRs** | `gh pr list --limit 10` | 查看 PR 清單 |
| **Checkout PR** | `gh pr checkout <number>` | 切換到 PR 分支 |

---

## ✅ 已測試功能

### 測試結果

1. **認證成功** ✅
   ```bash
   $ gh auth status
   Logged in to github.com account jetannku-hash
   ```

2. **列出倉庫** ✅
   - `jetannku-hash/test-ash-github-integration`
   - `jetannku-hash/Test`

3. **克隆倉庫** ✅
   - 成功克隆 `jetannku-hash/Test` 到 `/tmp/Test`

4. **建立新倉庫** ✅
   - 成功建立 `test-ash-github-integration`
   - 連結：https://github.com/jetannku-hash/test-ash-github-integration

---

## 💡 使用建議

### 權限要求

你的 PAT 必須包含以下權限：
- ✅ `repo` - 完整倉庫存取權限
- ✅ `workflow` - GitHub Actions 權限（如果需要）
- ✅ `admin:org` - 組織管理（如果需要）

### 安全提醒

⚠️ **PAT 已設定為環境變數**
- 每次執行 GitHub 命令都需要設定 `GITHUB_TOKEN`
- 我會自動在命令中包含 `export GITHUB_TOKEN=...`

### 使用方式

你可以直接跟我說：
- 「建立一個新倉庫，名稱是...」
- 「克隆我的 Test 倉庫到工作目錄」
- 「建立一個 Issue，標題是...」
- 「列出我所有的倉庫」

我會自動執行相應的 GitHub 命令！

---

## 🔗 參考資源

- [GitHub CLI 文件](https://cli.github.com/manual/)
- [操作範例說明]
- [[操作範例說明]]

---
**標籤：** #GitHub #筆記
