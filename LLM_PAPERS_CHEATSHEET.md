# LLM Papers Cheatsheet -- The Definitive Reading List

<div align="center">

  <p><strong>80+ essential research papers for understanding Large Language Models, organized by subdomain with importance signals.</strong><br/>From foundational Transformers to cutting-edge agents, evals, and inference optimization.</p>

  <a href="https://github.com/ombharatiya/FAANG-Coding-Interview-Questions/stargazers">
    <img src="https://img.shields.io/github/stars/ombharatiya/FAANG-Coding-Interview-Questions?style=flat" alt="GitHub stars" />
  </a>
  <a href="https://github.com/ombharatiya/FAANG-Coding-Interview-Questions/network/members">
    <img src="https://img.shields.io/github/forks/ombharatiya/FAANG-Coding-Interview-Questions?style=flat" alt="GitHub forks" />
  </a>

</div>

### How to Use This List

Each paper has an **importance signal** to help you prioritize:

| Signal | Meaning |
|--------|---------|
| **Essential** | Must-read. Foundational knowledge you'll be expected to know. |
| **Highly Influential** | Widely cited and referenced. Deep understanding gives you an edge. |
| **Interview Favorite** | Commonly discussed in ML/AI interviews at top companies. |
| **Cutting Edge** | Recent breakthrough. Shows you're tracking the frontier. |

---

## Table of Contents

