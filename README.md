# 🦐 小虾米 Xiaoxiaomi

<img src="banner.png" width="100%"/>

[![GitHub stars](https://img.shields.io/github/stars/BEelzebub-dev/xiaoxiaomi?style=flat-square&color=ff6b6b)](https://github.com/BEelzebub-dev/xiaoxiaomi/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/BEelzebub-dev/xiaoxiaomi?style=flat-square&color=4ecdc4)](https://github.com/BEelzebub-dev/xiaoxiaomi/network/members)
[![License](https://img.shields.io/github/license/BEelzebub-dev/xiaoxiaomi?style=flat-square&color=ffe66d)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.12+-blue?style=flat-square)](https://python.org)
[![OpenClaw](https://img.shields.io/badge/OpenClaw-Agent-blueviolet?style=flat-square)](https://openclaw.ai)

> 🧠 我的 AI 助手技能仓库 — 微信语音播客、公众号摘要、图像生成、文档处理

---

## 🎙️ 技能列表

### 🗣️ 播客系列
| 技能 | 说明 |
|------|------|
| [tts-podcast](skills/tts-podcast/) | 多角色语音播客生成，主持人/嘉宾交替音色，微信直接发送 |
| [JMTTS](skills/JMTTS/) | 即梦/Edge TTS 语音合成，jimeng 音色 + Edge 备用 |

### 📰 内容处理
| 技能 | 说明 |
|------|------|
| [jayson-wx-sum](skills/jayson-wx-sum/) | 微信公众号文章抓取，requests + 微信UA 直接解析正文 |
| [douyin-parse](skills/douyin-parse/) | 抖音视频解析 |
| [summarize](skills/summarize/) | 内容摘要总结 |

### 🎨 图像生成
| 技能 | 说明 |
|------|------|
| [minimax-image-gen](skills/minimax-image-gen/) | MiniMax image-01 人脸保持图像生成 |
| [doubao-img](skills/doubao-img/) | 豆包图像生成（备用） |

### 📄 文档办公
| 技能 | 说明 |
|------|------|
| [minimax-docx](skills/minimax-docx/) | Word 文档生成 |
| [minimax-xlsx](skills/minimax-xlsx/) | Excel 表格生成 |
| [pptx-generator](skills/pptx-generator/) | PPT 幻灯片生成 |
| [minimax-pdf](skills/minimax-pdf/) | PDF 文档生成 |
| [ke-office-automation](skills/ke-office-automation/) | Office 批量自动化 |

### 💬 微信生态
| 技能 | 说明 |
|------|------|
| [wechat-869-media-sender](skills/wechat-869-media-sender/) | 微信消息/语音/图片发送，869 接口 |
| [wechat-article-exporter](skills/wechat-article-exporter/) | 微信文章导出 |
| [lucky-music](skills/lucky-music/) | 音乐卡片发送 |

### 🛠️ 开发工具
| 技能 | 说明 |
|------|------|
| [skill-vetter](skills/skill-vetter/) | Skill 安全审查，安装前必读 |
| [agent-browser](skills/agent-browser/) | 浏览器自动化 |
| [mcporter](skills/mcporter/) | MCP 工具调用 |
| [github](skills/github/) | GitHub CLI 操作 |

---

## 🏗️ 系统架构

```
微信 / 飞书
     ↓
OpenClaw Gateway
     ↓
  AI (小虾米)
     ↓
   Skills
 ┌──┴──┐
TTS   图像   文档
播客  生成  Office
```

## 🔒 安全原则

所有 Skill 安装前必须通过 `skill-vetter` 审查：

| 等级 | 类型 | 处理方式 |
|------|------|---------|
| 🚨 高危 | `eval/exec`、未知网络请求 | 拒绝安装 |
| 🔴 中高 | 读取凭据文件、系统配置 | 人工审批 |
| 🟡 中低 | 文件操作、API 调用 | 完整代码审查 |
| 🟢 低危 | 纯本地处理 | 快速安装 |

---

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

---

*🦐 小虾米不是聊天机器人，是真正干活的助手。*
