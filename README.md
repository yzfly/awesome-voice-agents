# Awesome Voice Agents [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of voice AI agent frameworks, tools, resources, and best practices | 精选的语音 AI Agent 框架、工具、资源和最佳实践

Welcome to **Awesome Voice Agents**! This is a carefully curated collection of resources related to voice AI agents, covering core technologies such as endpoint detection, turn-taking management, real-time speech recognition, and speech synthesis.

本项目精心收录语音 AI Agent 相关的优质资源，涵盖端点检测、话轮管理、实时语音识别、语音合成等核心技术。

**Maintainer | 维护者: 云中江树**

💬 **Join Voice Agent Community | 加入 Voice Agent 交流群**  
Add WeChat | 添加微信: **1796060717**  
欢迎 Voice Agent 从业者和爱好者加入交流！

---

## Contents | 目录

- [Frameworks & Platforms | 框架与平台](#frameworks--platforms--框架与平台)
- [VAD (Voice Activity Detection) | 语音活动检测](#vad-voice-activity-detection--语音活动检测)
- [Turn Detection & Endpointing | 话轮检测与端点检测](#turn-detection--endpointing--话轮检测与端点检测)
- [STT (Speech-to-Text) | 语音转文本](#stt-speech-to-text--语音转文本)
- [TTS (Text-to-Speech) | 文本转语音](#tts-text-to-speech--文本转语音)
- [Developer Communities & Resources | 开发者社区与资源](#developer-communities--resources--开发者社区与资源)
- [Learning Resources | 学习资源](#learning-resources--学习资源)
- [Contributing | 贡献指南](#contributing--贡献指南)

---

## Frameworks & Platforms | 框架与平台

### Comprehensive Frameworks | 综合性框架

| Name | Stars | Description | Notes |
|------|-------|-------------|-------|
| [TEN Framework](https://github.com/TEN-framework/ten-framework) | ![GitHub Repo stars](https://badgen.net/github/stars/TEN-framework/ten-framework) | Open-source framework for conversational voice AI agents with multimodal capabilities (voice, vision, avatar). Low-latency, high-quality real-time assistant. | 支持多模态，低延迟高质量。[Demo](https://agent.theten.ai/) |
| [Pipecat](https://github.com/pipecat-ai/pipecat) | ![GitHub Repo stars](https://badgen.net/github/stars/pipecat-ai/pipecat) | Open Source framework for voice and multimodal conversational AI. Modular design with support for multiple STT, LLM, TTS services. | 模块化设计，支持多平台 SDK |
| [LiveKit Agents](https://github.com/livekit/agents) | ![GitHub Repo stars](https://badgen.net/github/stars/livekit/agents) | Powerful framework for building realtime voice AI agents. Fully open-source, WebRTC support, built-in semantic turn detection. | 完全开源，内置语义话轮检测 |
| [OpenAI Realtime Agents](https://github.com/openai/openai-realtime-agents) | ![GitHub Repo stars](https://badgen.net/github/stars/openai/openai-realtime-agents) | Advanced agentic patterns built on OpenAI Realtime API. Multi-agent collaboration, handoffs, tool use. | OpenAI 官方示例，支持多 Agent |
| [Vocode Core](https://github.com/vocodedev/vocode-core) | ![GitHub Repo stars](https://badgen.net/github/stars/vocodedev/vocode-core) | Build voice-based LLM agents. Modular and open source. Real-time streaming conversations. | 支持电话、Zoom 等场景部署 |
| [Bolna](https://github.com/bolna-ai/bolna) | ![GitHub Repo stars](https://badgen.net/github/stars/bolna-ai/bolna) | End-to-end open source production-ready voice agents platform. Build voice assistants through JSON config. | 生产就绪，支持 Twilio/Plivo |


### Specialized Solutions | 专用解决方案

| Name | Stars | Description | Notes |
|------|-------|-------------|-------|
| [BentoVoiceAgent](https://github.com/bentoml/BentoVoiceAgent) | ![GitHub Repo stars](https://badgen.net/github/stars/bentoml/BentoVoiceAgent) | Build phone calling voice agents fully powered by open source models. Uses BentoML for deployment. | 完全基于开源模型 |
---

## VAD (Voice Activity Detection) | 语音活动检测

Voice Activity Detection (VAD) is a key technology for identifying the presence of human speech in audio streams.

VAD 是识别音频流中是否存在人声的关键技术，用于过滤静音、减少计算成本、改善下游处理准确性。

### Core VAD Models | 核心 VAD 模型

| Name | Stars | Description | Notes |
|------|-------|-------------|-------|
| [Silero VAD](https://github.com/snakers4/silero-vad) | ![GitHub Repo stars](https://badgen.net/github/stars/snakers4/silero-vad) | Pre-trained enterprise-grade Voice Activity Detector. High-performance, low-latency, multi-language support. | ⭐ 最流行的 VAD 模型，支持 WebAssembly |
| [VAD (Browser)](https://github.com/ricky0123/vad) | ![GitHub Repo stars](https://badgen.net/github/stars/ricky0123/vad) | Voice activity detector for the browser with a simple API. Pure frontend implementation. | 浏览器端 VAD，零后端依赖 |
| [py-webrtcvad](https://github.com/wiseman/py-webrtcvad) | ![GitHub Repo stars](https://badgen.net/github/stars/wiseman/py-webrtcvad) | Python interface to Google WebRTC Voice Activity Detector. Classic signal processing approach. | 经典轻量方案，快速 |

### Noise Cancellation | 降噪增强

| Name | Stars | Description | Notes |
|------|-------|-------------|-------|
| [Krisp AI](https://krisp.ai/) | - | AI-powered background voice and noise cancellation. Krisp Server SDK for voice agents. | 显著改善 VAD 准确性，减少误触发 |

---

## Turn Detection & Endpointing | 话轮检测与端点检测

Turn Detection/Endpointing determines when a user has finished speaking - a core component of natural conversation.

话轮检测判断用户何时结束说话，是实现自然对话的核心技术。

### Intelligent Turn Detection Models | 智能话轮检测模型

| Name | Stars | Description | Notes |
|------|-------|-------------|-------|
| [Smart Turn (Pipecat)](https://github.com/pipecat-ai/smart-turn) | ![GitHub Repo stars](https://badgen.net/github/stars/pipecat-ai/smart-turn) | Open-source turn detection model (BSD 2-clause). Supports 23 languages. Semantic and audio feature-based. No GPU required for real-time inference. | 完全开源，提供 Fal 托管服务（免费）|
| [LiveKit Turn Detector](https://github.com/livekit/agents) | ![GitHub Repo stars](https://badgen.net/github/stars/livekit/agents) | Transformer-based semantic analysis. 85% true positive rate, ~50ms inference time. | 基于 Transformer，结合 VAD 效果最佳 |

### Commercial Solutions | 商业解决方案

| Name | Description | Notes |
|------|-------------|-------|
| [OpenAI Realtime API](https://platform.openai.com/docs/guides/realtime) | Semantic VAD with context-aware turn detection. Built into end-to-end model. | 上下文感知，端到端 |
| [AssemblyAI Universal-Streaming](https://www.assemblyai.com/blog/turn-detection-endpointing-voice-agent) | Intelligent endpointing with semantic analysis. Real-time streaming transcription. | 语义端点检测，实时流式 |
| [Retell AI Turn-Taking](https://www.retellai.com/) | Enterprise-grade turn-taking management. Adaptive endpointing, handles complex noise environments. | 企业级方案，适应噪音环境 |

---

## STT (Speech-to-Text) | 语音转文本

### Realtime Whisper Implementations | Whisper 实时流式实现

OpenAI Whisper is the most powerful open-source speech recognition model, but doesn't natively support real-time streaming. The following projects implement streaming transcription:

| Name | Stars | Description | Notes |
|------|-------|-------------|-------|
| [Whisper Streaming (UFAL)](https://github.com/ufal/whisper_streaming) | ![GitHub Repo stars](https://badgen.net/github/stars/ufal/whisper_streaming) | Whisper realtime streaming for long speech-to-text. Local agreement policy with self-adaptive latency. 3.3s latency. | 使用局部一致性策略，自适应延迟 |
| [WhisperLive](https://github.com/collabora/WhisperLive) | ![GitHub Repo stars](https://badgen.net/github/stars/collabora/WhisperLive) | Nearly-live implementation of OpenAI's Whisper. TensorRT acceleration support. Browser extensions and iOS client. | 支持 TensorRT 加速和多平台 |
| [Whisper Real Time](https://github.com/davabase/whisper_real_time) | ![GitHub Repo stars](https://badgen.net/github/stars/davabase/whisper_real_time) | Real time transcription with OpenAI Whisper. Continuously records and concatenates audio. | 简单易用的实时转录演示 |
| [VoiceStreamAI](https://github.com/alesaccoia/VoiceStreamAI) | ![GitHub Repo stars](https://badgen.net/github/stars/alesaccoia/VoiceStreamAI) | Near-realtime audio transcription using self-hosted Whisper and WebSocket. Supports Faster Whisper, integrated VAD. | WebSocket 架构，分块处理策略 |
| [speech-to-text (reriiasu)](https://github.com/reriiasu/speech-to-text) | ![GitHub Repo stars](https://badgen.net/github/stars/reriiasu/speech-to-text) | Real-time transcription using faster-whisper. HTML GUI with WebSocket support. SRT subtitle generation. | 提供 GUI，支持字幕生成 |
| [Whispering](https://github.com/shirayu/whispering) | ![GitHub Repo stars](https://badgen.net/github/stars/shirayu/whispering) | Streaming transcriber with whisper. Client-server architecture support. | 支持客户端-服务器架构 |

### Commercial STT APIs | 商业 STT 服务

| Name | Description | Notes |
|------|-------------|-------|
| [OpenAI Whisper API](https://platform.openai.com/docs/guides/speech-to-text) | Cloud-based Whisper API. Easy integration, pay-as-you-go pricing. | 云端 Whisper，按需付费 |
| [Azure Speech Services](https://azure.microsoft.com/products/ai-services/speech-to-text) | Microsoft's STT service. Multi-language support, custom model training. | 支持多语言，自定义模型 |
| [Deepgram](https://deepgram.com/) | Enterprise-grade real-time STT API. Ultra-low latency, streaming transcription. | 超低延迟，流式转录 |
| [AssemblyAI](https://www.assemblyai.com/) | Speech AI API with Universal-Streaming model. Immutable transcription, intelligent endpointing. | 不可变转录，智能端点检测 |

---

## TTS (Text-to-Speech) | 文本转语音

### Open Source TTS Models | 开源 TTS 模型

| Name | Stars | Description | Notes |
|------|-------|-------------|-------|
| [GPT-SoVITS](https://github.com/RVC-Boss/GPT-SoVITS) | ![GitHub Repo stars](https://badgen.net/github/stars/RVC-Boss/GPT-SoVITS) | Few-shot voice cloning TTS. High-quality synthesis. | 少样本语音克隆 |
| [Bark](https://github.com/suno-ai/bark) | ![GitHub Repo stars](https://badgen.net/github/stars/suno-ai/bark) | Transformer-based TTS model. Generates highly realistic audio including music, sound effects. | 可生成音乐和音效 |
| [Coqui TTS](https://github.com/coqui-ai/TTS) | ![GitHub Repo stars](https://badgen.net/github/stars/coqui-ai/TTS) | Deep learning TTS toolkit. 1100+ pre-trained models. Voice cloning support. | ⭐ 最全面的开源 TTS 工具箱 |
| [Piper TTS](https://github.com/rhasspy/piper) | ![GitHub Repo stars](https://badgen.net/github/stars/rhasspy/piper) | Fast, local neural TTS. Real-time synthesis with low resource usage. | 实时合成，低资源占用 |
| [Silero Models](https://github.com/snakers4/silero-models) | ![GitHub Repo stars](https://badgen.net/github/stars/snakers4/silero-models) | Pre-trained text-to-speech models made embarrassingly simple. Multi-language support. | 简单易用，高质量 |

### Commercial TTS APIs | 商业 TTS 服务

| Name | Description | Notes |
|------|-------------|-------|
| [ElevenLabs](https://elevenlabs.io/) | High-quality AI voice generation. Ultra-realistic speech, voice cloning, multi-language support. | 最高质量的商业 TTS |
| [OpenAI TTS](https://platform.openai.com/docs/guides/text-to-speech) | OpenAI's text-to-speech API. High-quality, low-latency, multiple voice options. | 高质量低延迟 |
| [Azure Speech Services](https://azure.microsoft.com/products/ai-services/text-to-speech) | Microsoft TTS with neural voices. Custom voice creation, SSML support. | 神经语音，自定义音色 |
| [Cartesia](https://cartesia.ai/) | Real-time streaming TTS. Ultra-low latency, natural intonation. | 超低延迟流式 TTS |
| [Deepgram Aura](https://deepgram.com/aura) | Real-time text-to-speech. Conversational voice quality. | 对话式语音，低延迟 |

---

## Developer Communities & Resources | 开发者社区与资源

### Communities | 社区平台

| Name | Description | Notes |
|------|-------------|-------|
| [RTE Community](https://www.rtecommunity.dev/) | Real-Time Engagement developer community. Technical articles, developer exchange, best practices. | 实时互动技术开发者社区 |
| [Voice Agent Knowledge Base (Feishu)](https://realtime.feishu.cn/docx/FFcedfbkNoNA3OxeD2IcdRWbnLf) | Comprehensive Voice Agent knowledge base in Chinese. Systematic tutorials, practical experience. | Voice Agent 中文知识库 |

### Platforms & Tools | 开发平台与工具

| Name | Description | Notes |
|------|-------------|-------|
| [Vapi](https://vapi.ai/) | Platform for quickly building voice AI agents. Low-code, rich integrations, telephony support. | 低代码快速构建平台 |
| [Retell AI](https://www.retellai.com/) | Conversational AI platform with enterprise-grade turn-taking management. | 企业级话轮管理 |
| [Tavus](https://www.tavus.io/) | Real-time conversational video API. Transformer-based turn detection, multimodal video+voice. | 视频+语音多模态 |

### Technical Blogs & Documentation | 技术博客与文档

| Name | Description | Notes |
|------|-------------|-------|
| [Voice AI & Voice Agents Primer](https://voiceaiandvoiceagents.com/) | Comprehensive illustrated guide to voice AI. Architecture design, technical overview, best practices. | 全面的语音 AI 图解指南 |
| [AssemblyAI Blog: Turn Detection](https://www.assemblyai.com/blog/turn-detection-endpointing-voice-agent) | In-depth analysis of turn detection. Algorithm comparison, latency analysis. | 话轮检测深度解析 |
| [LiveKit Blog: Transformer Turn Detection](https://blog.livekit.io/using-a-transformer-to-improve-end-of-turn-detection/) | Using transformers to improve endpointing. Technical details, performance comparison. | Transformer 改进端点检测 |
| [Krisp Blog: Turn-Taking](https://krisp.ai/blog/improving-turn-taking-of-ai-voice-agents-with-background-voice-cancellation/) | Background noise cancellation improves turn-taking. Evaluation and results. | 背景噪音消除改善话轮 |
| [Speechmatics: Semantic Turn Detection](https://blog.speechmatics.com/semantic-turn-detection) | Semantic turn detection with SLM. Implementation guide, threshold tuning. | 使用 SLM 的语义话轮检测 |
| [Agora: TEN VAD & Turn Detection](https://www.agora.io/en/blog/making-voice-ai-agents-more-human-with-ten-vad-and-turn-detection/) | Making voice agents more human with TEN VAD and Turn Detection. | TEN 的 VAD 和话轮检测 |

## Related Awesome Lists | 相关资源

- [awesome-voice-conversion](https://github.com/JeffC0628/awesome-voice-conversion)
- [awesome-ai-agents](https://github.com/e2b-dev/awesome-ai-agents)

---

## License | 许可证

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the contributors have waived all copyright and related rights to this work.

---

## Acknowledgments | 致谢

Thanks to all open-source contributors making voice AI technology more accessible and powerful!

If this list helps you, please give it a ⭐️!

---

**Maintainer | 维护者: 云中江树**  
**WeChat | 微信: 1796060717** (加入 Voice Agent 交流群)  

Welcome to exchange and discuss Voice Agent technology through Issues or PRs!  
欢迎通过 Issues 或 PR 交流讨论 Voice Agent 相关技术！