- [Top 15 Must-Read Papers](#top-15-must-read-papers)
- [Foundational Architecture](#1-foundational-architecture)
- [Pre-training and Scaling Laws](#2-pre-training-and-scaling-laws)
- [Alignment, RLHF, and Preference Optimization](#3-alignment-rlhf-and-preference-optimization)
- [Safety, Red-Teaming, and Guardrails](#4-safety-red-teaming-and-guardrails)
- [Evaluation and Benchmarks](#5-evaluation-and-benchmarks)
- [Reasoning and Chain-of-Thought](#6-reasoning-and-chain-of-thought)
- [Retrieval-Augmented Generation (RAG)](#7-retrieval-augmented-generation-rag)
- [Agents and Tool Use](#8-agents-and-tool-use)
- [Fine-Tuning and Parameter-Efficient Methods](#9-fine-tuning-and-parameter-efficient-methods)
- [Inference Optimization](#10-inference-optimization)
- [Long Context and Positional Encoding](#11-long-context-and-positional-encoding)
- [Mixture of Experts (MoE)](#12-mixture-of-experts-moe)
- [Multimodal Models](#13-multimodal-models)
- [Code Generation](#14-code-generation)
- [Diffusion and Image Generation](#15-diffusion-and-image-generation)
- [Speech and Audio](#16-speech-and-audio)
- [Recommended Reading Order](#recommended-reading-order)
- [Resources](#resources)

---

## Top 15 Must-Read Papers

If you read nothing else, read these. They are the absolute essentials that every ML/AI engineer should know.

| # | Paper | Year | Why It Matters |
|---|-------|------|---------------|
| 1 | [Attention Is All You Need](https://arxiv.org/abs/1706.03762) (Vaswani et al.) | 2017 | Invented the Transformer. The paper that started everything. |
| 2 | [Language Models are Few-Shot Learners (GPT-3)](https://arxiv.org/abs/2005.14165) (Brown et al.) | 2020 | Proved scaling works. 175B parameters, few-shot capabilities. |
| 3 | [Training Language Models to Follow Instructions (InstructGPT)](https://arxiv.org/abs/2203.02155) (Ouyang et al.) | 2022 | RLHF for aligning models with human intent. The blueprint for ChatGPT. |
| 4 | [Scaling Laws for Neural Language Models](https://arxiv.org/abs/2001.08361) (Kaplan et al.) | 2020 | Mathematical relationships governing model scaling. Changed how labs plan training. |
| 5 | [Training Compute-Optimal LLMs (Chinchilla)](https://arxiv.org/abs/2203.15556) (Hoffmann et al.) | 2022 | Showed most models were undertrained. Reshaped all subsequent training decisions. |
| 6 | [LoRA: Low-Rank Adaptation](https://arxiv.org/abs/2106.09685) (Hu et al.) | 2021 | 10,000x fewer trainable params. Made fine-tuning accessible to everyone. |
| 7 | [FlashAttention](https://arxiv.org/abs/2205.14135) (Dao et al.) | 2022 | IO-aware exact attention. 2-4x faster. Now standard in every inference stack. |
| 8 | [Chain-of-Thought Prompting](https://arxiv.org/abs/2201.11903) (Wei et al.) | 2022 | Unlocked reasoning in LLMs through step-by-step prompting. |
| 9 | [RAG: Retrieval-Augmented Generation](https://arxiv.org/abs/2005.11401) (Lewis et al.) | 2020 | Combined retrieval with generation. Foundation of every enterprise LLM app. |
| 10 | [ReAct: Reasoning and Acting](https://arxiv.org/abs/2210.03629) (Yao et al.) | 2022 | Interleaved reasoning + tool use. The blueprint for AI agents. |
| 11 | [Constitutional AI](https://arxiv.org/abs/2212.08073) (Bai et al.) | 2022 | AI self-critique for safety. Anthropic's foundational alignment approach. |
| 12 | [DPO: Direct Preference Optimization](https://arxiv.org/abs/2305.18290) (Rafailov et al.) | 2023 | Simplified RLHF into a classification loss. Now widely adopted. |
| 13 | [LLaMA: Open and Efficient Foundation Models](https://arxiv.org/abs/2302.13971) (Touvron et al.) | 2023 | Democratized open-source LLMs. Spawned the entire open-weights ecosystem. |
| 14 | [CLIP: Connecting Vision and Language](https://arxiv.org/abs/2103.00020) (Radford et al.) | 2021 | Bridged vision and language with contrastive learning. Foundation for multimodal AI. |
| 15 | [Efficient Memory Management with PagedAttention (vLLM)](https://arxiv.org/abs/2309.06180) (Kwon et al.) | 2023 | KV cache as virtual memory. 2-4x serving throughput. Industry-standard inference. |

---

## 1. Foundational Architecture

The building blocks everything else rests on.

| Paper | Authors | Year | Signal | Key Contribution |
|-------|---------|------|--------|-----------------|
| [Attention Is All You Need](https://arxiv.org/abs/1706.03762) | Vaswani et al. | 2017 | **Essential** | Introduced the Transformer architecture -- self-attention, multi-head attention, positional encoding |
| [BERT: Pre-training of Deep Bidirectional Transformers](https://arxiv.org/abs/1810.04805) | Devlin et al. | 2018 | **Essential** | Bidirectional encoders, masked language modeling, next sentence prediction |
| [Improving Language Understanding by Generative Pre-Training (GPT)](https://cdn.openai.com/research-covers/language-unsupervised/language_understanding_paper.pdf) | Radford et al. | 2018 | **Highly Influential** | First GPT model -- generative pre-training + discriminative fine-tuning |
| [Language Models are Unsupervised Multitask Learners (GPT-2)](https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf) | Radford et al. | 2019 | **Highly Influential** | Zero-shot task transfer, scaling to 1.5B parameters |
| [Language Models are Few-Shot Learners (GPT-3)](https://arxiv.org/abs/2005.14165) | Brown et al. | 2020 | **Essential** | 175B parameters, in-context learning, few-shot capabilities |
| [GPT-4 Technical Report](https://arxiv.org/abs/2303.08774) | OpenAI | 2023 | **Interview Favorite** | Multimodal capabilities, RLHF improvements, safety mitigations |

## 2. Pre-training and Scaling Laws

How models learn and why bigger (sometimes) means better.

| Paper | Authors | Year | Signal | Key Contribution |
|-------|---------|------|--------|-----------------|
| [Scaling Laws for Neural Language Models](https://arxiv.org/abs/2001.08361) | Kaplan et al. | 2020 | **Essential** | Power-law relationships between compute, data, model size, and loss |
| [Training Compute-Optimal LLMs (Chinchilla)](https://arxiv.org/abs/2203.15556) | Hoffmann et al. | 2022 | **Essential** | Optimal compute allocation: most models were undertrained on data |
| [PaLM: Scaling Language Modeling with Pathways](https://arxiv.org/abs/2204.02311) | Chowdhery et al. | 2022 | **Highly Influential** | 540B parameters, Pathways distributed compute, breakthrough reasoning |
| [LLaMA: Open and Efficient Foundation Language Models](https://arxiv.org/abs/2302.13971) | Touvron et al. | 2023 | **Essential** | Proved smaller models with more data compete with larger ones. Open-sourced. |
| [Llama 2: Open Foundation and Fine-Tuned Chat Models](https://arxiv.org/abs/2307.09288) | Touvron et al. | 2023 | **Interview Favorite** | Safety improvements, RLHF at scale, detailed training methodology |
| [LaMDA: Language Models for Dialog Applications](https://arxiv.org/abs/2201.08239) | Thoppilan et al. | 2022 | **Highly Influential** | Dialogue-focused pre-training, safety and grounding metrics |
| [Mistral 7B](https://arxiv.org/abs/2310.06825) | Mistral AI | 2023 | **Cutting Edge** | Sliding window attention, grouped-query attention, outperforms LLaMA 2 13B |

## 3. Alignment, RLHF, and Preference Optimization

Teaching models to be helpful, harmless, and honest.

| Paper | Authors | Year | Signal | Key Contribution |
|-------|---------|------|--------|-----------------|
| [Deep RL from Human Preferences](https://arxiv.org/abs/1706.03741) | Christiano et al. | 2017 | **Highly Influential** | Original RLHF formulation -- reward model learned from human comparisons |
| [Training Language Models to Follow Instructions (InstructGPT)](https://arxiv.org/abs/2203.02155) | Ouyang et al. | 2022 | **Essential** | Applied RLHF to GPT-3. The paper behind ChatGPT's alignment approach |
| [Constitutional AI: Harmlessness from AI Feedback](https://arxiv.org/abs/2212.08073) | Bai et al. | 2022 | **Essential** | AI self-critique using principles (CAI). Anthropic's safety foundation |
| [Direct Preference Optimization (DPO)](https://arxiv.org/abs/2305.18290) | Rafailov et al. | 2023 | **Essential** | Eliminates reward model -- optimizes policy directly from preferences via classification loss |
| [Finetuned Language Models Are Zero-Shot Learners (FLAN)](https://arxiv.org/abs/2109.01652) | Wei et al. | 2021 | **Highly Influential** | Instruction tuning across 60+ tasks. Surpassed GPT-3 zero-shot on 20/25 tasks |
| [Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca) | Taori et al. | 2023 | **Interview Favorite** | 52K self-instruct examples to fine-tune LLaMA-7B. Sparked open instruction-tuning movement |

## 4. Safety, Red-Teaming, and Guardrails

Preventing misuse and understanding failure modes.

| Paper | Authors | Year | Signal | Key Contribution |
|-------|---------|------|--------|-----------------|
| [Red Teaming Language Models with Language Models](https://arxiv.org/abs/2202.03286) | Perez et al. | 2022 | **Interview Favorite** | Automated adversarial testing using LLMs to find LLM vulnerabilities |
| [Sleeper Agents: Training Deceptive LLMs](https://arxiv.org/abs/2401.05566) | Hubinger et al. | 2024 | **Cutting Edge** | Backdoor behaviors persist through safety training. Adversarial training may make deception stealthier |
| [TruthfulQA: Measuring How Models Mimic Human Falsehoods](https://arxiv.org/abs/2109.07958) | Lin et al. | 2021 | **Interview Favorite** | 817 questions designed to elicit common misconceptions. Best model: 58% truthful vs 94% human |
| [Llama 2: Safety and RLHF Details](https://arxiv.org/abs/2307.09288) | Touvron et al. | 2023 | **Highly Influential** | Most detailed public description of safety RLHF training at scale |

## 5. Evaluation and Benchmarks

How we measure what LLMs actually know and can do. This is a critical gap in many reading lists.

| Paper | Authors | Year | Signal | Key Contribution |
|-------|---------|------|--------|-----------------|
| [Measuring Massive Multitask Language Understanding (MMLU)](https://arxiv.org/abs/2009.03300) | Hendrycks et al. | 2020 | **Essential** | 57 subjects from STEM to humanities. The standard knowledge benchmark |
| [Holistic Evaluation of Language Models (HELM)](https://arxiv.org/abs/2211.09110) | Liang et al. | 2022 | **Highly Influential** | Standardized evaluation across 42 scenarios, 7 metrics. Framework for fair comparison |
| [Chatbot Arena: Evaluating LLMs by Human Preference](https://arxiv.org/abs/2403.04132) | Chiang, Zheng et al. | 2024 | **Essential** | Crowdsourced pairwise comparisons (240K+ votes). The Elo leaderboard everyone watches |
| [Beyond the Imitation Game (BIG-bench)](https://arxiv.org/abs/2206.04615) | Srivastava et al. | 2022 | **Highly Influential** | 204 tasks from 450 authors. Best model surpassed average human on 65% of tasks |
| [Sparks of AGI: Early Experiments with GPT-4](https://arxiv.org/abs/2303.12712) | Bubeck et al. | 2023 | **Interview Favorite** | Analysis of emergent abilities: theory of mind, spatial reasoning, planning |
| [Emergent Abilities of Large Language Models](https://arxiv.org/abs/2206.07682) | Wei et al. | 2022 | **Highly Influential** | Catalogued capabilities that appear suddenly at scale (arithmetic, word unscrambling) |
| [Evaluating Large Language Models Trained on Code (HumanEval)](https://arxiv.org/abs/2107.03374) | Chen et al. | 2021 | **Interview Favorite** | 164 hand-written programming tasks. Standard benchmark for code generation |
| [GPQA: A Graduate-Level Google-Proof Q&A Benchmark](https://arxiv.org/abs/2311.12022) | Rein et al. | 2023 | **Cutting Edge** | Expert-level questions where domain experts scored 65%, non-experts 34% even with Google |
| [Let's Verify Step by Step](https://arxiv.org/abs/2305.20050) | Lightman et al. | 2023 | **Cutting Edge** | Process supervision (reward per step) significantly outperforms outcome supervision for math |

## 6. Reasoning and Chain-of-Thought

Making LLMs think before they answer.

| Paper | Authors | Year | Signal | Key Contribution |
|-------|---------|------|--------|-----------------|
| [Chain-of-Thought Prompting Elicits Reasoning](https://arxiv.org/abs/2201.11903) | Wei et al. | 2022 | **Essential** | Step-by-step reasoning examples in prompts dramatically improve math and logic tasks |
| [Self-Consistency Improves Chain of Thought Reasoning](https://arxiv.org/abs/2203.11171) | Wang et al. | 2022 | **Highly Influential** | Sample diverse reasoning paths + majority vote. +17.9% on GSM8K over greedy CoT |
| [Tree of Thoughts: Deliberate Problem Solving](https://arxiv.org/abs/2305.10601) | Yao et al. | 2023 | **Interview Favorite** | Generalizes CoT with tree search -- lookahead, backtracking, and evaluation |
| [Let's Verify Step by Step](https://arxiv.org/abs/2305.20050) | Lightman et al. | 2023 | **Cutting Edge** | Process reward models: supervise each reasoning step, not just the final answer |

## 7. Retrieval-Augmented Generation (RAG)

Grounding LLMs in external knowledge. The backbone of enterprise AI.

| Paper | Authors | Year | Signal | Key Contribution |
|-------|---------|------|--------|-----------------|
| [Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks](https://arxiv.org/abs/2005.11401) | Lewis et al. | 2020 | **Essential** | The original RAG paper: DPR retriever + BART generator, jointly trained end-to-end |
| [REALM: Retrieval-Augmented Language Model Pre-Training](https://arxiv.org/abs/2002.08909) | Guu et al. | 2020 | **Highly Influential** | Pre-trains retriever jointly with masked LM. Outperformed prior Open-QA by 4-16% |
| [Self-RAG: Learning to Retrieve, Generate, and Critique](https://arxiv.org/abs/2310.11511) | Asai et al. | 2023 | **Cutting Edge** | LM decides when to retrieve via special tokens, then self-reflects on relevance and quality |
| [CLIP: Connecting Vision and Language](https://arxiv.org/abs/2103.00020) | Radford et al. | 2021 | **Essential** | Contrastive language-image pre-training. Foundation for multimodal retrieval and embeddings |

## 8. Agents and Tool Use

LLMs that take actions in the real world.

| Paper | Authors | Year | Signal | Key Contribution |
|-------|---------|------|--------|-----------------|
| [ReAct: Synergizing Reasoning and Acting](https://arxiv.org/abs/2210.03629) | Yao et al. | 2022 | **Essential** | Interleaves reasoning traces + tool actions. Reduces hallucination via grounded interaction |
| [Toolformer: LMs Can Teach Themselves to Use Tools](https://arxiv.org/abs/2302.04761) | Schick et al. | 2023 | **Highly Influential** | Self-supervised tool-use learning. LM decides when to call calculator, search, etc. |
| [Generative Agents: Interactive Simulacra of Human Behavior](https://arxiv.org/abs/2304.03442) | Park et al. | 2023 | **Cutting Edge** | 25 LLM agents with memory, reflection, and planning in a sandbox world |
| [Voyager: Open-Ended Embodied Agent with LLMs](https://arxiv.org/abs/2305.16291) | Wang et al. | 2023 | **Cutting Edge** | GPT-4 Minecraft agent with auto-curriculum and skill library. 3.3x more items than prior SOTA |

## 9. Fine-Tuning and Parameter-Efficient Methods

Making adaptation affordable and practical.

| Paper | Authors | Year | Signal | Key Contribution |
|-------|---------|------|--------|-----------------|
| [LoRA: Low-Rank Adaptation of Large Language Models](https://arxiv.org/abs/2106.09685) | Hu et al. | 2021 | **Essential** | Inject trainable low-rank matrices into frozen layers. 10,000x fewer params, no inference overhead |
| [QLoRA: Efficient Finetuning of Quantized LLMs](https://arxiv.org/abs/2305.14314) | Dettmers et al. | 2023 | **Essential** | Fine-tune 65B model on single 48GB GPU via 4-bit quantization + LoRA |
| [Prefix-Tuning: Optimizing Continuous Prompts](https://arxiv.org/abs/2101.00190) | Li & Liang | 2021 | **Highly Influential** | Freeze LM, optimize tiny continuous prefix (0.1% of params). Predecessor to prompt tuning |
| [Finetuned Language Models Are Zero-Shot Learners (FLAN)](https://arxiv.org/abs/2109.01652) | Wei et al. | 2021 | **Highly Influential** | Instruction tuning across 60+ tasks. Showed multi-task fine-tuning generalizes to unseen tasks |
| [Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca) | Taori et al. | 2023 | **Interview Favorite** | 52K self-instruct examples fine-tuned LLaMA-7B. Democratized instruction tuning |

## 10. Inference Optimization

Making models fast and cheap enough to actually deploy.

| Paper | Authors | Year | Signal | Key Contribution |
|-------|---------|------|--------|-----------------|
| [FlashAttention: Fast and Memory-Efficient Exact Attention](https://arxiv.org/abs/2205.14135) | Dao et al. | 2022 | **Essential** | IO-aware tiling for exact attention. 2-4x speedup, longer sequences, no approximation |
| [FlashAttention-2: Faster Attention with Better Parallelism](https://arxiv.org/abs/2307.08691) | Dao | 2023 | **Highly Influential** | Improved work partitioning. 50-73% of theoretical max FLOPs on A100 |
| [Efficient Memory Management with PagedAttention (vLLM)](https://arxiv.org/abs/2309.06180) | Kwon et al. | 2023 | **Essential** | KV cache as virtual memory pages. 2-4x serving throughput. Industry standard |
| [Speculative Decoding](https://arxiv.org/abs/2211.17192) | Leviathan et al. | 2022 | **Interview Favorite** | Small draft model proposes tokens, large model verifies in parallel. 2-3x speedup, identical output |
| [GPTQ: Accurate Post-Training Quantization](https://arxiv.org/abs/2210.17323) | Frantar et al. | 2022 | **Highly Influential** | One-shot weight quantization to 3-4 bits. Quantizes 175B model in ~4 GPU hours |
| [AWQ: Activation-aware Weight Quantization](https://arxiv.org/abs/2306.00978) | Lin et al. | 2023 | **Interview Favorite** | Protects 1% salient channels via activation-aware scaling. Efficient 4-bit quantization |
| [Medusa: Simple LLM Inference Acceleration](https://arxiv.org/abs/2401.10774) | Cai et al. | 2024 | **Cutting Edge** | Multiple decoding heads predict future tokens in parallel. Lossless acceleration |

## 11. Long Context and Positional Encoding

Extending what models can see and remember.

| Paper | Authors | Year | Signal | Key Contribution |
|-------|---------|------|--------|-----------------|
| [RoFormer: Enhanced Transformer with Rotary Position Embedding (RoPE)](https://arxiv.org/abs/2104.09864) | Su et al. | 2021 | **Essential** | Rotation matrices encode position. Used in LLaMA, Mistral, and most modern LLMs |
| [ALiBi: Attention with Linear Biases](https://arxiv.org/abs/2108.12409) | Press et al. | 2021 | **Highly Influential** | Linear bias on attention scores replaces positional embeddings. Enables length extrapolation |
| [Ring Attention with Blockwise Transformers](https://arxiv.org/abs/2310.01889) | Liu et al. | 2023 | **Cutting Edge** | Distributes sequences across devices in ring topology. Near-infinite context |
| [Mamba: Linear-Time Sequence Modeling with Selective State Spaces](https://arxiv.org/abs/2312.00752) | Gu & Dao | 2023 | **Cutting Edge** | Replaces attention with selective SSM layers. Linear-time inference, 5x throughput |

## 12. Mixture of Experts (MoE)

Scaling model capacity without scaling compute.

| Paper | Authors | Year | Signal | Key Contribution |
|-------|---------|------|--------|-----------------|
| [Switch Transformers: Scaling to Trillion Parameter Models](https://arxiv.org/abs/2101.03961) | Fedus et al. | 2022 | **Highly Influential** | Simplified MoE routing. 7x pre-training speedup with same compute budget |
| [Mixtral of Experts](https://arxiv.org/abs/2401.04088) | Mistral AI | 2024 | **Cutting Edge** | 8x7B experts (47B total, 13B active). Outperforms Llama 2 70B, matches GPT-3.5 |

## 13. Multimodal Models

Beyond text -- vision, audio, and cross-modal understanding.

| Paper | Authors | Year | Signal | Key Contribution |
|-------|---------|------|--------|-----------------|
| [CLIP: Learning Transferable Visual Models from Natural Language](https://arxiv.org/abs/2103.00020) | Radford et al. | 2021 | **Essential** | Contrastive language-image pre-training. Zero-shot image classification |
| [DALL-E 2: Hierarchical Text-Conditional Image Generation](https://arxiv.org/abs/2204.06125) | Ramesh et al. | 2022 | **Highly Influential** | Text-to-image via CLIP latents and diffusion. Set the quality bar for image generation |
| [Flamingo: Visual Language Model for Few-Shot Learning](https://arxiv.org/abs/2204.14198) | Alayrac et al. | 2022 | **Highly Influential** | Bridges frozen vision encoder + frozen LLM with gated cross-attention. Few-shot visual learning |
| [Visual Instruction Tuning (LLaVA)](https://arxiv.org/abs/2304.08485) | Liu et al. | 2023 | **Interview Favorite** | Connects CLIP to LLM via visual instruction tuning. 85.1% relative score vs GPT-4 on multimodal chat |
| [Gemini: A Family of Highly Capable Multimodal Models](https://arxiv.org/abs/2312.11805) | Google | 2023 | **Cutting Edge** | Natively multimodal architecture. Text, image, audio, video in a single model |

## 14. Code Generation

LLMs that write, understand, and fix code.

| Paper | Authors | Year | Signal | Key Contribution |
|-------|---------|------|--------|-----------------|
| [Evaluating LLMs Trained on Code (Codex / HumanEval)](https://arxiv.org/abs/2107.03374) | Chen et al. | 2021 | **Essential** | 164 programming tasks benchmark. Codex (GPT fine-tuned on code) solves 28.8% |
| [Competition-Level Code Generation with AlphaCode](https://arxiv.org/abs/2203.07814) | Li et al. | 2022 | **Highly Influential** | Massive sampling + filtering. Top-54% among 5,000+ Codeforces competitors |
| [StarCoder: May the Source Be With You](https://arxiv.org/abs/2305.06161) | Li et al. | 2023 | **Interview Favorite** | 15.5B open code LM. 1T tokens from The Stack. Matches OpenAI code-cushman-001 |
| [Code Llama: Open Foundation Models for Code](https://arxiv.org/abs/2308.12950) | Roziere et al. | 2023 | **Interview Favorite** | 7B-70B code models with infilling and 100K context. 67% on HumanEval |
| [SWE-bench: Can LMs Resolve Real-World GitHub Issues?](https://arxiv.org/abs/2310.06770) | Jimenez et al. | 2023 | **Cutting Edge** | 2,294 real GitHub issues. Tests end-to-end software engineering, not just function generation |

## 15. Diffusion and Image Generation

The generative AI revolution beyond text.

| Paper | Authors | Year | Signal | Key Contribution |
|-------|---------|------|--------|-----------------|
| [Denoising Diffusion Probabilistic Models (DDPM)](https://arxiv.org/abs/2006.11239) | Ho et al. | 2020 | **Essential** | Established diffusion models for image synthesis. FID 3.17 on CIFAR-10 |
| [High-Resolution Image Synthesis with Latent Diffusion (Stable Diffusion)](https://arxiv.org/abs/2112.10752) | Rombach et al. | 2021 | **Essential** | Diffusion in learned latent space with cross-attention conditioning. Drastically reduced compute |
| [DALL-E 2: Hierarchical Text-Conditional Image Generation](https://arxiv.org/abs/2204.06125) | Ramesh et al. | 2022 | **Highly Influential** | CLIP latents + diffusion for controllable, high-quality text-to-image |

## 16. Speech and Audio

Extending LLMs to the audio domain.

| Paper | Authors | Year | Signal | Key Contribution |
|-------|---------|------|--------|-----------------|
| [Robust Speech Recognition via Large-Scale Weak Supervision (Whisper)](https://arxiv.org/abs/2212.04356) | Radford et al. | 2022 | **Essential** | 680K hours multilingual audio. Zero-shot speech recognition competitive with supervised models |

---

## Recommended Reading Order

### Beginner Track (Start Here)
1. **Attention Is All You Need** -- Understand the Transformer
2. **GPT / GPT-2** -- Understand generative pre-training
3. **GPT-3** -- Understand scaling and in-context learning
4. **InstructGPT** -- Understand RLHF and alignment
5. **LoRA** -- Understand efficient fine-tuning
6. **Chain-of-Thought Prompting** -- Understand reasoning

### Intermediate Track (Building Depth)
7. **Chinchilla** -- Scaling laws and compute-optimal training
8. **LLaMA + Llama 2** -- Open-source models and safety
9. **RAG** -- Retrieval-augmented generation
10. **FlashAttention** -- Inference optimization
11. **MMLU + HELM** -- How we evaluate models
12. **CLIP** -- Multimodal foundations

### Advanced Track (Cutting Edge)
13. **DPO** -- Modern alignment without reward models
14. **ReAct + Toolformer** -- Agents and tool use
15. **Speculative Decoding + vLLM** -- Production inference
16. **Self-RAG** -- Advanced retrieval
17. **Mamba** -- Alternatives to attention
18. **Sleeper Agents** -- AI safety research

---

## Resources

- [Hugging Face Model Hub](https://huggingface.co/models) -- Repository of thousands of pre-trained models
- [Papers With Code](https://paperswithcode.com/task/language-modelling) -- LLM papers with implementation code
- [Chatbot Arena Leaderboard](https://chat.lmsys.org/?leaderboard) -- Live Elo rankings from human evaluations
- [Stanford CS324: Large Language Models](https://stanford-cs324.github.io/winter2022/) -- University course materials
- [State of AI Report](https://www.stateof.ai/) -- Annual report on AI progress
- [Anthropic Research](https://www.anthropic.com/research) -- Safety and alignment research
- [OpenAI Research](https://openai.com/research) -- Frontier model research

---

<div align="center">

### 🔔 You Found the Shortcut. Don't Lose It.

New questions, papers, and strategies drop here **every single week** — before they surface anywhere else.

The engineers who land FAANG offers aren't the ones who *find* a resource — they're the ones who **never lose it**.

⚡ **One click. Every update. Zero effort.**

<a href="https://github.com/ombharatiya/FAANG-Coding-Interview-Questions/subscription">
  <img src="https://img.shields.io/badge/🔔 Watch This Repo-Get Every Update-blue?style=for-the-badge" alt="Watch Repo" />
</a>&nbsp;
<a href="https://github.com/ombharatiya/FAANG-Coding-Interview-Questions">
  <img src="https://img.shields.io/badge/⭐ Star-Show Support-yellow?style=for-the-badge" alt="Star Repo" />
</a>

**Follow [@ombharatiya](https://github.com/ombharatiya)** for exclusive tips, paper breakdowns, and career moves that never make it into the repo:

[![GitHub](https://img.shields.io/badge/GitHub-@ombharatiya-181717?style=flat-square&logo=github)](https://github.com/ombharatiya)
[![Twitter](https://img.shields.io/badge/Twitter-@ombharatiya-1DA1F2?style=flat-square&logo=twitter)](https://twitter.com/ombharatiya)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-ombharatiya-0A66C2?style=flat-square&logo=linkedin)](https://linkedin.com/in/ombharatiya)

</div>
