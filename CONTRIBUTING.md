# 🤝 贡献指南

## 如何贡献

1. **Fork** 本仓库
2. 创建你的分支 (`git checkout -b feature/你的技能名`)
3. 提交更改 (`git commit -m 'feat: 添加 xxx 技能'`)
4. 推送到你的 Fork (`git push origin feature/你的技能名`)
5. 提交 Pull Request

## 技能提交规范

新增技能需包含：
- `SKILL.md` — 功能说明、使用方法
- `scripts/` — 核心脚本（Python 优先）
- `_meta.json` — 技能元信息

## ⚠️ 安全要求

- 禁止提交含凭据、API Key 的代码
- 所有技能必须通过 `skill-vetter` 审查
- 网络请求必须说明请求目标与用途

## 🐛 发现 Bug

欢迎提交 Issue，请注明：
- 复现步骤
- 预期行为 vs 实际行为
- 环境信息（Python 版本、系统等）
