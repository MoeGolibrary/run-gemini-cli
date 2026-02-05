# 项目守则 & 上下文

你必须遵循以下项目守则，否则你的任何请求将被拒绝。

## 1. 语言与交互

- **输出语言**: **简体中文**

## 2. 安全守则

1. **分支保护**: 绝对禁止直接修改 `main` 分支和 `release` 分支（必须通过 Pull Request 合并）。

## 3. 分支命名规范 & Commit & PR 标题规范

生成短标识：feature-或bugfix- + -分隔描述（≤3词，≤30字符，禁/）；
生成 Commit/PR：<type>: <subject> <ISSUE-ID>，type 限定，Issue 必须在末尾，推荐使用 IFRFE-0（在用户没说的情况下）。

# Code Review 

当需要进行 Code Review 工作时，必须遵循以下守则：
1. 应当且必须将英文语句拼写错误、语法不恰当、时态冗余等“非母语常犯错误”作为 comment 点在后续提交。
2. 在进行 CR 之前，你必须先阅读 README.md 文件以及 docs/ 目录下 md 文件，获取关于项目的基础知识以及开发前必读内容。

# Invoke

当你执行 invoke 能力时，在代码提交前务必根据项目实际配置进行 Lint 检查和格式化

# 项目启动

1. 如果你希望通过`pnpm i`来安装依赖，执行之前，务必通过以下代码登录私有云
```bash
npx npm-cli-login \
  -u "$NPM_PUBLISHER_USR" \
  -p "$NPM_PUBLISHER_PSW" \
  -e devops@moego.pet \
  --config-path .npmrc \
  -r "https://nexus.devops.moego.pet/repository/npm-local/"
```
