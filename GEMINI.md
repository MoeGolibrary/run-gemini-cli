# 项目守则 & 上下文

你必须遵循以下项目守则，否则你的任何请求将被拒绝。

## 1. 语言与交互

- **输出语言**: 请全程使用 **简体中文** 进行交流和生成内容。

## 2. 安全守则

1. **分支保护**: 绝对禁止直接修改 `main` 分支和 `release` 分支（必须通过 Pull Request 合并）。

## 3. 分支命名规范

- **格式**: `prefix-description` (仅使用连字符 `-`，**严禁**使用斜杠 `/`)
- **必须前缀**: `feature-` 或 `bugfix-`
- **长度约束**:
  - 总长度不超过 **30 字符**。
  - 描述部分（前缀后）尽量不超过 **3 个单词**。
- **示例**:
  - ✅ `feature-login-ui`
  - ✅ `bugfix-api-crash`
  - ❌ `feature/login` (使用了斜杠)
  - ❌ `feat-login` (前缀错误)

## 4. Commit & PR 标题规范

- **格式**: `<type>: <subject> <issue-id>`
- **Type 白名单**: `feat`, `fix`, `styles`, `perf`, `docs`
- **单号规则 (Issue ID)**:
  - 必须位于标题的 **最末尾**。
  - 若未指定具体单号，**必须**使用默认值 `IFRFE-0`。
- **示例**:
  - ✅ `feat: add user list api IFRFE-1024`
  - ✅ `styles: fix header padding MER-0`
  - ❌ `feat: add user list api` (未指定单号)
