<p align="center">
    <img alt="AI Engineering Interview Questions Company Wise" src="https://github.com/pallavi-shekhar/ai-engineering-interview-questions-company-wise/blob/main/assets/banner.png">
</p>

# AI 工程面试题（按公司分类）

> AI Engineering Interview Questions Company Wise - Your Cheat Sheet For AI Engineering Interviews at Top AI Companies
>
> 这是一个按公司整理的 AI 工程面试题速查表，覆盖 35 家顶尖 AI 公司，按企业分组收录真实面试题，并在我们有答案时附上链接。
>
> 这些题目适用于以下岗位：
>
> - AI Engineer
> - Gen AI Engineer
> - LLM Engineer
> - Agentic AI Engineer
> - AI Agent Engineer
> - Machine Learning Engineer
> - Research Engineer
> - Applied Scientist
> - Forward Deployed Engineer
> - AI Solutions Architect
> - AI Platform Engineer
> - Applied AI Engineer
> - LLM Inference and Performance Engineer
> - MLOps Engineer
> - LLMOps Engineer

## 目录

- [如何使用本仓库](#如何使用本仓库)
- [跨公司常见问题](#跨公司常见问题)
  - [LLM 内部机制与架构](#llm-内部机制与架构)
  - [推理、服务与 GPU 性能](#推理服务与-gpu-性能)
  - [RAG 与检索](#rag-与检索)
  - [Agents 与工具调用](#agents-与工具调用)
  - [微调、后训练与对齐](#微调后训练与对齐)
  - [评估与可观测性](#评估与可观测性)
  - [安全、隐私与负责任 AI](#安全隐私与负责任-ai)
  - [多模态、语音与语音 AI](#多模态语音与语音-ai)
  - [AI 系统设计](#ai-系统设计)
  - [编码与数据结构](#编码与数据结构)
- [前沿 AI 实验室](#前沿-ai-实验室)
  - [Anthropic](#anthropic)
  - [OpenAI](#openai)
  - [Google DeepMind 与 Google AI](#google-deepmind-与-google-ai)
  - [Meta（Superintelligence Labs、FAIR、Llama）](#meta-superintelligence-labs-fair-llama)
  - [xAI](#xai)
  - [Mistral AI](#mistral-ai)
  - [Cohere](#cohere)
  - [DeepSeek](#deepseek)
  - [Moonshot AI (Kimi)](#moonshot-ai-kimi)
  - [Zhipu AI (GLM)](#zhipu-ai-glm)
  - [Alibaba (Qwen)](#alibaba-qwen)
  - [Sarvam AI](#sarvam-ai)
- [大厂 AI 组织](#大厂-ai-组织)
  - [Microsoft](#microsoft)
  - [Amazon (AWS)](#amazon-aws)
  - [Apple](#apple)
  - [NVIDIA](#nvidia)
  - [Tesla](#tesla)
  - [消费级规模 ML 公司（Uber、Netflix、LinkedIn、Airbnb、Pinterest、Spotify）](#消费级规模-ml-公司uber-netflix-linkedin-airbnb-pinterest-spotify)
- [AI 基础设施与平台公司](#ai-基础设施与平台公司)
  - [Databricks](#databricks)
  - [Groq](#groq)
  - [Together AI](#together-ai)
  - [Hugging Face](#hugging-face)
  - [Scale AI](#scale-ai)
  - [Perplexity](#perplexity)
- [AI 原生产品公司](#ai-原生产品公司)
  - [Cursor (Anysphere)](#cursor-anysphere)
  - [Cognition (Devin, Windsurf)](#cognition-devin-windsurf)
  - [Sierra](#sierra)
  - [Harvey](#harvey)
  - [Glean](#glean)
  - [Character.AI](#characterai)
  - [ElevenLabs](#elevenlabs)
  - [Abridge](#abridge)
  - [Figure AI](#figure-ai)
  - [Waymo](#waymo)
- [前置部署与企业 AI](#前置部署与企业-ai)
  - [Palantir](#palantir)

### 维护者：[Outcome School](https://outcomeschool.com)

> AI 与机器学习课程： [AI and Machine Learning Program](https://outcomeschool.com/program/ai-and-machine-learning)

### 关注 Outcome School

- [YouTube](https://youtube.com/@OutcomeSchool)
- [X/Twitter](https://x.com/outcome_school)
- [LinkedIn](https://www.linkedin.com/company/outcomeschool)
- [GitHub](https://github.com/OutcomeSchool)

---

> **说明：我们会持续更新新的题目和答案。**
>
> 若想看按主题整理的题目与答案，请见 [AI Engineering Interview Questions and Answers](https://github.com/amitshekhariitbhu/ai-engineering-interview-questions).

---

## 如何使用本仓库

- 题目来自公开报道的面试经历，内容不涉及机密。面试轮次会持续变化，并且会因团队、级别和地区而不同，所以把每家公司部分视作“该公司关注什么”的地图，而不是“会被问什么”的脚本。
- 先从 [跨公司常见问题](#跨公司常见问题) 开始。这些是高频重复出现的问题，每道题只在此处列出一次，并注明它出现在哪些公司。
- 然后去看目标公司。每个公司章节都会列出该岗位覆盖范围、公开报道的面试流程，以及按主题归纳的公司专项题目。
- 只要我们有答案，就会直接放在每道题下面链接中。我们会持续补充。

---

## 跨公司常见问题

> 这些题目会在很多 AI 工程面试中出现。每道题只出现在这里，并标注它在哪些公司出现过。建议先把这些问题刷一遍。

### LLM 内部机制与架构

- 解释缩放点积注意力（scaled dot-product attention），以及 1/sqrt(d_k) 缩放因子为什么重要。
  - 答案： [Math behind √dₖ Scaling Factor in Attention](https://outcomeschool.com/blog/scaling-dot-product-attention) 与 [Math behind Attention - Q, K, and V](https://outcomeschool.com/blog/math-behind-attention-qkv)
- KV Cache 是什么？它在大规模场景下会带来什么内存影响？请推导公式。
  - 见于： [OpenAI](#openai), [xAI](#xai), [Mistral AI](#mistral-ai), [Amazon](#amazon-aws), [Apple](#apple), [NVIDIA](#nvidia), [Together AI](#together-ai), [Character.AI](#characterai)
  - 答案： [What is KV Cache in LLMs?](https://outcomeschool.com/blog/kv-cache-in-llms) 与 [KV Cache Compression](https://outcomeschool.com/blog/kv-cache-compression)
- 什么是 Multi-Query Attention (MQA) 和 Grouped-Query Attention (GQA)？它们各自牺牲了什么？
  - 见于： [Meta](#meta-superintelligence-labs-fair-llama), [Mistral AI](#mistral-ai)
  - 答案： [Grouped Query Attention](https://outcomeschool.com/blog/grouped-query-attention)
- 什么是 Multi-head Latent Attention (MLA)？DeepSeek 为什么要引入它？
  - 见于： [DeepSeek](#deepseek), [Moonshot AI](#moonshot-ai-kimi)
  - 答案： [KV Cache Compression](https://outcomeschool.com/blog/kv-cache-compression)
- 解释 FlashAttention。它不减少 FLOPs，为什么仍然更快？
  - 见于： [Together AI](#together-ai)
  - 答案： [Decoding Flash Attention in LLMs](https://outcomeschool.com/blog/decoding-flash-attention)
- BPE 是如何工作的？它有哪些失败模式（数字、代码、非拉丁文字）？
  - 见于： [Alibaba](#alibaba-qwen), [Sarvam AI](#sarvam-ai), [Hugging Face](#hugging-face)
  - 答案： [Byte Pair Encoding](https://outcomeschool.com/blog/bpe-in-llms) 与 [Tokenization in Large Language Models (LLMs)](https://www.youtube.com/watch?v=sK2s9I84EVI) 与 [Tokenization in LLMs](https://outcomeschool.com/blog/tokenization-in-llms)
- Transformer 中的位置编码是什么？它经历了怎样的演化（sinusoidal → learned → RoPE → ALiBi）？
  - 答案： [Positional Embeddings in LLMs](https://outcomeschool.substack.com/p/positional-embeddings-in-llms) 与 [Math Behind RoPE (Rotary Position Embedding)](https://outcomeschool.com/blog/math-behind-rope-rotary-position-embedding)
- 解释 RoPE，以及位置插值（position interpolation）/ YaRN 是如何把上下文长度扩展到训练长度之外的。
  - 见于： [Meta](#meta-superintelligence-labs-fair-llama), [Moonshot AI](#moonshot-ai-kimi), [Alibaba](#alibaba-qwen)
  - 答案： [Math Behind RoPE (Rotary Position Embedding)](https://outcomeschool.com/blog/math-behind-rope-rotary-position-embedding)
- Chinchilla 缩放定律说了什么？它和早期的扩展直觉有何不同？
  - 见于： [Anthropic](#anthropic)
- 什么是 Mixture-of-Experts（MoE）架构？它如何在不增加 FLOPs 的情况下扩展容量？
  - 见于： [Mistral AI](#mistral-ai), [Cohere](#cohere), [DeepSeek](#deepseek), [Moonshot AI](#moonshot-ai-kimi), [Zhipu AI](#zhipu-ai-glm), [Alibaba](#alibaba-qwen)
  - 答案： [Mixture of Experts Explained](https://outcomeschool.com/blog/mixture-of-experts)
- 解释预训练（pre-training）、监督微调（SFT）和偏好优化（preference optimization）之间的区别。
  - 见于： [Meta](#meta-superintelligence-labs-fair-llama), [Scale AI](#scale-ai)
  - 答案： [Decoding InstructGPT](https://outcomeschool.com/blog/decoding-instructgpt) 与 [RLHF](https://outcomeschool.com/blog/reinforcement-learning-from-human-feedback-rlhf) 与 [How does Pretraining work?](https://outcomeschool.com/blog/llm-pretraining)
- 对比 greedy、beam search、top-k、top-p 和 temperature sampling。每种方法在什么情况下会失败？
  - 见于： [Google DeepMind](#google-deepmind-and-google-ai), [Apple](#apple), [Perplexity](#perplexity)
  - 答案： [How does Temperature control LLM output?](https://outcomeschool.com/blog/how-does-temperature-control-llm-output) 与 [How do Top-k and Top-p Sampling work?](https://outcomeschool.com/blog/how-do-top-k-and-top-p-sampling-work)
- “lost-in-the-middle” 是什么？在长上下文中如何规避？
  - 见于： [Moonshot AI](#moonshot-ai-kimi)
  - 答案： [The Lost in the Middle Problem in LLMs](https://outcomeschool.com/blog/lost-in-the-middle-problem-in-llms)
- 为什么 LayerNorm 会放在现代 Transformer 的前置 block 中？RMSNorm 又是什么？
  - 答案： [RMSNorm (Root Mean Square Layer Normalization)](https://outcomeschool.com/blog/rmsnorm-root-mean-square-layer-normalization)
- 解释 SwiGLU，以及为什么门控激活（gated activations）替代了现代 LLM MLP 中的 ReLU/GELU。
  - 见于： [Meta](#meta-superintelligence-labs-fair-llama)
  - 答案： [Feed-Forward Networks in LLMs](https://outcomeschool.com/blog/feed-forward-networks-in-llms)
- 逐张量地讲讲 decoder-only transformer 在一次前向传播中的发生过程。
  - 见于： [Anthropic](#anthropic)
  - 答案： [Decoding Transformer Architecture](https://outcomeschool.com/blog/decoding-transformer-architecture)

### 推理、服务与 GPU 性能

- 解释 prefill 和 decode 两个阶段。为什么 prefill 是计算绑定（compute-bound），而 decode 是内存带宽绑定（memory-bandwidth-bound）？
  - 见于： [Moonshot AI](#moonshot-ai-kimi), [NVIDIA](#nvidia), [Together AI](#together-ai)
  - 答案： [Prefill vs Decode: LLM Inference Optimization](https://outcomeschool.com/blog/prefill-vs-decode-llm-inference-optimization)
- 什么是 continuous batching？为什么它取代了静态 batching？
  - 见于： [Anthropic](#anthropic), [xAI](#xai), [Mistral AI](#mistral-ai), [NVIDIA](#nvidia), [Together AI](#together-ai)
  - 答案： [Continuous Batching in LLMs](https://outcomeschool.com/blog/continuous-batching-in-llms)
- PagedAttention 是如何工作的？它解决了什么 KV-cache 碎片化问题？
  - 见于： [NVIDIA](#nvidia), [Together AI](#together-ai)
  - 答案： [Paged Attention in LLMs](https://outcomeschool.com/blog/paged-attention-in-llms) 与 [How does vLLM work?](https://outcomeschool.com/blog/how-does-vllm-work)
- 什么是 speculative decoding？为什么输出质量不变，而且什么时候它没用？
  - 见于： [NVIDIA](#nvidia), [Together AI](#together-ai)
  - 答案： [Speculative Decoding](https://outcomeschool.com/blog/speculative-decoding)
- 解释 prefix caching / prompt caching。什么时候该用，缓存前缀什么会失效？
  - 见于： [Moonshot AI](#moonshot-ai-kimi), [Character.AI](#characterai)
  - 答案： [How does Prompt Caching work?](https://outcomeschool.com/blog/how-does-prompt-caching-work)
- 对比 FP16、BF16、FP8、INT8、INT4 和 FP4：在服务阶段各自的利弊与限制是什么？
  - 见于： [Mistral AI](#mistral-ai), [Apple](#apple), [NVIDIA](#nvidia), [Together AI](#together-ai), [Character.AI](#characterai)
  - 答案： [How does Model Quantization work?](https://outcomeschool.com/blog/how-does-model-quantization-work)
- 对比 tensor、pipeline、data、sequence 和 expert parallelism。什么时候需要组合使用？
  - 见于： [Google DeepMind](#google-deepmind-and-google-ai), [Meta](#meta-superintelligence-labs-fair-llama), [Amazon](#amazon-aws), [NVIDIA](#nvidia)
- 估算一台 GPU 服务 70B 模型时所需的显存：权重、KV cache、激活值和碎片化。
  - 见于： [NVIDIA](#nvidia)
  - 答案： [What is KV Cache in LLMs?](https://outcomeschool.com/blog/kv-cache-in-llms) 与 [Paged Attention in LLMs](https://outcomeschool.com/blog/paged-attention-in-llms) 与 [How does an LLM use GPU memory?](https://outcomeschool.com/blog/llm-gpu-memory)
- 什么是 TTFT、TPOT、ITL 和 throughput？它们如何相互取舍？
  - 见于： [Microsoft](#microsoft), [Apple](#apple), [Perplexity](#perplexity)
  - 答案： [Prefill vs Decode: LLM Inference Optimization](https://outcomeschool.com/blog/prefill-vs-decode-llm-inference-optimization) 与 [The First-Token Latency Problem in LLMs](https://www.youtube.com/watch?v=XD8DD4cEHu0)
- 选择 vLLM、SGLang、TensorRT-LLM 还是自定义栈时，如何做取舍？
  - 见于： [NVIDIA](#nvidia), [Together AI](#together-ai)
  - 答案： [How does vLLM work?](https://outcomeschool.com/blog/how-does-vllm-work), [How does SGLang work?](https://outcomeschool.com/blog/how-does-sglang-work) 和 [How does TensorRT-LLM work?](https://outcomeschool.com/blog/how-does-tensorrt-llm-work)
- 如何把 LLM 服务成本压低 10 倍？枚举所有杠杆并按优先级排序。
  - 见于： [Microsoft](#microsoft), [Amazon](#amazon-aws), [NVIDIA](#nvidia), [Cursor](#cursor-anysphere)
  - 答案： [LLM Inference Optimization](https://outcomeschool.com/blog/llm-inference-optimization)

### RAG 与检索

- 对大型技术文档语料，你会采用哪种 chunking 策略？为什么？
  - 见于： [Glean](#glean)
  - 答案： [Chunking Strategies for RAG](https://outcomeschool.com/blog/chunking-strategies-for-rag)
- 如何在稀疏检索（BM25）和稠密检索之间选择？什么时候需要两者结合？
  - 见于： [Microsoft](#microsoft), [Perplexity](#perplexity), [Glean](#glean)
  - 答案： [How does Hybrid Search work?](https://outcomeschool.com/blog/how-does-hybrid-search-work)
- 什么是 reranker？什么时候应该使用它？交叉编码器会带来什么成本？
  - 见于： [Cohere](#cohere), [Microsoft](#microsoft), [Perplexity](#perplexity)
  - 答案： [How does a Reranker work?](https://outcomeschool.com/blog/how-does-a-reranker-work)
- 你如何评估一个 RAG 系统的质量：检索和生成要分开评估？
  - 见于： [Cohere](#cohere)
  - 答案： [LLM Evaluation](https://outcomeschool.com/blog/llm-evaluation)
- 什么是 HyDE（Hypothetical Document Embeddings）？什么时候它比标准稠密检索更有效？
  - 答案： [How does HyDE work in RAG?](https://outcomeschool.com/blog/how-does-hyde-work)
- Agentic RAG 与标准 RAG 的区别是什么？什么时候值得增加复杂度？
  - 答案： [Agentic RAG](https://outcomeschool.com/blog/agentic-rag)
- 设计权限感知的检索：用户绝不能看到其在源系统中无权访问的内容。
  - 见于： [Microsoft](#microsoft), [Databricks](#databricks), [Glean](#glean), [Palantir](#palantir)
- 比较 HNSW、IVF-PQ 和 flat index。如何挑选？召回率提升的代价是什么？
  - 答案： [How does Approximate Nearest Neighbor (ANN) search work?](https://outcomeschool.com/blog/how-does-approximate-nearest-neighbor-ann-search-work) 与 [How does a Vector Database work?](https://outcomeschool.com/blog/how-does-a-vector-database-work)
- 在持续更新的语料库中，如何保持索引新鲜？
  - 见于： [Perplexity](#perplexity), [Cursor](#cursor-anysphere)
- 如何把生成答案中的每个声明追踪到具体的检索片段？
  - 见于： [Perplexity](#perplexity), [Harvey](#harvey), [Abridge](#abridge)

### Agents 与工具调用

- 解释 ReAct 模式，以及它相较纯 chain-of-thought 解决了什么问题。
  - 答案： [ReAct Agent](https://outcomeschool.com/blog/react-agent) 与 [How does Chain-of-Thought (CoT) Prompting work?](https://outcomeschool.com/blog/how-does-chain-of-thought-prompting-work)
- 如何处理 agentic loop 中的工具调用错误、超时和重试？
  - 见于： [OpenAI](#openai), [Cognition](#cognition-devin-windsurf)
  - 答案： [AI Agent Loop](https://outcomeschool.com/blog/ai-agent-loop)
- 结构化输出和函数调用有什么区别？
  - 见于： [Mistral AI](#mistral-ai), [Apple](#apple)
  - 答案： [How does Function Calling work in LLMs?](https://outcomeschool.com/blog/how-does-function-calling-work-in-llms)
- 什么是 MCP（Model Context Protocol）？它和传统 function calling 有何不同？
  - 见于： [Microsoft](#microsoft)
- 工具太多会怎样？如何设计 LLM 真正能可靠调用的工具 schema？
  - 见于： [Anthropic](#anthropic), [Cognition](#cognition-devin-windsurf)
- 多 agent 编排怎么做？什么时候会失效？
  - 见于： [Cognition](#cognition-devin-windsurf)
- 设计一个长时间运行的 agent 的记忆系统：存什么、放哪里、如何检索？
  - 见于： [Anthropic](#anthropic)
- Agent 如何决定是调用工具还是直接回答？
- 让 agent 循环正确终止，如何限制代价和步骤数？
  - 答案： [AI Agent Loop](https://outcomeschool.com/blog/ai-agent-loop)
- 生产系统中如何让 agent 的动作可逆，至少可审计？
  - 见于： [Palantir](#palantir)
- 设计“人类在环”审批：当 agent 执行高风险行动时，如何把关？
  - 见于： [OpenAI](#openai), [Palantir](#palantir)

### 微调、后训练与对齐

- 解释 RLHF 的端到端流程：奖励模型、策略优化、KL 惩罚。
  - 答案： [RLHF](https://outcomeschool.com/blog/reinforcement-learning-from-human-feedback-rlhf) 与 [PPO](https://outcomeschool.com/blog/proximal-policy-optimization-ppo)
- 什么是 DPO？为什么它在很多实验室中取代了 PPO-based RLHF？什么时候在线 RL 仍然更有效？
  - 见于： [Hugging Face](#hugging-face), [Scale AI](#scale-ai)
  - 答案： [Direct Preference Optimization (DPO)](https://outcomeschool.com/blog/direct-preference-optimization-dpo)
- 解释 GRPO 以及为什么在大规模场景下去掉 value network 很关键。
  - 见于： [DeepSeek](#deepseek)
  - 答案： [Group Relative Policy Optimization (GRPO)](https://outcomeschool.com/blog/group-relative-policy-optimization-grpo)
- 解释 LoRA 的数学分解：为什么它有效？如何选择 rank r？
  - 答案： [LoRA - Low-Rank Adaptation of LLMs](https://outcomeschool.com/blog/lora-low-rank-adaptation-of-llms)
- QLoRA 是如何实现显存下降的？量化带来哪些权衡？
  - 见于： [Hugging Face](#hugging-face)
- 比较 LoRA、prefix tuning、prompt tuning 和 full fine-tuning：何时选哪种？
  - 见于： [Sarvam AI](#sarvam-ai), [Apple](#apple)
- 什么是 catastrophic forgetting？微调时如何缓解？
  - 见于： [Mistral AI](#mistral-ai)
- Prompting、RAG 和 fine-tuning：给出成本与延迟感知的决策框架。
  - 见于： [OpenAI](#openai), [Mistral AI](#mistral-ai), [Cohere](#cohere), [Microsoft](#microsoft), [Databricks](#databricks), [Glean](#glean)
- 什么是 RLVR（RL with verifiable rewards）？它在什么场景下优于 learned reward model？
  - 见于： [Zhipu AI](#zhipu-ai-glm), [Alibaba](#alibaba-qwen), [Sarvam AI](#sarvam-ai), [Scale AI](#scale-ai)
- 解释 reward hacking，以及实验室如何应对它。
  - 见于： [Scale AI](#scale-ai)
- 什么是蒸馏（distillation）？如何从大模型中训练一个强小模型？
  - 见于： [Alibaba](#alibaba-qwen)

### 评估与可观测性

- 设计一个 LLM-as-judge 评估方案。它有哪些已知偏差？如何修正？
  - 见于： [Perplexity](#perplexity)
  - 答案： [LLM as a Judge](https://outcomeschool.com/blog/llm-as-a-judge)
- 当没有标注 ground truth 且专家成本很高时，如何构建评估集？
  - 见于： [Cohere](#cohere), [Harvey](#harvey)
- 如何检测和测量生产中 RAG 系统的幻觉？
  - 见于： [Anthropic](#anthropic), [OpenAI](#openai), [Cursor](#cursor-anysphere)
- 设计回归门禁，用于决定提示词或模型变更是否应该上线。
  - 见于： [Anthropic](#anthropic)
- 为什么 benchmark 分数提升了，但用户却觉得系统变差了？原因有哪些？
  - 见于： [Cognition](#cognition-devin-windsurf)
- 什么是 benchmark contamination？如何防范？
  - 见于： [Zhipu AI](#zhipu-ai-glm), [Alibaba](#alibaba-qwen), [Scale AI](#scale-ai)
- 一个生产化 LLM 系统需要哪些观测能力：trace、span、成本、反馈？
  - 答案： [AI Agent Observability](https://outcomeschool.com/blog/ai-agent-observability)
- 如何管理生产中的 prompt 版本和回滚？
- 在线评估需要记录什么、抽样什么、做 A/B 什么？
  - 见于： [Perplexity](#perplexity)
- 如果评估的是 agent，而不是单次模型响应，应该怎样做？
  - 见于： [Moonshot AI](#moonshot-ai-kimi), [Zhipu AI](#zhipu-ai-glm), [Scale AI](#scale-ai), [Cognition](#cognition-devin-windsurf)
  - 答案： [AI Agent Evaluation](https://outcomeschool.com/blog/ai-agent-evaluation)

### 安全、隐私与负责任 AI

- 什么是 prompt injection（直接和间接）？你的分层防御策略是什么？
  - 见于： [Anthropic](#anthropic), [OpenAI](#openai), [Microsoft](#microsoft), [Sierra](#sierra)
  - 答案： [Prompt Injection in LLMs](https://outcomeschool.com/blog/prompt-injection-in-llms)
- OWASP Top 10 for LLM applications 里哪些问题在实际中最容易落地？
- jailbreak 和 adversarial prompting 的区别是什么？
  - 答案： [Prompt Injection in LLMs](https://outcomeschool.com/blog/prompt-injection-in-llms) 与 [What is jailbreaking in LLMs?](https://outcomeschool.com/blog/jailbreaking-in-llms)
- 为消费级助手设计 guardrails：输入过滤、输出过滤，还是两者都要？
  - 见于： [Sierra](#sierra), [Character.AI](#characterai)
  - 答案： [How do LLM guardrails work?](https://outcomeschool.com/blog/how-do-llm-guardrails-work)
- Constitutional AI 和 RLHF 的区别是什么？RLAIF 又是什么？
  - 见于： [Anthropic](#anthropic)
- 如何防止一个具备工具权限的 agent 通过恶意网页将数据窃取出去？
  - 见于： [OpenAI](#openai)
- 如何处理 prompts、日志和训练数据中的 PII？
  - 见于： [Abridge](#abridge)
- 什么是 mechanistic interpretability？为什么研究实验室会投入它？
- 如果你在部署模型后，需要审计它在不同用户群体上的差异化表现，应该怎么做？
  - 见于： [Microsoft](#microsoft)

### 多模态、语音与语音 AI

- 视觉语言模型如何把图像送进 LLM：投影器、cross-attention，还是原生 token？
  - 见于： [Meta](#meta-superintelligence-labs-fair-llama), [Alibaba](#alibaba-qwen)
  - 答案： [Multimodal AI](https://outcomeschool.com/blog/multimodal-ai) 与 [How does a Vision-Language Model (VLM) work?](https://outcomeschool.com/blog/vision-language-model-vlm)
- 从图像到视频后，系统发生了什么变化？
  - 见于： [Meta](#meta-superintelligence-labs-fair-llama)
- 预算一个实时语音 agent 的端到端延迟：VAD、ASR、LLM、TTS、网络。时间究竟花在哪里？
  - 见于： [Sarvam AI](#sarvam-ai), [ElevenLabs](#elevenlabs)
  - 答案： [Design a Real-Time Voice AI Agent](https://outcomeschool.com/blog/design-a-real-time-voice-ai-agent)
- 设计 barge-in / interruption handling：如何让语音 agent 能正确处理打断？
  - 见于： [ElevenLabs](#elevenlabs)
- cascaded ASR+LLM+TTS 与 native speech-to-speech 怎么选？
  - 见于： [ElevenLabs](#elevenlabs)
- 如何评估 ASR 质量（不仅仅是 WER），以及 TTS 质量（因为没有唯一正确答案）？
  - 见于： [ElevenLabs](#elevenlabs)
- 处理代码切换和口音在生产 ASR 中有哪些关键问题？
  - 见于： [Sarvam AI](#sarvam-ai), [Abridge](#abridge)
- 解释 streaming TTS chunking 和 jitter-buffer sizing。
  - 见于： [ElevenLabs](#elevenlabs)
- 设计 diarisation（说话人分离）系统：关键不是仅仅聚类，而是“把角色归因清楚”。
  - 见于： [Abridge](#abridge)

### AI 系统设计

- 设计一个面向 1000 万文档的企业 RAG 助手，并支持每用户权限控制。
  - 见于： [OpenAI](#openai), [Microsoft](#microsoft), [Amazon](#amazon-aws), [Databricks](#databricks), [Scale AI](#scale-ai)
- 设计一个代码助手：仓库索引、上下文装配、修改应用、评估闭环。
  - 见于： [Cursor](#cursor-anysphere)
- 设计一个能真正下单并升级到人工客服的客户支持 agent。
  - 见于： [Consumer-Scale ML Companies](#consumer-scale-ml-companies-uber-netflix-linkedin-airbnb-pinterest-spotify), [Sierra](#sierra)
- 设计大规模商品目录上的语义搜索。
  - 见于： [Character.AI](#characterai)
- 设计一个结合分类器和 LLM 的内容审核系统。
  - 见于： [Meta](#meta-superintelligence-labs-fair-llama)
- 设计一个文档智能管道：扫描 PDF 输入，输出结构化字段，支持 1000 万文档规模。
  - 见于： [Palantir](#palantir)
- 设计一个超大型数据仓库上的 Text-to-SQL 系统。
  - 见于： [Databricks](#databricks), [Palantir](#palantir)
- 设计一个会议助理：录音、说话人分离、摘要、行动项、集成。
  - 见于： [Microsoft](#microsoft)
- 设计一个 LLM gateway：跨 provider 路由、故障转移、缓存、预算和限流。
  - 见于： [Perplexity](#perplexity), [Palantir](#palantir)
- 设计一个服务于数亿用户的消费级聊天助手的基础设施栈。
  - 见于： [Anthropic](#anthropic), [OpenAI](#openai), [Google DeepMind](#google-deepmind-and-google-ai), [Meta](#meta-superintelligence-labs-fair-llama), [xAI](#xai)

### 编码与数据结构

- 从零实现 scaled dot-product attention，并加上 causal mask，用 NumPy 或 PyTorch。
  - 见于： [Anthropic](#anthropic), [Google DeepMind](#google-deepmind-and-google-ai), [Amazon](#amazon-aws)
- 实现 multi-head attention，然后改成 grouped-query attention。
  - 见于： [Google DeepMind](#google-deepmind-and-google-ai), [Mistral AI](#mistral-ai), [Alibaba](#alibaba-qwen)
- 实现 KV cache 和单步 decode。
  - 见于： [Moonshot AI](#moonshot-ai-kimi)
- 从零实现 BPE 训练与编码。
- 实现 top-k、top-p 和 temperature sampling。
  - 见于： [Google DeepMind](#google-deepmind-and-google-ai), [Apple](#apple)
- 实现 O(1) 的 LRU cache，再加 TTL。
  - 见于： [OpenAI](#openai), [xAI](#xai), [Alibaba](#alibaba-qwen)
- 实现 token bucket rate limiter，然后做分布式扩展。
  - 见于： [Anthropic](#anthropic), [OpenAI](#openai), [xAI](#xai), [Cohere](#cohere)
- 设计异步批处理器，处理 API 并发限制、抖动重试和错误隔离。
  - 见于： [Anthropic](#anthropic), [Perplexity](#perplexity)
- 实现带重叠的文本 chunker，确保不会截断语义单元。
  - 见于： [Harvey](#harvey)
- 实现 embedding 的余弦相似度检索，然后解释为什么不能直接上线。
- 最小化实现一个 agent loop，包含工具调度、错误处理和 step budget。
  - 见于： [Cognition](#cognition-devin-windsurf)

---

## 前沿 AI 实验室

### Anthropic

> **覆盖岗位：** Member of Technical Staff, Software Engineer, Research Engineer, Research Scientist, Applied AI Engineer, Forward Deployed Engineer, Performance Engineer, Product Engineer.
>
> **公开报道的面试流程：** 招聘官筛选 → 代码能力评估 → 虚拟 onsite（项目深挖、代码轮、系统设计、文化价值观） → 约 3 周到 2 个月。
>
> **重点准备：** 参考 [跨公司常见问题](#跨公司常见问题) 中标注 Anthropic 的内容，包括 LLM 内部机制、服务性能、Agent、评估、安全和系统设计。

#### 编码与数据结构

- 实现一个小型银行应用的核心业务逻辑，要求逐步扩展到更复杂版本。
- 实现一个内存数据库：支持 SET/GET/DELETE，随后增加过滤扫描、TTL 和文件压缩。
- 创建一个任务调度器。
- 构建一个管理课程、成绩和学生的 OOP 系统。
- 给定一个 URL 抓取助手，先写同步版，再做异步版。
- 将嵌套堆栈跟踪转换为离散的 start/end 事件。
- 设计速率限制器，并逐步加入多租户限制、突发额度和滑动窗口。
- 如果要对 50,000 份文档调用一个 LLM API，且并发限制约为 100，同时偶尔返回 429 和超时，如何用 Python 实现？

#### Inference / Serving / GPU

- 说明延迟、吞吐、队列和成本如何在大规模推理中权衡。

#### 安全与评估

- 设计一套能衡量 Claude 代理使用效果和可靠性的评估框架。

### OpenAI

> **覆盖岗位：** Research Engineer, Software Engineer, Applied AI Engineer, AI Safety Engineer, Product Engineer.
>
> **公开报道的面试流程：** 通常是筛选 + 编程/系统设计 + 项目深挖 + 文化和值观。
>
> **重点准备：** 参考 [跨公司常见问题](#跨公司常见问题) 中标注 OpenAI 的题目，包括推理、RAG、安全、Agents 与系统设计。

#### AI 系统设计

- 设计一个企业级 RAG 助手，支持权限控制和高可用性。
- 设计面向大规模用户的聊天服务栈，以及推理与缓存策略。

#### Safety

- 设计防注入、防越权、防数据泄露的安全架构。

### Google DeepMind 与 Google AI

> **覆盖岗位：** Research Engineer, ML Engineer, System Engineer, Applied Scientist.
>
> **重点准备：** Transformer 原理、推理性能、分布式训练、RAG、评估和大规模模型系统。

#### LLM 内部机制与架构

- 解释 Transformer 的核心构造、位置编码和注意力机制。
- 探讨大规模 MoE、分布式训练和模型扩展的工程实践。

### Meta（Superintelligence Labs、FAIR、Llama）

> **重点准备：** 训练与推理、MoE、优化、RAG、视觉/多模态、数据工程与大规模产品化。

### xAI

> **重点准备：** 低时延推理、数据结构、工程实现能力、真实产品构建能力。

### Mistral AI

> **重点准备：** 组合式 attention、MoE、模型量化、服务端工程、实际部署和企业场景。

### Cohere

> **重点准备：** RAG、检索、多语言、企业部署、评估和 AI agent 生产化。

### DeepSeek

> **重点准备：** MoE、推理优化、低精度训练、后训练与 RL、系统工程。

### Moonshot AI (Kimi)

> **重点准备：** 上下文窗口扩展、KV cache 压缩、MoE、大规模 agentic 评估和长上下文系统。

### Zhipu AI (GLM)

> **重点准备：** 预训练目标、MoE、长上下文、agentic coding、强化学习与评测。

### Alibaba (Qwen)

> **重点准备：** 多语言、长上下文、代码模型、大规模推理、VLM 和应用部署。

### Sarvam AI

> **重点准备：** 语音、语义、代码和低资源多语言模型。

---

## 大厂 AI 组织

### Microsoft

> **重点准备：** RAG、权限、AI gateway、企业 AI、工具调用与安全。

### Amazon (AWS)

> **重点准备：** 面向企业的生成式 AI、LLM 服务、性能与成本优化、真实场景设计。

### Apple

> **重点准备：** 模型量化、私有部署、推理优化、语音和多模态理解。

### NVIDIA

> **重点准备：** CUDA / kernel、GPU 性能、roofline reasoning、KV cache、TensorRT-LLM、模型服务。

### Tesla

> **重点准备：** 计算机视觉、3D 感知、自动驾驶工程、数据管道、模型部署和安全评估。

### 消费级规模 ML 公司（Uber、Netflix、LinkedIn、Airbnb、Pinterest、Spotify）

> **重点准备：** 排序、推荐、A/B 测试、在线评估、训练/在线偏差和大规模工程实践。

---

## AI 基础设施与平台公司

### Databricks

> **重点准备：** Spark、流式系统、数据工程、分布式平台、RAG 与企业 AI。 

### Groq

> **重点准备：** compiler、内存层次结构、低延迟 inference、空间数据流加速器、系统性能。

### Together AI

> **重点准备：** 连续批处理、serving scheduler、speculative decoding、成本控制和大规模 GPU 平台。

### Hugging Face

> **重点准备：** `transformers`、`datasets`、tokenizer、模型量化、Hub 系统、微调与开放生态。

### Scale AI

> **重点准备：** 数据质量、标注平台、评测、RLHF/DPO/GRPO、企业部署与 RL 环境设计。

### Perplexity

> **重点准备：** web-scale 检索、答案引擎、reranking、延迟预算、评估和安全验证。

---

## AI 原生产品公司

### Cursor (Anysphere)

> **重点准备：** 仓库索引、上下文检索、代码编辑 agent、成本优化、在线评估。

### Cognition (Devin, Windsurf)

> **重点准备：** coding agent、云端执行环境、评估、工具利用、基础设施与安全。

### Sierra

> **重点准备：** 客服 agent、guardrails、审批、流程自动化和 human-in-the-loop。

### Harvey

> **重点准备：** 法律文档检索、RAG、合同审查、证据与来源归因。

### Glean

> **重点准备：** 企业搜索、权限、连接器、GraphRAG、代理与工作流自动化。

### Character.AI

> **重点准备：** 长会话记忆、KV cache、对话风格、内容安全与参与度优化。

### ElevenLabs

> **重点准备：** TTS、ASR、实时语音、多模态语音 agent、低延迟架构和语音安全。

### Abridge

> **重点准备：** 医疗 ASR、诊疗文本生成、RAG、安全与隐私、病历结构化。

### Figure AI

> **重点准备：** 机器人学习、模仿学习、强化学习、sim-to-real、执行器控制和安全。

### Waymo

> **重点准备：** 感知、预测、规划、自动驾驶安全评估、模拟与运维。

---

## 前置部署与企业 AI

### Palantir

> **重点准备：** 分解问题、数据建模、SQL、API、企业工作流、AI agent 安全与生产治理。

---

### License

```
   Copyright (C) 2026 Outcome School

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
```

---

这份仓库已按中文内容结构进行了翻译整理，保留了原始链接和公司分类，方便你在阅读中文材料时同时对应原始英文来源。
