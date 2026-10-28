# Lei Studio

> 一个人 + 一套自动化。独立开发者的产品、工具与内容基础设施。<br>
> *One person, a stack of automation — products, tools and content infrastructure.*

这里是我所有项目的主仓库（`leixlabs`）。个人 fork 与实验留在 [@0xkamalei](https://github.com/0xkamalei)。

---

## 在做的事

- **本地优先的产品**：能跑在你自己机器上的工具，不上传、不订阅、不依赖第三方 API Key。
- **内容基础设施**：把散的、非结构化的东西（网页、Slack、文档、视频、语音）变成可检索、可复用的数据。
- **小工具解决真问题**：先解决自己每天遇到的摩擦，再考虑它是不是一个产品。

---

## 主打项目

### [MonoSub](https://github.com/leixlabs/monosub) · Rust
把视频和音频转成文字，**全程本地，不上云**。播客、访谈、讲座、会议录音丢进去，出来的是可复制的文本。
已在 Microsoft Store 上架 · [下载](https://apps.microsoft.com/detail/9P6WTCCRQTVW)

### [Hangar](https://github.com/leixlabs/hangar) · Rust
Clash 订阅管理 CLI。订阅增删查、内置 HTTP 配置服务器、文件变更监控、后台常驻，还能用自然语言让 AI 改配置。

### [Paperplane](https://github.com/leixlabs/paperplane) · JavaScript
点一下工具栏图标，用 Chrome 内置 AI（Gemini Nano）在本地把网页提炼成要点，直接发到 Telegram 频道。MV3 无服务器架构，零后端、零 API Key，唯一的本地存储是用来去重的 IndexedDB。

### [食刻 / Calory](https://github.com/leixlabs/kcalapp) · Dart
本地 AI 食物热量记录。拍一张餐食照片，交给你自己配置的多模态 LLM，返回可编辑的食材、估算重量、热量与三大营养素；确认后汇入当日饮食和长期趋势。

### [Synapse](https://github.com/leixlabs/synapse) · Chrome Extension + Server
把多个社交平台的内容同步进 Notion 数据库。采集端在浏览器，落库端在自己服务器。 · [更新日志](https://updates.leix.dev)

### [Selected AI](https://github.com/leixlabs/selected-ai) · Swift
macOS 划词 AI 工具条：选中任意文本，就地调用模型操作，不打断你手上的活。

---

## 内容基础设施

| 项目 | 说明 |
|---|---|
| [word-radar](https://github.com/leixlabs/word-radar) · Go | 点词查词、发音，生词自动同步到 Obsidian。Chrome 扩展 + Go 后端。 |
| [slack-radar](https://github.com/leixlabs/slack-radar) · HTML | 被动采集 Slack 网页版消息落到本地 SQLite，**不用 Slack API**，数据直接从渲染后的 DOM 抽取。 |
| [google-doc-radar](https://github.com/leixlabs/google-doc-radar) · Go | Chrome 扩展 + Go 服务，抓取并全文检索 Google Docs 内容。 |
| [snore-monitor](https://github.com/leixlabs/snore-monitor) · Rust | 树莓派 3B 打鼾监测：麦克风连续录音存无损 WAV，规则检测器标记候选事件，按体积预算先进先出回收。**输出是候选片段，不是诊断。** |
| [ipa-master](https://github.com/leixlabs/ipa-master) · TypeScript | 英语音标学习站点。 |
| [dify-tool-firestore](https://github.com/leixlabs/dify-tool-firestore) / [dify-tool-google-sheet-fork](https://github.com/leixlabs/dify-tool-google-sheet-fork) · Python | 给 Dify 用的外部工具插件：Firestore 读写、Google Sheet 操作。 |

---

## 其他

- **私有仓库**里有正在打磨的产品和内部工具（时间追踪、增长分析、LLM 网关、各类 demo），成熟一个开源一个。
- 这些仓库里有不少我日常自动化的地基：Clash 代理运维、Hermes 工作流、内容排版与分发流水线。

## 技术栈

**Go** · **Rust** · **TypeScript / JavaScript** · **Swift** · **Python** · **Dart**
Chrome Extension (MV3) · SQLite · Notion API · Telegram Bot API · 本地推理（Gemini Nano / 多模态 LLM）

---

<sub>仓库按"能跑起来、能自己用"的标准维护。提 issue 我会看，PR 欢迎但要先说明它解决什么问题。</sub>
