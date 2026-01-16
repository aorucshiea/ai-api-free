# AI API Free

A comprehensive collection of free AI model APIs and providers.

[English](#english) | [中文](README.zh-CN.md)

---

## English

### Overview

This repository maintains a curated list of free AI model APIs and providers that you can use without paying. Perfect for developers, researchers, and hobbyists who want to experiment with AI models without breaking the bank.

### Why 1000+ Daily Requests Are Enough for Normal Use

Even if someone uses AI 24/7 without eating or sleeping, with each request taking 1.5 minutes (90 seconds), they would only consume about 960 requests per day:

```
24 hours × 60 minutes × 60 seconds = 86,400 seconds per day
86,400 seconds ÷ 90 seconds per request = 960 requests per day
```

Therefore, **1000+ daily requests are completely sufficient for normal use** - unless you're running multiple concurrent windows or automated scripts at scale.

### Usage Patterns: Regular Users vs Programmers

In the current AI application ecosystem, there are significant differences in usage patterns between regular users and programmers (AI coding users). This difference is mainly reflected in the definition of "requests" - whether it's the number of commands actively issued by users, or the number of API calls triggered in the background.

The following is an analysis and estimation based on typical usage scenarios in 2025:

#### 1. Regular Users Using AI

Regular users typically use AI as a tool for search, writing, drawing, or daily life assistance.

- **Use Cases**: Q&A, polishing emails/documents, translation, travel planning, image generation, simple math calculations, etc.
- **Request Frequency (Estimated)**:
  - **Light Users**: 5 - 15 times per day. Occasionally ask questions when encountering problems, or occasionally use AI to polish a piece of text.
  - **Heavy Users (AI Natives)**: 30 - 60 times per day. These users are accustomed to using AI as their first-choice search engine, or even use AI for long-term conversation companionship or brainstorming.
- **Characteristics**: Requests are usually discrete and non-continuous. One interaction may contain dozens of rounds of dialogue (context), but the number of core intents (prompts) is relatively small.

#### 2. Programmers/AI Coding Users Using AI

Programmers use AI (such as Cursor, GitHub Copilot, ChatGPT, and our Zhipu's CodeGeeX, etc.) much more frequently because programming is a high-density mental and text output activity.

Here we need to distinguish between "explicit requests" and "implicit requests":

**A. Explicit Requests (Active Questions/Commands)**

Programmers actively input questions in IDEs (Integrated Development Environments) or chat windows, asking to generate code, explain bugs, or refactor.

- **Estimated Frequency**: 40 - 100 times per day.
  - When writing new features, may frequently ask to "write a function", "write a unit test".
  - When debugging, will continuously paste error messages asking "why is this wrong", "how to fix this".

**B. Implicit Requests (Auto-completion/Inline Suggestions)**

This is the core function of modern AI coding tools (like Copilot). Every time a programmer types a few letters, AI will make a request in the background to predict the next word or code block.

- **Estimated Frequency**: 200 - 1000 times per day or even higher.
  - Although each request has very few tokens, due to the very frequent typing during programming, these "micro-requests" will be continuously triggered. Programmers may not realize it, but the background is always performing real-time completion through AI.

#### Summary Comparison

| User Type | Core Request Type | Estimated Daily Requests | Main Behavior Pattern |
|-----------|-------------------|-------------------------|----------------------|
| Regular Users | Explicit Dialogue | 10 - 30 times (average) | Ask questions, write articles, draw images, intermittent use |
| Programmers | Explicit Commands | 40 - 100 times | Explain code, generate functions, Debug, continuous use |
| Programmers | Implicit Completion | 500+ times | Auto-suggestions triggered by typing code, accompanying use |

#### Conclusion

If you calculate the number of times users press Enter to send, programmers are about 3 to 5 times that of regular users; if you calculate the number of API calls actually processed by the model (including auto-completion), programmers' usage may be 20 to 50 times that of regular users.

### Official / Major Platforms (Direct Official API)

| Provider | Free Models | Notes |
|----------|-------------|-------|
| **iFlytek Spark (讯飞星火)** | spark-lite | Permanently free, unlimited tokens, QPS≈2 |
| **Baidu ERNIE (百度文心)** | ERNIE-Speed-8K/128K/Lite/Tiny | Long-term free quota, RPM≈300, TPM≈300000 |
| **Tencent Hunyuan (腾讯混元)** | hunyuan-lite | Free, max 5 concurrent requests |
| **Zhipu AI (智谱)** | glm-4-flash | Long-term free API, concurrent≈5 |
| **InternLM (书生·浦语)** | internlm2.5-latest | Requires application, RPM=10, TPM=5000 |

### Aggregation / Proxy Platforms (HTTP API with Free Quota)

| Provider | Description | Notes |
|----------|-------------|-------|
| **iflow** ⭐ | ~2000 API calls/day, 1 concurrent, includes GLM-4.6, Qwen3, DeepSeek - Sufficient for normal use |
| **NVIDIA NIM** ⭐ | 1000-5000 credits for development, includes GLM-4.7, MiniMax-M2.1 - Sufficient for normal use |
| **SiliconFlow** | 20M free tokens on signup, 9B+ models permanently free |
| **OpenRouter** | 50-1000 daily :free model calls depending on balance |
| **ModelScope (魔塔)** ⭐ | 2000 free calls/day, 500 per model, covers Qwen, DeepSeek, GLM - Sufficient for normal use |
| **Cherry Studio** | Desktop client with built-in free models, no API key required |
| **anigravity** ⭐ | Weekly free quota for Gemini and Claude latest models - Sufficient for normal use |
| **opencode zen** | Curated quality models (GLM4.7, MiniMax2.1) - Not recommended, requires large quota |

### Special Free APIs

| Provider | Description | Notes |
|----------|-------------|-------|
| **Free Qwen3** 🆓 | Completely free, no registration required - Sufficient for normal use |
| **Free QwQ-32B** 🆓 | QwQ-32B distributed API, completely free, no registration, unlimited calls - Sufficient for normal use |
| **Zhipu Z.AI** | Web chat interface, free web access to GLM-4.6/4.7 |
| **Baidu ERNIE Web** | Web chat interface, officially announced completely free |

### Legend

- ⭐ = Recommended
- 🆓 = Completely free, no registration required

### Contributing

Found a new free AI API provider? Feel free to submit a pull request or open an issue!

### License

MIT License

---

## 中文

### 概述

本仓库维护了一个精选的免费 AI 模型 API 和供应商列表，无需付费即可使用。非常适合开发者、研究人员和爱好者在不花费太多的情况下实验 AI 模型。

### 官方/大厂自营平台（直接官方 API）

| 供应商 | 免费模型 | 说明 |
|--------|----------|------|
| **讯飞星火** | spark-lite | 永久免费，Tokens 不限，QPS≈2 |
| **百度文心/千帆** | ERNIE-Speed-8K/128K/Lite/Tiny | 长期免费配额，RPM≈300，TPM≈300000 |
| **腾讯混元** | hunyuan-lite | 免费，最多 5 路并发 |
| **智谱 AI** | glm-4-flash | 首个长期免费 API，并发数约 5 |
| **书生·浦语** | internlm2.5-latest | 需要申请开通，RPM=10，TPM=5000 |

### 聚合/中转平台（HTTP API，有免费额度）

| 供应商 | 描述 | 说明 |
|--------|------|------|
| **iflow** ⭐ | 每天约 2000 次 API 调用，1 并发，包含 GLM-4.6、Qwen3、DeepSeek - 正常人完全够用 |
| **NVIDIA NIM** ⭐ | 1000-5000 credits 用于开发，包含 GLM-4.7、MiniMax-M2.1 - 正常人完全够用 |
| **SiliconFlow (硅基流动)** | 注册赠送 2000 万 Tokens，9B 以下模型永久免费 |
| **OpenRouter** | 50-1000 次/天 :free 模型调用（取决于余额） |
| **ModelScope (魔塔)** ⭐ | 每天 2000 次免费调用，单模型 500 次/天，覆盖 Qwen、DeepSeek、GLM - 正常人完全够用 |
| **Cherry Studio** | 桌面客户端，内置免费模型，无需 API Key |
| **anigravity** ⭐ | 每周可免费使用一定额度的 Gemini 和 Claude 最新模型 - 正常人完全够用 |
| **opencode zen** | 精选高质量模型（GLM4.7、MiniMax2.1） - 不推荐，需要很多额度 |

### 特殊免费 API

| 供应商 | 描述 | 说明 |
|--------|------|------|
| **Free Qwen3** 🆓 | 完全免费，无需注册 - 正常人完全够用 |
| **Free QwQ-32B** 🆓 | QwQ-32B 分布式 API，完全免费，无需注册，无调用上限 - 正常人完全够用 |
| **智谱 Z.AI** | 网页聊天界面，免费网页访问 GLM-4.6/4.7 |
| **百度文心一言网页版** | 网页聊天界面，官方宣布全面免费 |

### 图例

- ⭐ = 推荐使用
- 🆓 = 完全免费，无需注册

### 贡献

发现了新的免费 AI API 供应商？欢迎提交 Pull Request 或创建 Issue！

### 许可证

MIT License
