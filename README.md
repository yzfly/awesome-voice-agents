# Awesome Voice Agents [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of voice AI agent frameworks, tools, resources, and best practices | 精选的语音 AI Agent 框架、工具、资源和最佳实践

Welcome to **Awesome Voice Agents**! This is a carefully curated collection of resources related to voice AI agents, covering core technologies such as endpoint detection, turn-taking management, real-time speech recognition, and speech synthesis.

本项目精心收录语音 AI Agent 相关的优质资源，涵盖端点检测、话轮管理、实时语音识别、语音合成等核心技术。

**Maintainer | 维护者: 云中江树**（微信公众号: 云中江树）

💬 **Connect | 交流**  
Add WeChat | 添加江树微信: **1796060717**  
欢迎 Voice Agent 从业者和爱好者加微信交流！

---

## Contents | 目录

- [Frameworks & Platforms | 框架与平台](#frameworks--platforms--框架与平台)
- [VAD (Voice Activity Detection) | 语音活动检测](#vad-voice-activity-detection--语音活动检测)
- [Turn Detection & Endpointing | 话轮检测与端点检测](#turn-detection--endpointing--话轮检测与端点检测)
- [STT (Speech-to-Text) | 语音转文本](#stt-speech-to-text--语音转文本)
- [TTS (Text-to-Speech) | 文本转语音](#tts-text-to-speech--文本转语音)
- [End-to-End Speech Models | 端到端语音模型](#end-to-end-speech-models--端到端语音模型)
- [Voice MCP & Coding Agent Voice | 语音 MCP 与编程 Agent 语音](#voice-mcp--coding-agent-voice--语音-mcp-与编程-agent-语音)
- [Toolkits, Wake Word & Voice Conversion | 语音工具箱, 唤醒词与变声](#toolkits-wake-word--voice-conversion--语音工具箱-唤醒词与变声)
- [Developer Communities & Resources | 开发者社区与资源](#developer-communities--resources--开发者社区与资源)
- [Learning Resources | 学习资源](#learning-resources--学习资源)
- [Related Awesome Lists | 相关资源](#related-awesome-lists--相关资源)
- [Contributing | 贡献指南](#contributing--贡献指南)
- [License | 许可证](#license--许可证)
- [Acknowledgments | 致谢](#acknowledgments--致谢)

---

## Frameworks & Platforms | 框架与平台

### Comprehensive Frameworks | 综合性框架

| Name | Stars | Description | Notes |
|------|-------|-------------|-------|
| [TEN Framework](https://github.com/TEN-framework/ten-framework) | ![GitHub Repo stars](https://badgen.net/github/stars/TEN-framework/ten-framework) | Open-source framework for conversational voice AI agents with multimodal capabilities (voice, vision, avatar). Low-latency, high-quality real-time assistant. | 支持多模态，低延迟高质量。[Demo](https://agent.theten.ai/) |
| [Pipecat](https://github.com/pipecat-ai/pipecat) | ![GitHub Repo stars](https://badgen.net/github/stars/pipecat-ai/pipecat) | Open Source framework for voice and multimodal conversational AI. Modular design with support for multiple STT, LLM, TTS services. | 模块化设计，支持多平台 SDK |
| [LiveKit Agents](https://github.com/livekit/agents) | ![GitHub Repo stars](https://badgen.net/github/stars/livekit/agents) | Powerful framework for building realtime voice AI agents. Fully open-source, WebRTC support, built-in semantic turn detection. | 完全开源，内置语义话轮检测 |
| [Vision Agents](https://github.com/GetStream/Vision-Agents) | ![GitHub Repo stars](https://badgen.net/github/stars/GetStream/Vision-Agents) | Open framework for low-latency voice and vision AI agents. Pluggable STT/LLM/TTS plus realtime video understanding, provider-agnostic with WebRTC edge transport. | GetStream 出品，低延迟语音+视觉智能体框架 |
| [OpenAI Realtime Agents](https://github.com/openai/openai-realtime-agents) | ![GitHub Repo stars](https://badgen.net/github/stars/openai/openai-realtime-agents) | Advanced agentic patterns built on OpenAI Realtime API. Multi-agent collaboration, handoffs, tool use. | OpenAI 官方示例，支持多 Agent |
| [openai-agents-js](https://github.com/openai/openai-agents-js) | ![GitHub Repo stars](https://badgen.net/github/stars/openai/openai-agents-js) | A lightweight, powerful framework for multi-agent workflows and voice agents. | OpenAI 官方示例，支持多 Agent 和语音Agent |
| [call-center-ai](https://github.com/microsoft/call-center-ai) | ![GitHub Repo stars](https://badgen.net/github/stars/microsoft/call-center-ai) | Send a phone call from AI agent, in an API call. Or, directly call the bot from the configured phone number! | 基于 Azure 和 OpenAI GPT 的 AI 驱动呼叫中心解决方案。|
| [Vocode Core](https://github.com/vocodedev/vocode-core) | ![GitHub Repo stars](https://badgen.net/github/stars/vocodedev/vocode-core) | Build voice-based LLM agents. Modular and open source. Real-time streaming conversations. | 支持电话、Zoom 等场景部署 |
| [Bolna](https://github.com/bolna-ai/bolna) | ![GitHub Repo stars](https://badgen.net/github/stars/bolna-ai/bolna) | End-to-end open source production-ready voice agents platform. Build voice assistants through JSON config. | 生产就绪，支持 Twilio/Plivo |
| [LLMRTC](https://github.com/llmrtc/llmrtc) | ![GitHub Repo stars](https://badgen.net/github/stars/llmrtc/llmrtc) | Open-source WebRTC orchestration SDK. Handles server-side VAD, barge-in, and multi-provider switching. | **WebRTC-based**, **Low Latency**. Infrastructure-agnostic. |
| [Ultravox](https://github.com/fixie-ai/ultravox) | ![GitHub Repo stars](https://badgen.net/github/stars/fixie-ai/ultravox) | Fast multimodal LLM for real-time voice. Understands speech directly without a separate STT step, low time-to-first-token. | 直接理解语音，无需独立 STT，首字延迟低 |
| [Unmute (Kyutai)](https://github.com/kyutai-labs/unmute) | ![GitHub Repo stars](https://badgen.net/github/stars/kyutai-labs/unmute) | Modular pipeline (Kyutai STT + any LLM + Kyutai TTS) that turns any text LLM into a low-latency voice agent. Docker + vLLM composable. | Kyutai 出品，把任意文本 LLM 包成实时语音体 |
| [FastRTC](https://github.com/gradio-app/fastrtc) | ![GitHub Repo stars](https://badgen.net/github/stars/gradio-app/fastrtc) | Turn any Python function into a real-time WebRTC/WebSocket audio-video stream. Built-in VAD, turn-taking, STT/TTS, even a free temp phone number. | HuggingFace 生态，几行代码搞定实时语音流 |
| [Speaches](https://github.com/speaches-ai/speaches) | ![GitHub Repo stars](https://badgen.net/github/stars/speaches-ai/speaches) | "Ollama for TTS/STT": OpenAI-API-compatible self-hosted server (faster-whisper + Kokoro/Piper) with a `/v1/realtime` WebSocket endpoint. | 自托管语音服务器，兼容 OpenAI API，全本地 |
| [Gabber](https://github.com/gabber-dev/gabber) | ![GitHub Repo stars](https://badgen.net/github/stars/gabber-dev/gabber) | Source-available engine for real-time multimodal agents that see, hear, and speak. React/Python/Unity SDKs. | 实时多模态智能体引擎，可看可听可说 |
| [Dograh](https://github.com/dograh-hq/dograh) | ![GitHub Repo stars](https://badgen.net/github/stars/dograh-hq/dograh) | Self-hosted open-source Vapi/Retell alternative with drag-and-drop visual workflow builder, BYOK, MCP-native and telephony built in. | 自托管的可视化拖拽语音流程编排，自带电话与 MCP |
| [huggingface/speech-to-speech](https://github.com/huggingface/speech-to-speech) | ![GitHub Repo stars](https://badgen.net/github/stars/huggingface/speech-to-speech) | Modular STT→LLM→TTS pipeline to build local voice agents entirely from open-source models. | 用开源模型搭本地语音 Agent 流水线 |
| [Rasa](https://github.com/RasaHQ/rasa) | ![GitHub Repo stars](https://badgen.net/github/stars/RasaHQ/rasa) | Mature open-source NLU + dialogue-management framework (now with the LLM-driven CALM engine) for text and voice assistants. | 老牌开源对话框架，CALM 引擎结合 LLM 与业务逻辑 |
| [Rapida voice-ai](https://github.com/rapidaai/voice-ai) | ![GitHub Repo stars](https://badgen.net/github/stars/rapidaai/voice-ai) | End-to-end voice orchestration platform connecting STT, LLM and TTS providers for building and deploying production voice agents. | 端到端语音编排平台，串联 STT/LLM/TTS 部署生产级语音 Agent |
| [Patter](https://github.com/PatterAI/Patter) | ![GitHub Repo stars](https://badgen.net/github/stars/PatterAI/Patter) | Open-source voice AI SDK for building real-time conversational voice agents with pluggable speech pipelines. | 开源语音 AI SDK，可插拔语音流水线构建实时对话 Agent |
| [EchoKit Server](https://github.com/second-state/echokit_server) | ![GitHub Repo stars](https://badgen.net/github/stars/second-state/echokit_server) | Open-source voice agent server connecting STT, LLM and TTS for the EchoKit hardware and any client; configurable, self-hostable. | 开源语音 Agent 服务端，串联 STT/LLM/TTS，可自托管 |

### Specialized Solutions | 专用解决方案

| Name | Stars | Description | Notes |
|------|-------|-------------|-------|
| [BentoVoiceAgent](https://github.com/bentoml/BentoVoiceAgent) | ![GitHub Repo stars](https://badgen.net/github/stars/bentoml/BentoVoiceAgent) | Build phone calling voice agents fully powered by open source models. Uses BentoML for deployment. | 完全基于开源模型 |
| [LangGraph Voice Agent](https://github.com/Rajathbharadwaj/voice-agent) | ![GitHub Repo stars](https://badgen.net/github/stars/Rajathbharadwaj/voice-agent) | Voice AI SDR Agent for automated sales calls. Built with LangGraph, Twilio, and OpenAI. Production-ready with call routing, objection handling, and appointment scheduling. | LangGraph 架构，销售自动化 |
| [RealtimeVoiceChat](https://github.com/KoljaB/RealtimeVoiceChat) | ![GitHub Repo stars](https://badgen.net/github/stars/KoljaB/RealtimeVoiceChat) | Browser-to-Python stack for ~500ms natural spoken conversation with local LLMs (Ollama). Built on RealtimeSTT + RealtimeTTS. | 本地语音对话栈，约 500ms 延迟 |
| [react-voice-agent](https://github.com/langchain-ai/react-voice-agent) | ![GitHub Repo stars](https://badgen.net/github/stars/langchain-ai/react-voice-agent) | LangChain official example wiring the OpenAI Realtime API into a tool-using ReAct-style voice agent over WebSockets. | LangChain 官方 React 风格语音 Agent 示例，接入 OpenAI Realtime API |

### Commercial Speech-to-Speech Platforms | 商业语音平台

| Name | Description | Notes |
|------|-------------|-------|
| [Hume EVI](https://www.hume.ai/empathic-voice-interface) | Empathic speech-to-speech foundation model (EVI 3) that reads and responds to emotion/prosody. 100,000+ customizable voices. | 共情语音模型，感知并回应情绪语调 |
| [Amazon Nova Sonic](https://aws.amazon.com/ai/generative-ai/nova/) | AWS Bedrock speech-to-speech foundation model with polyglot voices, async tool calling, large context, LiveKit/Pipecat integrations. | AWS 语音到语音大模型，多语种同声、异步工具调用 |
| [Speechmatics Flow](https://www.speechmatics.com/flow) | Conversational voice-agent API built on high-accuracy multilingual ASR with sentiment/tone awareness. | 基于高精度多语种 ASR 的对话语音 Agent API |
| [Agora Conversational AI Engine](https://www.agora.io/en/products/conversational-ai-engine/) | Real-time RTC platform orchestrating ASR + any LLM + TTS for global low-latency voice agents. | 全球实时通信厂商的语音 Agent 引擎，低延迟 |
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
| [WhisperLiveKit](https://github.com/QuentinFuxa/WhisperLiveKit) | ![GitHub Repo stars](https://badgen.net/github/stars/QuentinFuxa/WhisperLiveKit) | Real-time, fully local speech-to-text with speaker diarization; web UI plus FastAPI server, built on SimulStreaming/WhisperStreaming. | 同步实时语音转文字，含说话人分离，全本地可部署 |
| [Whisper Streaming (UFAL)](https://github.com/ufal/whisper_streaming) | ![GitHub Repo stars](https://badgen.net/github/stars/ufal/whisper_streaming) | Whisper realtime streaming for long speech-to-text. Local agreement policy with self-adaptive latency. 3.3s latency. | 使用局部一致性策略，自适应延迟 |
| [WhisperLive](https://github.com/collabora/WhisperLive) | ![GitHub Repo stars](https://badgen.net/github/stars/collabora/WhisperLive) | Nearly-live implementation of OpenAI's Whisper. TensorRT acceleration support. Browser extensions and iOS client. | 支持 TensorRT 加速和多平台 |
| [Whisper Real Time](https://github.com/davabase/whisper_real_time) | ![GitHub Repo stars](https://badgen.net/github/stars/davabase/whisper_real_time) | Real time transcription with OpenAI Whisper. Continuously records and concatenates audio. | 简单易用的实时转录演示 |
| [VoiceStreamAI](https://github.com/alesaccoia/VoiceStreamAI) | ![GitHub Repo stars](https://badgen.net/github/stars/alesaccoia/VoiceStreamAI) | Near-realtime audio transcription using self-hosted Whisper and WebSocket. Supports Faster Whisper, integrated VAD. | WebSocket 架构，分块处理策略 |
| [speech-to-text (reriiasu)](https://github.com/reriiasu/speech-to-text) | ![GitHub Repo stars](https://badgen.net/github/stars/reriiasu/speech-to-text) | Real-time transcription using faster-whisper. HTML GUI with WebSocket support. SRT subtitle generation. | 提供 GUI，支持字幕生成 |
| [Whispering](https://github.com/shirayu/whispering) | ![GitHub Repo stars](https://badgen.net/github/stars/shirayu/whispering) | Streaming transcriber with whisper. Client-server architecture support. | 支持客户端-服务器架构（已归档）|

### Open Source STT Models | 开源 STT 模型

| Name | Stars | Description | Notes |
|------|-------|-------------|-------|
| [DeepSpeech](https://github.com/mozilla/DeepSpeech) | ![GitHub Repo stars](https://badgen.net/github/stars/mozilla/DeepSpeech) | Open-source speech-to-text engine that runs offline and in real time on-device, from embedded to server. | Mozilla 开源离线设备端实时 STT 引擎（已停维护）|
| [faster-whisper](https://github.com/SYSTRAN/faster-whisper) | ![GitHub Repo stars](https://badgen.net/github/stars/SYSTRAN/faster-whisper) | Faster Whisper transcription with CTranslate2. Up to 4x faster than openai/whisper with less memory. INT8 quantization support. | ⭐ 工业级首选，4 倍加速，低内存 |
| [NVIDIA Parakeet](https://huggingface.co/nvidia/parakeet-tdt-0.6b-v2) | - | 600M-param FastConformer ASR model. Top of Hugging Face Open ASR leaderboard, accurate word-level timestamps, transcribes 60-min audio in one pass. | 准确率领先，长音频高效转录 |
| [Moonshine](https://github.com/usefulsensors/moonshine) | ![GitHub Repo stars](https://badgen.net/github/stars/usefulsensors/moonshine) | Fast and accurate speech recognition optimized for on-device and edge. Variable-length input, lower latency than Whisper on short audio. | 端侧优化，短音频低延迟 |
| [Kyutai STT](https://github.com/kyutai-labs/delayed-streams-modeling) | ![GitHub Repo stars](https://badgen.net/github/stars/kyutai-labs/delayed-streams-modeling) | Streaming-native STT (Delayed Streams Modeling); ~0.5s delay + semantic VAD, word-level timestamps, ~400 streams on one H100. Rust + MLX. | Kyutai 出品，专为实时语音代理设计的流式 ASR |
| [NVIDIA NeMo](https://github.com/NVIDIA-NeMo/NeMo) | ![GitHub Repo stars](https://badgen.net/github/stars/NVIDIA-NeMo/NeMo) | Scalable speech/LLM framework, home of Parakeet (tops HF Open-ASR leaderboard) and Canary; cache-aware chunked streaming, multilingual. | 英伟达语音框架，Parakeet/Canary 的训练部署基座 |
| [FunASR](https://github.com/modelscope/FunASR) | ![GitHub Repo stars](https://badgen.net/github/stars/modelscope/FunASR) | Alibaba industrial toolkit hosting Paraformer (non-autoregressive, ~120x real-time) with streaming, VAD, punctuation, diarization, 50+ languages. | 阿里达摩院工业级 ASR，中文效果强，支持流式 |
| [SenseVoice](https://github.com/FunAudioLLM/SenseVoice) | ![GitHub Repo stars](https://badgen.net/github/stars/FunAudioLLM/SenseVoice) | Multilingual (50+ langs) ASR + emotion recognition + audio-event detection; non-autoregressive Small is ~15x faster than Whisper-large-v3. | 多语种语音理解，识别+情感+事件三合一 |
| [whisper.cpp](https://github.com/ggml-org/whisper.cpp) | ![GitHub Repo stars](https://badgen.net/github/stars/ggml-org/whisper.cpp) | Plain C/C++ Whisper inference via ggml; zero-dependency, runs CPU/Metal/CUDA/Core ML. Ideal for on-device and low-latency local agents. | 纯 C/C++ Whisper 推理，零依赖跨平台，CPU 也能跑 |
| [WhisperX](https://github.com/m-bain/whisperX) | ![GitHub Repo stars](https://badgen.net/github/stars/m-bain/whisperX) | Whisper + wav2vec2 forced alignment for accurate word-level timestamps, plus speaker diarization and VAD batching (70x real-time). | Whisper 加对齐，精确词级时间戳+说话人分离 |
| [Distil-Whisper](https://github.com/huggingface/distil-whisper) | ![GitHub Repo stars](https://badgen.net/github/stars/huggingface/distil-whisper) | Distilled Whisper-large-v3, 6x faster and ~50% smaller within 1% WER. Good low-latency English choice. | HuggingFace 蒸馏版 Whisper，速度快 6 倍 |

### Commercial STT APIs | 商业 STT 服务

| Name | Description | Notes |
|------|-------------|-------|
| [OpenAI Whisper API](https://platform.openai.com/docs/guides/speech-to-text) | Cloud-based Whisper API. Easy integration, pay-as-you-go pricing. | 云端 Whisper，按需付费 |
| [Azure Speech Services](https://azure.microsoft.com/products/ai-services/speech-to-text) | Microsoft's STT service. Multi-language support, custom model training. | 支持多语言，自定义模型 |
| [Deepgram](https://deepgram.com/) | Enterprise-grade real-time STT API. Ultra-low latency, streaming transcription. | 超低延迟，流式转录 |
| [AssemblyAI](https://www.assemblyai.com/) | Speech AI API with Universal-Streaming model. Immutable transcription, intelligent endpointing. | 不可变转录，智能端点检测 |
| [Speechmatics](https://www.speechmatics.com/) | Real-time ASR (Ursa 2) with sub-1s latency, strong accent/multilingual robustness, on-prem options. | 企业级实时 ASR，口音鲁棒，支持私有化 |
| [Groq Whisper](https://groq.com/) | Whisper-large-v3/-turbo served on Groq LPUs for ultra-low-latency, very high-throughput transcription/translation. | Groq LPU 跑 Whisper，超低延迟高吞吐 |

---

## TTS (Text-to-Speech) | 文本转语音

### Open Source TTS Models | 开源 TTS 模型

| Name | Stars | Description | Notes |
|------|-------|-------------|-------|
| [Voicebox](https://github.com/jamiepine/voicebox) | ![GitHub Repo stars](https://badgen.net/github/stars/jamiepine/voicebox) | Local-first open-source voice cloning & synthesis studio. 5 TTS engines, 23 languages, timeline editor, REST API. Open-source ElevenLabs alternative. | ⭐ 本地优先，支持声音克隆、多轨编辑、后处理音效。[官网](https://voicebox.sh) |
| [GPT-SoVITS](https://github.com/RVC-Boss/GPT-SoVITS) | ![GitHub Repo stars](https://badgen.net/github/stars/RVC-Boss/GPT-SoVITS) | Few-shot voice cloning TTS. High-quality synthesis. | 少样本语音克隆 |
| [Bark](https://github.com/suno-ai/bark) | ![GitHub Repo stars](https://badgen.net/github/stars/suno-ai/bark) | Transformer-based TTS model. Generates highly realistic audio including music, sound effects. | 可生成音乐和音效 |
| [Coqui TTS](https://github.com/coqui-ai/TTS) | ![GitHub Repo stars](https://badgen.net/github/stars/coqui-ai/TTS) | Deep learning TTS toolkit. 1100+ pre-trained models. Voice cloning support. | 全面的开源 TTS 工具箱（已停官方维护）|
| [Piper TTS](https://github.com/rhasspy/piper) | ![GitHub Repo stars](https://badgen.net/github/stars/rhasspy/piper) | Fast, local neural TTS. Real-time synthesis with low resource usage. | 实时合成，低资源占用 |
| [Silero Models](https://github.com/snakers4/silero-models) | ![GitHub Repo stars](https://badgen.net/github/stars/snakers4/silero-models) | Pre-trained text-to-speech models made embarrassingly simple. Multi-language support. | 简单易用，高质量 |
| [Kokoro](https://github.com/hexgrad/kokoro) | ![GitHub Repo stars](https://badgen.net/github/stars/hexgrad/kokoro) | Open-weight 82M-param TTS model. Lightweight yet high quality, fast and cost-efficient, Apache-licensed. | ⭐ 轻量高质量，推理快成本低 |
| [CosyVoice](https://github.com/FunAudioLLM/CosyVoice) | ![GitHub Repo stars](https://badgen.net/github/stars/FunAudioLLM/CosyVoice) | Multilingual large voice generation model from Alibaba FunAudioLLM. Zero-shot voice cloning, streaming inference, fine-grained control. | 阿里出品，零样本克隆，流式推理 |
| [Fish-Speech](https://github.com/fishaudio/fish-speech) | ![GitHub Repo stars](https://badgen.net/github/stars/fishaudio/fish-speech) | SOTA open-source multilingual TTS. Zero-shot and few-shot voice cloning, low latency, no phoneme dependency. | 多语言，零样本克隆，低延迟 |
| [F5-TTS](https://github.com/SWivid/F5-TTS) | ![GitHub Repo stars](https://badgen.net/github/stars/SWivid/F5-TTS) | Fairytaler that fakes fluent and faithful speech with flow matching. Fast, high-quality zero-shot voice cloning. | 基于 flow matching，零样本克隆 |
| [ChatTTS](https://github.com/2noise/ChatTTS) | ![GitHub Repo stars](https://badgen.net/github/stars/2noise/ChatTTS) | Generative TTS model optimized for dialogue scenarios. Natural conversational prosody, fine-grained prosodic control. | 对话场景优化，自然韵律 |
| [VoiceCraft](https://github.com/jasonppy/VoiceCraft) | ![GitHub Repo stars](https://badgen.net/github/stars/jasonppy/VoiceCraft) | Token-infilling neural codec model for zero-shot speech editing and TTS in the wild; clones a voice from a few seconds of reference audio. | 野外环境零样本语音编辑与 TTS，几秒参考音频即可克隆 |
| [Chatterbox](https://github.com/resemble-ai/chatterbox) | ![GitHub Repo stars](https://badgen.net/github/stars/resemble-ai/chatterbox) | Resemble AI MIT-licensed TTS; Turbo variant ~75ms latency, 5-second voice cloning, emotion-exaggeration control, 23-language variant. | Resemble AI，MIT，75ms 超低延迟，5 秒克隆 |
| [Orpheus TTS](https://github.com/canopyai/Orpheus-TTS) | ![GitHub Repo stars](https://badgen.net/github/stars/canopyai/Orpheus-TTS) | Llama-3B-based emotive TTS with ~200ms (down to ~100ms) streaming latency, zero-shot cloning, emotion/intonation tags. | Canopy Labs，Llama 架构，~200ms 流式低延迟 |
| [IndexTTS2](https://github.com/index-tts/index-tts) | ![GitHub Repo stars](https://badgen.net/github/stars/index-tts/index-tts) | Bilibili industrial zero-shot TTS, first AR model with precise duration control plus disentangled emotion/timbre control. | B站出品，工业级零样本+时长控制+情感音色解耦 |
| [Spark-TTS](https://github.com/SparkAudio/Spark-TTS) | ![GitHub Repo stars](https://badgen.net/github/stars/SparkAudio/Spark-TTS) | Efficient 0.5B LLM-based single-stream TTS (BiCodec tokens); zero-shot cloning plus controllable speaker creation. | 单流 BiCodec+Qwen2.5，高效零样本克隆 |
| [Higgs Audio v2](https://github.com/boson-ai/higgs-audio) | ![GitHub Repo stars](https://badgen.net/github/stars/boson-ai/higgs-audio) | Boson AI 3B foundation model (10M+ hrs); expressive multi-speaker dialogue, multilingual, voice cloning, can add background music. | Boson AI 音频基座，多说话人对话，表现力极强 |
| [MegaTTS 3](https://github.com/bytedance/MegaTTS3) | ![GitHub Repo stars](https://badgen.net/github/stars/bytedance/MegaTTS3) | ByteDance lightweight (0.45B DiT) Apache-2.0 TTS; ultra-high-quality zero-shot cloning, Chinese/English code-switching. | 字节跳动，轻量 DiT，高质量中英零样本克隆 |
| [Dia](https://github.com/nari-labs/dia) | ![GitHub Repo stars](https://badgen.net/github/stars/nari-labs/dia) | Nari Labs 1.6B model generating ultra-realistic multi-speaker dialogue in one pass with nonverbals (laughter, coughs). | Nari Labs，一次生成超真实多角色对话 |
| [MeloTTS](https://github.com/myshell-ai/MeloTTS) | ![GitHub Repo stars](https://badgen.net/github/stars/myshell-ai/MeloTTS) | MyShell MIT-licensed multilingual library (EN/ES/FR/ZH/JA/KO), fast enough for CPU real-time inference. | MyShell，MIT，多语种 CPU 实时推理 |
| [StyleTTS 2](https://github.com/yl4579/StyleTTS2) | ![GitHub Repo stars](https://badgen.net/github/stars/yl4579/StyleTTS2) | Style-diffusion + adversarial TTS reaching human-level quality and zero-shot speaker adaptation; a foundational OSS model. | 风格扩散+对抗训练达到人类水平，众多项目底座 |
| [Parler-TTS](https://github.com/huggingface/parler-tts) | ![GitHub Repo stars](https://badgen.net/github/stars/huggingface/parler-tts) | Hugging Face fully-open controllable TTS where voice traits (gender, pitch, rate, reverb) are set via a text description prompt. | HuggingFace 全开源，自然语言描述控制音色 |

### Commercial TTS APIs | 商业 TTS 服务

| Name | Description | Notes |
|------|-------------|-------|
| [ElevenLabs](https://elevenlabs.io/) | High-quality AI voice generation. Ultra-realistic speech, voice cloning, multi-language support. | 最高质量的商业 TTS |
| [PHANTOM VOICES](https://auto-business-agent.replit.app/portfolio) | 10 free professional AI voice clones via public REST API. Zero-cost, 29 platform configs (Vapi, Retell, Bland, LangChain, HeyGen, etc). AI-powered recommendation endpoint. Multilingual (9+ languages). | 免费专业 AI 语音克隆 API |
| [OpenAI TTS](https://platform.openai.com/docs/guides/text-to-speech) | OpenAI's text-to-speech API. High-quality, low-latency, multiple voice options. | 高质量低延迟 |
| [Azure Speech Services](https://azure.microsoft.com/products/ai-services/text-to-speech) | Microsoft TTS with neural voices. Custom voice creation, SSML support. | 神经语音，自定义音色 |
| [Cartesia](https://cartesia.ai/) | Real-time streaming TTS. Ultra-low latency, natural intonation. | 超低延迟流式 TTS |
| [Deepgram Aura-2](https://deepgram.com/product/text-to-speech) | Real-time text-to-speech. Conversational voice quality. | 对话式语音，低延迟 |
| [voicetoinstrument.com](https://voicetoinstrument.com) | Convert voice to instrumental tracks using AI. Separate vocals and convert to instrument versions. | 语音转乐器音轨 |
| [Hume AI Octave](https://www.hume.ai/) | First LLM-based "speech-language" TTS that understands context to set emotion/cadence; voice design from prompts. | 首个理解语义的 LLM-TTS，情感表现力强 |
| [MiniMax (Hailuo) Speech](https://www.minimax.io/audio) | Speech-02/2.5/2.6 series, 40+ languages, 100+ voices + cloning; topped Speech Arena above OpenAI/ElevenLabs. | MiniMax 海螺，40+ 语种，多榜单第一 |
| [Rime](https://rime.ai/) | Enterprise TTS for real-time voice agents; Mist v2 ~70-225ms TTFA, Arcana v2 for expressive paralinguistic voices. | 主打实时语音 Agent，极低延迟，发音确定性强 |
| [PlayAI (PlayHT)](https://play.ai/) | Conversational-AI-focused API; Play 3.0 Mini ~143ms TTFB multilingual streaming, PlayDialog for two-speaker dialogue. | 面向对话 AI，低延迟流式，双人对话 |

---

## End-to-End Speech Models | 端到端语音模型

End-to-end speech models process audio input and produce audio output directly, without separate STT/LLM/TTS pipelines, enabling lower latency and richer paralinguistic understanding.

端到端语音模型直接处理音频输入并输出音频，无需 STT/LLM/TTS 串联流水线，可实现更低延迟和更丰富的副语言理解。这是 Voice Agent 的前沿方向。

### Speech-to-Speech & Full-Duplex Models | 语音对话与全双工模型

| Name | Stars | Description | Notes |
|------|-------|-------------|-------|
| [Moshi](https://github.com/kyutai-labs/moshi) | ![GitHub Repo stars](https://badgen.net/github/stars/kyutai-labs/moshi) | Full-duplex speech-text foundation model from Kyutai. Real-time dialogue with theoretical ~160ms latency, listens and speaks simultaneously. | ⭐ 全双工实时对话，超低延迟 |
| [Qwen3-Omni](https://github.com/QwenLM/Qwen3-Omni) | ![GitHub Repo stars](https://badgen.net/github/stars/QwenLM/Qwen3-Omni) | Alibaba's latest natively end-to-end omni-modal LLM (text/audio/image/video in, text+speech out). 119 text languages, ~211ms audio latency, Apache 2.0. | 阿里最新原生全模态大模型，多语种实时语音生成 |
| [Qwen2.5-Omni](https://github.com/QwenLM/Qwen2.5-Omni) | ![GitHub Repo stars](https://badgen.net/github/stars/QwenLM/Qwen2.5-Omni) | End-to-end multimodal model from Alibaba. Perceives text, image, audio, video and generates text and natural speech in streaming. | 阿里全模态，Thinker-Talker 架构，流式语音生成 |
| [GLM-4-Voice](https://github.com/zai-org/GLM-4-Voice) | ![GitHub Repo stars](https://badgen.net/github/stars/zai-org/GLM-4-Voice) | End-to-end Chinese-English speech model from Zhipu. Low-latency conversation, controllable emotion, tone, speed and dialect. Apache 2.0. | 智谱出品，中英双语，情感语速方言可控 |
| [NVIDIA PersonaPlex](https://github.com/NVIDIA/personaplex) | ![GitHub Repo stars](https://badgen.net/github/stars/NVIDIA/personaplex) | Real-time full-duplex speech-to-speech model that listens and talks simultaneously, with persona control via text role prompts + audio voice conditioning. Code MIT, weights NVIDIA Open Model License. Backbone of Nemotron 3 VoiceChat (#1 open full-duplex model on VoiceBench). | ⭐ 英伟达开源全双工 speech-to-speech 模型，边听边说+人设控制 |
| [Step-Audio 2](https://github.com/stepfun-ai/Step-Audio2) | ![GitHub Repo stars](https://badgen.net/github/stars/stepfun-ai/Step-Audio2) | End-to-end speech-to-speech MLLM from StepFun; open Step-Audio-2-mini (8B, Apache 2.0) with CoT-RL and paralinguistic reasoning, reportedly surpassing GPT-4o-Audio. | 阶跃星辰，全开源 8B 语音对话模型，支持副语言推理 |
| [Kimi-Audio](https://github.com/MoonshotAI/Kimi-Audio) | ![GitHub Repo stars](https://badgen.net/github/stars/MoonshotAI/Kimi-Audio) | Open 7B audio foundation model from Moonshot AI for ASR, audio QA, captioning, emotion recognition and end-to-end speech conversation. 13M+ hours pretraining. | 月之暗面通用音频基座，理解+对话一体 |
| [LLaMA-Omni2](https://github.com/ictnlp/LLaMA-Omni2) | ![GitHub Repo stars](https://badgen.net/github/stars/ictnlp/LLaMA-Omni2) | Real-time SpeechLM series (0.5B-14B) on Qwen2.5 with autoregressive streaming speech decoder; ~583ms latency. ACL 2025. | 中科院计算所，自回归流式语音合成，数据极省 |
| [Mini-Omni2](https://github.com/gpt-omni/mini-omni2) | ![GitHub Repo stars](https://badgen.net/github/stars/gpt-omni/mini-omni2) | Open GPT-4o-style omni model with vision+speech+duplex; real-time speech-to-speech with interruption, no external ASR/TTS. | 开源版 GPT-4o，支持视觉+语音+打断 |
| [VITA-Audio](https://github.com/VITA-MLLM/VITA-Audio) | ![GitHub Repo stars](https://badgen.net/github/stars/VITA-MLLM/VITA-Audio) | Fast interleaved cross-modal token generation; first-audio-token latency to 53ms, 3-5x speedup at 7B. NeurIPS 2025. | 首 token 仅 53ms，3-5 倍加速，全开源数据训练 |
| [Freeze-Omni](https://github.com/VITA-MLLM/Freeze-Omni) | ![GitHub Repo stars](https://badgen.net/github/stars/VITA-MLLM/Freeze-Omni) | Low-latency speech-to-speech with a frozen text LLM backbone (avoids catastrophic forgetting); chunk-wise streaming. ICML 2025. | 冻结 LLM 主干避免知识遗忘，低延迟流式对话 |
| [Baichuan-Audio](https://github.com/baichuan-inc/Baichuan-Audio) | ![GitHub Repo stars](https://badgen.net/github/stars/baichuan-inc/Baichuan-Audio) | Unified end-to-end speech interaction framework (tokenizer + audio LLM + flow-matching decoder), 12.5Hz multi-codebook tokens. | 百川端到端语音交互统一框架 |
| [SpeechGPT 2.0-preview](https://github.com/OpenMOSS/SpeechGPT-2.0-preview) | ![GitHub Repo stars](https://badgen.net/github/stars/OpenMOSS/SpeechGPT-2.0-preview) | End-to-end spoken dialogue LLM (7B) with <200ms latency, strong style/emotion control, tool calls and web search (Chinese-only). | 复旦 OpenMOSS，<200ms 延迟，多情感+工具调用 |
| [SALMONN-omni](https://github.com/bytedance/SALMONN) | ![GitHub Repo stars](https://badgen.net/github/stars/bytedance/SALMONN) | First standalone codec-free full-duplex speech LLM; dynamic thinking for turn-taking, barge-in, echo cancellation. | 字节，无 codec 的独立全双工语音 LLM，支持打断 |
| [Westlake-Omni](https://github.com/xinchen-ai/Westlake-Omni) | ![GitHub Repo stars](https://badgen.net/github/stars/xinchen-ai/Westlake-Omni) | Open-source Chinese emotional end-to-end speech model; unified discrete speech+text, low-latency simultaneous output. | 西湖心辰，开源中文情感语音交互模型 |
| [Sesame CSM](https://github.com/SesameAILabs/csm) | ![GitHub Repo stars](https://badgen.net/github/stars/SesameAILabs/csm) | Conversational Speech Model generating Mimi audio codes from text+audio context (Llama backbone). Powers Sesame's natural voice demo. | Sesame 对话语音生成模型，上下文驱动，自然度极高 |
| [Gemini Live API](https://ai.google.dev/gemini-api/docs/live) | - | Google's low-latency bidirectional voice and video API. Native audio understanding and generation, interruption handling, tool use. | Google 官方，原生音视频，支持打断 |
| [Gemini Live API Examples](https://github.com/google-gemini/gemini-live-api-examples) | ![GitHub Repo stars](https://badgen.net/github/stars/google-gemini/gemini-live-api-examples) | Official Google sample apps for the Gemini Live realtime voice/video API across web, mobile and backends. | Google 官方 Gemini Live 实时语音 API 示例集 |
| [OpenAI gpt-realtime](https://platform.openai.com/docs/guides/realtime) | - | Production speech-to-speech API; native audio comprehension, mid-sentence language switching, tool calling. | OpenAI 商用实时语音模型，闭源 API |

### Audio Understanding Models | 语音理解模型 (audio-in, text-out)

| Name | Stars | Description | Notes |
|------|-------|-------------|-------|
| [Qwen2-Audio](https://github.com/QwenLM/Qwen2-Audio) | ![GitHub Repo stars](https://badgen.net/github/stars/QwenLM/Qwen2-Audio) | Large audio-language model with voice-chat and audio-analysis modes; SOTA without task-specific fine-tuning. | 阿里大规模音频语言模型，免微调即 SOTA |
| [SALMONN](https://github.com/bytedance/SALMONN) | ![GitHub Repo stars](https://badgen.net/github/stars/bytedance/SALMONN) | Audio-text multimodal LLM perceiving speech, audio events and music via Whisper + BEATs dual encoders. ICLR 2024. | 字节+清华，语音/音频/音乐三模态理解 |
| [Audio Flamingo 3](https://github.com/NVIDIA/audio-flamingo) | ![GitHub Repo stars](https://badgen.net/github/stars/NVIDIA/audio-flamingo) | NVIDIA fully-open 7B large audio-language model with unified speech/sound/music encoder, CoT reasoning, up to 10-min long-audio understanding. | 英伟达全开源大音频语言模型，长音频+推理 |
| [Voxtral (Mistral)](https://mistral.ai/news/voxtral/) | - | Audio-input LLM (24B & 3B) for transcription, translation, Q&A, summarization; 32k context, multilingual, function calling. Apache 2.0 weights. | Mistral 音频理解模型，转写/翻译/问答一体 |

---

## Voice MCP & Coding Agent Voice | 语音 MCP 与编程 Agent 语音

Talk to (and be talked to by) AI coding assistants like Claude Code, Cursor and Codex. Covers MCP speech servers, voice plugins, and dictation tools developers actually use.

让你能用语音与 Claude Code, Cursor, Codex 等编程 Agent 对话，收录语音 MCP 服务、语音插件与开发者高频使用的听写工具。

### Voice MCP Servers | 语音 MCP 服务

| Name | Stars | Description | Notes |
|------|-------|-------------|-------|
| [Voice Mode (VoiceMode)](https://github.com/mbailey/voicemode) | ![GitHub Repo stars](https://badgen.net/github/stars/mbailey/voicemode) | MCP server giving Claude Code and any MCP agent full natural voice conversations; Whisper STT + OpenAI/Kokoro TTS, can run fully local. MIT. | ⭐ 给 Claude Code 加"打电话式"语音对话，最成熟的语音 MCP |
| [ElevenLabs MCP](https://github.com/elevenlabs/elevenlabs-mcp) | ![GitHub Repo stars](https://badgen.net/github/stars/elevenlabs/elevenlabs-mcp) | Official ElevenLabs MCP server: TTS, transcription, voice cloning, outbound voice agents. Works with Claude Desktop/Cursor/Windsurf. | 官方 ElevenLabs MCP，高质量 TTS+克隆+外呼，生态最广 |
| [speech-mcp](https://github.com/Kvadratni/speech-mcp) | ![GitHub Repo stars](https://badgen.net/github/stars/Kvadratni/speech-mcp) | Goose MCP voice extension with audio visualization, faster-whisper STT + Kokoro TTS (54+ voices), continuous conversation, all local. | 为 Goose 打造的本地语音 MCP，带可视化，54+ 音色 |
| [mcp-tts](https://github.com/blacktop/mcp-tts) | ![GitHub Repo stars](https://badgen.net/github/stars/blacktop/mcp-tts) | MCP server exposing multiple TTS backends (ElevenLabs, OpenAI, Google, macOS `say`) to agents. Go, MIT. | 一个 MCP 接多家 TTS（含本地 say），让 Agent 开口 |
| [mcp-server-whisper](https://github.com/arcaputo3/mcp-server-whisper) | ![GitHub Repo stars](https://badgen.net/github/stars/arcaputo3/mcp-server-whisper) | MCP server for audio transcription/processing using OpenAI Whisper + GPT-4o audio. MIT. | 用 Whisper/GPT-4o 做转写的 MCP，给 Agent 加"耳朵" |
| [claude-code-tts](https://github.com/ybouhjira/claude-code-tts) | ![GitHub Repo stars](https://badgen.net/github/stars/ybouhjira/claude-code-tts) | TTS MCP plugin specifically for Claude Code — audio feedback while coding via OpenAI TTS, non-blocking worker pool. MIT. | 专为 Claude Code 的 TTS 插件，编码时听语音反馈 |

### Coding Agent Voice Tools | 编程 Agent 语音工具

| Name | Stars | Description | Notes |
|------|-------|-------------|-------|
| [OpenClaw](https://github.com/openclaw/openclaw) | ![GitHub Repo stars](https://badgen.net/github/stars/openclaw/openclaw) | Local-first personal AI assistant across WhatsApp/Telegram/Slack/Discord/iMessage etc., with native Voice Wake + Talk Mode and a large voice-plugin ecosystem. | 🦞 现象级本地 AI 助手，原生语音唤醒+对话，语音插件生态繁荣 |
| [VoxClaw](https://github.com/malpern/VoxClaw) | ![GitHub Repo stars](https://badgen.net/github/stars/malpern/VoxClaw) | macOS menu-bar app/CLI giving OpenClaw a voice (Apple/OpenAI/ElevenLabs TTS), teleprompter overlay, network API. MIT. | 给 OpenClaw 配音的 Mac 菜单栏应用，多 TTS 后端 |
| [openclaw-voice](https://github.com/Purple-Horizons/openclaw-voice) | ![GitHub Repo stars](https://badgen.net/github/stars/Purple-Horizons/openclaw-voice) | Self-hosted browser voice chat for AI assistants, Whisper STT + ElevenLabs TTS, works with OpenAI/Claude/custom. MIT. | 浏览器端自托管语音聊天，私有免费 |
| [claude-whisper](https://github.com/Ashton-Sidhu/claude-whisper) | ![GitHub Repo stars](https://badgen.net/github/stars/Ashton-Sidhu/claude-whisper) | Push-to-talk (hold ESC) voice control for Claude Code — wake word + command transcribed and run via Claude Agent SDK. | 按住 ESC 说话，唤醒词+指令直接驱动 Claude Code |
| [voice-to-claude](https://github.com/enesbasbug/voice-to-claude) | ![GitHub Repo stars](https://badgen.net/github/stars/enesbasbug/voice-to-claude) | Claude Code plugin for high-quality dictation via whisper.cpp with Metal GPU accel; hold Ctrl+Alt to record. MIT. | whisper.cpp+Metal 加速的 Claude Code 本地听写插件 |
| [Vibe Kanban](https://github.com/BloopAI/vibe-kanban) | ![GitHub Repo stars](https://badgen.net/github/stars/BloopAI/vibe-kanban) | Kanban orchestration for Claude Code / Codex / Gemini CLI agents; pairs naturally with voice dictation for hands-free planning. | 统一编排 Claude Code/Codex 等 Agent 的看板，配语音全程动嘴 |

> **Note | 提示**: Claude Code now ships native voice dictation / push-to-talk; the tools above add richer two-way conversation, wake words and TTS feedback on top. | Claude Code 已内置原生语音听写，上述工具在此之上提供更丰富的双向对话、唤醒词与语音反馈。

### Commercial Dictation | 商业听写工具

| Name | Description | Notes |
|------|-------------|-------|
| [Wispr Flow](https://wisprflow.ai/) | Cloud AI dictation (Mac/Win/iOS/Android), auto-edits filler/grammar; dedicated Cursor & Windsurf extensions to tag files/run commands by voice. | 开发者最热门 AI 听写，深度集成 Cursor/Windsurf |
| [superwhisper](https://superwhisper.com/) | Mac-only, privacy-first dictation running Whisper fully on-device; system-wide. | Mac 本地 Whisper 听写，隐私优先，离线可用 |

---

## Toolkits, Wake Word & Voice Conversion | 语音工具箱, 唤醒词与变声

High-star, general-purpose voice/speech projects: end-to-end toolkits, wake-word detection, voice cloning and conversion.

高星通用语音项目：一体化工具箱、唤醒词检测、声音克隆与变声。

### Speech Toolkits & Libraries | 语音工具箱与库

| Name | Stars | Description | Notes |
|------|-------|-------------|-------|
| [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) | ![GitHub Repo stars](https://badgen.net/github/stars/k2-fsa/sherpa-onnx) | Offline/real-time STT, TTS, speaker diarization, VAD and keyword spotting from next-gen Kaldi; runs on 10+ platforms with many language bindings. | 下一代 Kaldi 出品，离线 STT/TTS/说话人分离/VAD，跨平台 |
| [SpeechBrain](https://github.com/speechbrain/speechbrain) | ![GitHub Repo stars](https://badgen.net/github/stars/speechbrain/speechbrain) | All-in-one PyTorch speech toolkit (ASR, TTS, diarization, enhancement, speaker ID). Apache-2.0. | 一体化 PyTorch 语音工具箱 |
| [ESPnet](https://github.com/espnet/espnet) | ![GitHub Repo stars](https://badgen.net/github/stars/espnet/espnet) | End-to-end speech processing toolkit covering ASR, TTS, speech translation, enhancement and SLU. | 端到端语音处理工具箱，覆盖 ASR/TTS/翻译 |
| [vosk-api](https://github.com/alphacep/vosk-api) | ![GitHub Repo stars](https://badgen.net/github/stars/alphacep/vosk-api) | Offline STT for Android/iOS/RPi/servers, many languages and bindings. Apache-2.0. | 离线 STT，跨平台多语言绑定 |
| [RealtimeSTT](https://github.com/KoljaB/RealtimeSTT) | ![GitHub Repo stars](https://badgen.net/github/stars/KoljaB/RealtimeSTT) | Low-latency STT library with advanced VAD, wake-word activation and instant transcription. A core voice-agent building block. | 低延迟实时 STT，带 VAD 与唤醒词，Agent 基础组件 |
| [RealtimeTTS](https://github.com/KoljaB/RealtimeTTS) | ![GitHub Repo stars](https://badgen.net/github/stars/KoljaB/RealtimeTTS) | Low-latency TTS library streaming strings/LLM token streams to audio with multi-engine fallback. | 低延迟流式 TTS，可流式播放 LLM token |
| [OpenVoiceOS (ovos-core)](https://github.com/OpenVoiceOS/ovos-core) | ![GitHub Repo stars](https://badgen.net/github/stars/OpenVoiceOS/ovos-core) | FOSS voice-assistant OS platform, the actively-maintained Mycroft successor. Apache-2.0. | FOSS 语音助手系统（Mycroft 继任者）|
| [mlx-audio](https://github.com/Blaizzy/mlx-audio) | ![GitHub Repo stars](https://badgen.net/github/stars/Blaizzy/mlx-audio) | TTS, STT and speech-to-speech library built on Apple MLX for fast on-device audio generation and recognition on Apple Silicon. | 基于 Apple MLX 的 TTS/STT/STS 库，苹果芯片本地高速推理 |

### Wake Word Detection | 唤醒词检测

| Name | Stars | Description | Notes |
|------|-------|-------------|-------|
| [openWakeWord](https://github.com/dscripka/openWakeWord) | ![GitHub Repo stars](https://badgen.net/github/stars/dscripka/openWakeWord) | Open-source wake-word/phrase detection, performance-focused and simple to train custom words. Apache-2.0. | 开源唤醒词检测，注重性能，易训练自定义词 |
| [Porcupine](https://github.com/Picovoice/porcupine) | ![GitHub Repo stars](https://badgen.net/github/stars/Picovoice/porcupine) | On-device deep-learning wake-word detection engine by Picovoice. Cross-platform, Apache-2.0. | Picovoice 端侧深度学习唤醒词检测 |

### Voice Cloning & Conversion | 声音克隆与变声

| Name | Stars | Description | Notes |
|------|-------|-------------|-------|
| [OpenVoice](https://github.com/myshell-ai/OpenVoice) | ![GitHub Repo stars](https://badgen.net/github/stars/myshell-ai/OpenVoice) | Instant voice cloning audio foundation model by MIT + MyShell; flexible style control, cross-lingual. MIT. | MIT×MyShell 即时声音克隆基础模型 |
| [RVC WebUI](https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI) | ![GitHub Repo stars](https://badgen.net/github/stars/RVC-Project/Retrieval-based-Voice-Conversion-WebUI) | Train a good voice-conversion model from ≤10 min of data. Hugely popular. MIT. | ≤10 分钟数据训练高质量变声模型 |
| [voice-changer](https://github.com/w-okada/voice-changer) | ![GitHub Repo stars](https://badgen.net/github/stars/w-okada/voice-changer) | Real-time voice changer supporting RVC, so-vits-svc and other backends. | 实时变声器，支持多种模型后端 |
| [MockingBird](https://github.com/babysor/MockingBird) | ![GitHub Repo stars](https://badgen.net/github/stars/babysor/MockingBird) | Clone a (esp. Chinese) voice in ~5s for real-time speech. Very popular in the CN community. | 5 秒克隆音色实时合成，中文社区代表作 |

### CLI & Local Dictation Tools | 命令行与本地听写工具

| Name | Stars | Description | Notes |
|------|-------|-------------|-------|
| [Handy](https://github.com/cjpais/Handy) | ![GitHub Repo stars](https://badgen.net/github/stars/cjpais/Handy) | Free, fully-offline push-to-talk dictation app (Tauri/Rust) for Win/Mac/Linux using Whisper + Parakeet, auto-pasting into any field. | 全离线按键说话听写，跨平台，自动粘贴 |
| [vibe](https://github.com/thewh1teagle/vibe) | ![GitHub Repo stars](https://badgen.net/github/stars/thewh1teagle/vibe) | Cross-platform offline audio/video transcription (90+ languages, diarization) with CLI and HTTP API. | 跨平台离线音视频转录，含 CLI 与 HTTP API |
| [WhisperWriter](https://github.com/savbell/whisper-writer) | ![GitHub Repo stars](https://badgen.net/github/stars/savbell/whisper-writer) | Small Python dictation app: hotkey listens, then auto-types Whisper transcription into the active window. | 轻量 Python 听写，热键触发自动输入 |
| [nerd-dictation](https://github.com/ideasman42/nerd-dictation) | ![GitHub Repo stars](https://badgen.net/github/stars/ideasman42/nerd-dictation) | Single-file, hackable offline speech-to-text for Linux using VOSK, with Python-based text post-processing. | 单文件可魔改的 Linux 离线听写 |
| [wyoming-satellite](https://github.com/rhasspy/wyoming-satellite) | ![GitHub Repo stars](https://badgen.net/github/stars/rhasspy/wyoming-satellite) | Remote voice satellite (Wyoming protocol) for Home Assistant on Raspberry Pi with local wake-word detection. | Home Assistant 远程语音卫星，树莓派+本地唤醒词 |

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
| [Unpod](https://unpod.ai) | Voice infrastructure platform for building AI-native phone and messaging agents. Handles real-time call routing, low-latency speech pipelines, and telephony + SMS automation. | 电话+消息自动化，AI 原生语音基础设施 \| [GitHub](https://github.com/geneffic/unpod) |
| [voicetest](https://github.com/voicetestdev/voicetest) | Test harness for voice agents. Import from Retell, VAPI, Bland, LiveKit. Run simulations. Evaluate with LLM judges. | 开源测试工具，多平台支持 |
| [Future AGI](https://github.com/future-agi/future-agi) | Open-source platform to stress-test voice and text AI agents with persona-driven, multi-turn simulations, scoring the results with 70+ evals to find where an agent breaks before your users do. | 用人设多轮对话压测语音/文本 Agent，转写打分，提前发现问题 |

### Technical Blogs & Documentation | 技术博客与文档

| Name | Description | Notes |
|------|-------------|-------|
| [Voice AI & Voice Agents Primer](https://voiceaiandvoiceagents.com/) | Comprehensive illustrated guide to voice AI. Architecture design, technical overview, best practices. | 全面的语音 AI 图解指南 |
| [AssemblyAI Blog: Turn Detection](https://www.assemblyai.com/blog/turn-detection-endpointing-voice-agent) | In-depth analysis of turn detection. Algorithm comparison, latency analysis. | 话轮检测深度解析 |
| [LiveKit Blog: Transformer Turn Detection](https://blog.livekit.io/using-a-transformer-to-improve-end-of-turn-detection/) | Using transformers to improve endpointing. Technical details, performance comparison. | Transformer 改进端点检测 |
| [Krisp Blog: Turn-Taking](https://krisp.ai/blog/improving-turn-taking-of-ai-voice-agents-with-background-voice-cancellation/) | Background noise cancellation improves turn-taking. Evaluation and results. | 背景噪音消除改善话轮 |
| [Speechmatics: Semantic Turn Detection](https://blog.speechmatics.com/semantic-turn-detection) | Semantic turn detection with SLM. Implementation guide, threshold tuning. | 使用 SLM 的语义话轮检测 |
| [Agora: TEN VAD & Turn Detection](https://www.agora.io/en/blog/making-voice-ai-agents-more-human-with-ten-vad-and-turn-detection/) | Making voice agents more human with TEN VAD and Turn Detection. | TEN 的 VAD 和话轮检测 |

---

## Learning Resources | 学习资源

Curated resources for getting started and going deep with voice AI agents.

入门与进阶语音 AI Agent 的精选学习资源。

| Name | Description | Notes |
|------|-------------|-------|
| [Voice AI & Voice Agents Primer](https://voiceaiandvoiceagents.com/) | Comprehensive illustrated guide to voice AI. Architecture design, technical overview, best practices. | 全面的语音 AI 图解指南，强烈推荐入门 |
| [Voice Agent Knowledge Base (Feishu)](https://realtime.feishu.cn/docx/FFcedfbkNoNA3OxeD2IcdRWbnLf) | Comprehensive Voice Agent knowledge base in Chinese. Systematic tutorials, practical experience. | Voice Agent 中文知识库 |
| [AssemblyAI Blog: Turn Detection](https://www.assemblyai.com/blog/turn-detection-endpointing-voice-agent) | In-depth analysis of turn detection. Algorithm comparison, latency analysis. | 话轮检测深度解析 |
| [LiveKit Blog: Transformer Turn Detection](https://blog.livekit.io/using-a-transformer-to-improve-end-of-turn-detection/) | Using transformers to improve endpointing. Technical details, performance comparison. | Transformer 改进端点检测 |
| [Speechmatics: Semantic Turn Detection](https://blog.speechmatics.com/semantic-turn-detection) | Semantic turn detection with SLM. Implementation guide, threshold tuning. | 使用 SLM 的语义话轮检测 |
| [Agora: TEN VAD & Turn Detection](https://www.agora.io/en/blog/making-voice-ai-agents-more-human-with-ten-vad-and-turn-detection/) | Making voice agents more human with TEN VAD and Turn Detection. | TEN 的 VAD 和话轮检测 |

> 更多技术博客见上方 [Technical Blogs & Documentation](#technical-blogs--documentation--技术博客与文档) 小节。

---

## Related Awesome Lists | 相关资源

- [awesome-voice-conversion](https://github.com/JeffC0628/awesome-voice-conversion)
- [awesome-ai-agents](https://github.com/e2b-dev/awesome-ai-agents)

---

## Contributing | 贡献指南

Contributions are welcome! 欢迎贡献！

1. Fork this repository and create a new branch. | Fork 本仓库并新建分支。
2. Add your resource to the most relevant section, keeping the existing table format (Name, Stars, Description, Notes). | 将资源添加到最相关的小节，保持现有表格格式。
3. Ensure the link is valid and the project is actively maintained and relevant to voice AI agents. | 确保链接有效，项目活跃维护且与语音 AI Agent 相关。
4. Keep descriptions concise and provide bilingual (English + 中文) notes where possible. | 描述简洁，尽量提供中英双语说明。
5. Submit a Pull Request describing what you added and why. | 提交 PR 并说明添加内容及理由。

You can also open an Issue to suggest resources or report broken links. | 也可通过 Issue 推荐资源或报告失效链接。

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
**微信公众号 | WeChat Official Account: 云中江树**  
**WeChat | 微信: 1796060717** (欢迎加微信交流 Voice Agent 技术)  

Welcome to exchange and discuss Voice Agent technology through Issues or PRs!  
欢迎通过 Issues 或 PR 交流讨论 Voice Agent 相关技术！
