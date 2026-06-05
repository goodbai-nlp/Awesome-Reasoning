# ⚡ Efficient Reasoning

Papers about making reasoning cheaper, shorter, faster, or easier to deploy. This category covers concise reasoning, overthinking reduction, early stopping, token pruning, model compression, small reasoning models, and efficiency-aware evaluation.

# Bookmarks

- [Surveys & Roadmaps](#surveys--roadmaps)
- [Short / Compressed CoT](#short--compressed-cot)
- [Overthinking Reduction](#overthinking-reduction)
- [Early Stopping & Adaptive Exit](#early-stopping--adaptive-exit)
- [Token / KV / Memory Optimization](#token--kv--memory-optimization)
- [Distillation & Small Reasoning Models](#distillation--small-reasoning-models)
- [Efficient Multimodal Reasoning](#efficient-multimodal-reasoning)
- [Efficiency Benchmarks](#efficiency-benchmarks)

## Surveys & Roadmaps

| Year | Title | Venue | Paper | Code/Data | Tags | Note |
| ---- | ----- | ----- | :---: | :-------: | ---- | ---- |
| 2026 | The Latent Space: Foundation, Evolution, Mechanism, Ability, and Outlook | arXiv | [📄](https://arxiv.org/abs/2604.02029) | [📦](https://github.com/YU-deep/Awesome-Latent-Space) | `survey`, `latent-space` | Unified latent-space survey across foundation, evolution, mechanism, ability, and outlook. |
| 2025 | Implicit Reasoning in Large Language Models: A Comprehensive Survey | arXiv | [📄](https://arxiv.org/abs/2509.02350) | [📦](https://github.com/digailab/awesome-llm-implicit-reasoning) | `survey`, `efficient-reasoning` | Taxonomy of implicit reasoning by execution paradigm: latent optimization, signal-guided control, and layer-recurrent execution. |
| 2025 | A Survey on Latent Reasoning | arXiv | [📄](https://arxiv.org/abs/2507.06203) | [📦](https://github.com/multimodal-art-projection/LatentCoT-Horizon) | `survey`, `latent-cot` | Organizes latent reasoning into vertical recurrence and horizontal recurrence, plus fine-tuning strategies that internalize explicit traces. |
| 2025 | Thinking with Images for Multimodal Reasoning: Foundations, Methods, and Future Frontiers | arXiv | [📄](https://arxiv.org/abs/2506.23918) | [📦](https://github.com/zhaochen0110/Awesome_Think_With_Images) | `survey`, `multimodal`, `think-with-images` | Surveys the shift from thinking about images to thinking with images as a dynamic cognitive workspace. |
| 2025 | Reasoning Beyond Language: A Comprehensive Survey on Latent Chain-of-Thought Reasoning | arXiv | [📄](https://arxiv.org/abs/2505.16782) | [📦](https://github.com/EIT-NLP/Awesome-Latent-CoT) | `survey`, `latent-cot` | Latent CoT taxonomy from token-wise horizontal methods to layer-wise vertical strategies, with analysis and applications. |
| 2025 | Perception, Reason, Think, and Plan: A Survey on Large Multimodal Reasoning Models | arXiv | [📄](https://arxiv.org/abs/2505.04921) | [📦](https://github.com/HITsz-TMG/Awesome-Large-Multimodal-Reasoning-Models) | `survey`, `multimodal` | Four-stage roadmap of large multimodal reasoning models from modular pipelines to native agentic reasoning. |
| 2025 | Efficient Reasoning Models: A Survey | arXiv | [📄](https://arxiv.org/abs/2504.10903) | [📦](https://github.com/fscdc/Awesome-Efficient-Reasoning-Models) | `survey`, `efficient-reasoning` | Categorizes efficient reasoning into shorter CoT, smaller models, and faster decoding. |
| 2025 | Harnessing the Reasoning Economy | arXiv | [📄](https://arxiv.org/abs/2503.24377) | [📦](https://github.com/DevoAllen/Awesome-Reasoning-Economy-Papers) | `survey`, `reasoning-economy` | Surveys reasoning economy across cost, token budget, latency, and deployment trade-offs. |
| 2025 | Stop Overthinking: A Survey on Efficient Reasoning for Large Language Models | TMLR 2025 | [📄](https://arxiv.org/abs/2503.16419) | [📦](https://github.com/Eclipsess/Awesome-Efficient-Reasoning-LLMs) | `survey`, `efficient-reasoning`, `overthinking` | Broad survey of efficient LLM reasoning, including concise reasoning and overthinking reduction. |
| 2025 | Multimodal Chain-of-Thought Reasoning: A Comprehensive Survey | arXiv | [📄](https://arxiv.org/abs/2503.12605) | [📦](https://github.com/yaotingwangofficial/Awesome-MCoT) | `survey`, `multimodal` | First systematic survey of multimodal CoT across image, video, audio, 3D, and structured data. |

[Back](#bookmarks)

## Short / Compressed CoT

Implicit, latent, soft, or hidden reasoning that replaces long explicit chain-of-thought.

| Year | Title | Venue | Paper | Code/Data | Tags | Note |
| ---- | ----- | ----- | :---: | :-------: | ---- | ---- |
| 2026 | SeLaR: Selective Latent Reasoning in Large Language Models | ACL 2026 | [📄](https://arxiv.org/abs/2604.08299) | — | `method`, `soft-readout`, `autoregressive`, `parallel` | Entropy-gated soft embeddings at low-confidence steps for efficient multi-path latent exploration. |
| 2026 | Latent Thoughts Tuning | arXiv | [📄](https://arxiv.org/abs/2602.10229) | — | `method`, `hidden-state`, `autoregressive`, `routing` | Fuses context and prediction to construct stable latent thoughts for implicit reasoning. |
| 2026 | LatentChem: From Textual CoT to Latent Thinking in Chemical Reasoning | ICML 2026 | [📄](https://arxiv.org/abs/2602.07075) | — | `method`, `hidden-state`, `autoregressive`, `compression` | Internalizes textual chemical CoT into continuous latent thinking. |
| 2026 | ThinkRouter | arXiv | [📄](https://arxiv.org/abs/2602.11683) | — | `method`, `hidden-state`, `autoregressive`, `routing` | Routes between latent and discrete thinking modes for efficient inference. |
| 2026 | Latent Reasoning with Supervised Thinking States | arXiv | [📄](https://arxiv.org/abs/2602.08332) | — | `method`, `hidden-state`, `autoregressive`, `compression` | Supervised thinking states carry intermediate reasoning in hidden space. |
| 2026 | Latent Chain-of-Thought as Planning: Decoupling Reasoning from Verbalization | arXiv | [📄](https://arxiv.org/abs/2601.21358) | [📦](https://github.com/zz1358m/ATP-Latent-master) | `method`, `hidden-state`, `autoregressive`, `routing` | Formulates latent CoT as planning decoupled from verbalization. |
| 2026 | iCLP: Large Language Model Reasoning with Implicit Cognition Latent Planning | arXiv | [📄](https://arxiv.org/abs/2512.24014) | [📦](https://github.com/AgenticFinLab/latent-planning) | `method`, `hidden-state`, `autoregressive`, `routing`, `distillation` | VQ latent plans distilled from explicit plans for implicit inference-time planning. |
| 2026 | JEPA-Reasoner: Decoupling Latent Reasoning from Token Generation | arXiv | [📄](https://arxiv.org/abs/2512.19171) | — | `method`, `hidden-state`, `autoregressive`, `routing` | JEPA engine reasons in continuous space; Talker decodes text without token error backflow. |
| 2026 | Dynamic Large Concept Models: Latent Reasoning in an Adaptive Semantic Space | arXiv | [📄](https://arxiv.org/abs/2512.24617) | — | `method`, `soft-readout`, `autoregressive`, `concept-embedding` | Semantic-level latent reasoning in an adaptive concept space. |
| 2025 | SemCoT | NeurIPS 2025 | [📄](https://proceedings.neurips.cc/paper_files/paper/2025/file/3ddbd473456a57e3cafb1ee51ddf8ff6-Paper-Conference.pdf) | [📦](https://github.com/YinhanHe123/SemCoT) | `method`, `soft-readout`, `autoregressive`, `compression` | Semantically aligned implicit tokens compress explicit CoT. |
| 2025 | Latent Reasoning in LLMs as a Vocabulary-Space Superposition | arXiv | [📄](https://arxiv.org/abs/2510.15522) | [📦](https://github.com/DJC-GO-SOLO/Latent-SFT) | `method`, `soft-readout`, `autoregressive`, `compression` | Maps latent thoughts to vocabulary-space superpositions. |
| 2025 | Lightweight Latent Reasoning for Narrative Tasks (LiteReason) | arXiv | [📄](https://arxiv.org/abs/2512.02240) | — | `method`, `soft-readout`, `autoregressive`, `compression` | Reasoning projector emits continuous latent tokens interleaved with discrete sampling. |
| 2025 | R-Capsule: Compressing High-Level Plans for Efficient LLM Reasoning | arXiv | [📄](https://arxiv.org/abs/2509.22131) | — | `method`, `hidden-state`, `autoregressive`, `compression` | Compresses high-level plans into compact reconstructible reasoning capsules. |
| 2025 | LTA-thinker: Latent Thought-Augmented Training Framework for LLMs | arXiv | [📄](https://arxiv.org/abs/2509.12875) | — | `method`, `hidden-state`, `autoregressive`, `compression` | Learnable priors and distribution-direction losses enhance latent thought training. |
| 2025 | MARCOS: Deep Thinking by Markov Chain of Continuous Thoughts | arXiv | [📄](https://arxiv.org/abs/2509.25020) | — | `method`, `soft-readout`, `parallel` | Models reasoning as a Markov chain of continuous thoughts with variational training. |
| 2025 | Learning to Reason with Mixture of Tokens (MoT-G) | arXiv | [📄](https://arxiv.org/abs/2509.21482) | — | `method`, `soft-readout`, `parallel` | Continuous token-mixture reasoning under RLVR for higher-entropy exploration. |
| 2025 | Fast Thinking for Large Language Models | arXiv | [📄](https://arxiv.org/abs/2509.23633) | — | `method`, `soft-readout`, `autoregressive`, `concept-embedding` | Latent codebooks plus GainRouter enable single-pass strategy routing via continuous thoughts. |
| 2025 | Soft Tokens, Hard Truths | arXiv | [📄](https://arxiv.org/abs/2509.19170) | — | `method`, `soft-readout`, `parallel` | Weighted embeddings and soft tokens for implicit distributional reasoning. |
| 2025 | SynAdapt: Learning Adaptive Reasoning via Synthetic Continuous CoT | arXiv | [📄](https://arxiv.org/abs/2508.00574) | — | `method`, `soft-readout`, `autoregressive`, `compression` | Synthetic continuous CoT alignment with difficulty-aware rethinking. |
| 2025 | Enhancing Latent Computation in Transformers with Latent Tokens | arXiv | [📄](https://arxiv.org/abs/2505.12629) | — | `method`, `soft-readout`, `autoregressive`, `concept-embedding` | Learnable dummy latent tokens guide implicit computation during decoding. |
| 2025 | Hybrid Latent Reasoning via Reinforcement Learning | NeurIPS 2025 | [📄](https://openreview.net/forum?id=LjtgTpWH71) | [📦](https://github.com/Yueeeeeeee/HRPO) | `method`, `hidden-state`, `autoregressive`, `compression`, `rl` | Mixes hidden states and tokens optimized with RL for implicit reasoning. |
| 2025 | Think Silently, Think Fast | NeurIPS 2025 | [📄](https://openreview.net/forum?id=AQsko3PPUe) | [📦](https://github.com/xiaomi-research/colar) | `method`, `hidden-state`, `autoregressive`, `compression` | Dynamic latent compression of reasoning chains. |
| 2025 | Text Generation Beyond Discrete Token Sampling | arXiv | [📄](https://arxiv.org/abs/2505.14827) | — | `method`, `soft-readout`, `parallel` | Generates text directly in continuous readout space. |
| 2025 | SofT-GRPO | arXiv | [📄](https://arxiv.org/abs/2511.06411) | [📦](https://github.com/zz1358m/SofT-GRPO-master) | `method`, `soft-readout`, `parallel`, `rl` | RL with Gumbel/soft-thinking for posterior-style latent optimization. |
| 2026 | GTS: Gaussian Thought Sampler | arXiv | [📄](https://arxiv.org/abs/2602.14077) | — | `method`, `soft-readout`, `parallel` | Explicitly models thought distributions with Gaussian sampling. |
| 2025 | Soft Thinking | NeurIPS 2025 | [📄](https://proceedings.neurips.cc/paper_files/paper/2025/file/f7396d1c54d51416958d63e285377103-Paper-Conference.pdf) | [📦](https://github.com/eric-ai-lab/Soft-Thinking) | `method`, `soft-readout`, `parallel` | Samples and searches in a continuous concept space instead of explicit CoT. |
| 2025 | Parallel Continuous Chain-of-Thought with Jacobi Iteration | EMNLP 2025 | [📄](https://aclanthology.org/2025.emnlp-main.47/) | [📦](https://github.com/whyNLP/PCCoT) | `method`, `soft-readout`, `parallel` | Jacobi-style parallel updates for continuous implicit CoT. |
| 2025 | Continuous Chain of Thought Enables Parallel Exploration and Reasoning (CoT2) | ICLR 2026 | [📄](https://openreview.net/forum?id=sTPKDKn5ig) | — | `method`, `soft-readout`, `parallel` | Continuous thoughts enable parallel implicit exploration. |
| 2025 | Learning More Effective Representations for Dense Retrieval through Deliberate Thinking before Search (Debater) | arXiv | [📄](https://arxiv.org/abs/2502.12974) | [📦](https://github.com/OpenBMB/DEBATER) | `method`, `hidden-state`, `autoregressive`, `routing` | Latent-space deliberation before search for efficient retrieval reasoning. |
| 2025 | SIM-CoT | ICLR 2026 | [📄](https://openreview.net/forum?id=6YRJ4jmVQl) | [📦](https://github.com/InternLM/SIM-CoT) | `method`, `hidden-state`, `autoregressive`, `compression` | Token-level supervised implicit chain-of-thought. |
| 2025 | Efficient Post-Training Refinement of Latent Reasoning in LLMs | arXiv | [📄](https://arxiv.org/abs/2506.08552) | — | `method`, `hidden-state`, `autoregressive`, `compression` | Post-training compression and refinement for latent reasoning models. |
| 2025 | DART | EMNLP 2025 | [📄](https://aclanthology.org/2025.emnlp-main.256/) | — | `method`, `hidden-state`, `autoregressive`, `compression`, `distillation` | Distills autoregressive reasoning into silent latent thoughts. |
| 2025 | CODI | EMNLP 2025 | [📄](https://aclanthology.org/2025.emnlp-main.36/) | [📦](https://github.com/zhenyi-shen/CODI) | `method`, `hidden-state`, `autoregressive`, `compression`, `distillation` | Self-distills CoT into a continuous latent space. |
| 2025 | LightThinker | EMNLP 2025 | [📄](https://aclanthology.org/2025.emnlp-main.673/) | [📦](https://github.com/zjunlp/LightThinker) | `method`, `hidden-state`, `autoregressive`, `compression` | Step-by-step compression of explicit CoT into latent states. |
| 2025 | Token Assorted | ICML 2025 | [📄](https://proceedings.mlr.press/v267/su25g.html) | — | `method`, `soft-readout`, `autoregressive`, `compression` | Mixes latent and text tokens as a hybrid soft-readout carrier. |
| 2025 | SoftCoT | ACL 2025 | [📄](https://aclanthology.org/2025.acl-long.1137/) | — | `method`, `soft-readout`, `autoregressive`, `compression` | Soft thought tokens replace long explicit CoT. |
| 2025 | LLM Pretraining with Continuous Concepts | arXiv | [📄](https://arxiv.org/abs/2502.08524) | [📦](https://github.com/facebookresearch/RAM/tree/main/projects/cocomix) | `method`, `soft-readout`, `autoregressive`, `concept-embedding` | Continuous concepts as soft semantic carriers for implicit reasoning. |
| 2025 | Latent Preference Coding | arXiv | [📄](https://arxiv.org/abs/2505.04993) | — | `method`, `soft-readout`, `autoregressive`, `concept-embedding` | Discrete latent codes model preference posteriors for efficient reasoning. |
| 2025 | Enhancing Non-Core Language Instruction-Following in Speech LLMs via Semi-Implicit Cross-Lingual CoT (XS-CoT) | arXiv | [📄](https://arxiv.org/abs/2504.20835) | — | `method`, `hidden-state`, `autoregressive`, `audio`, `compression` | Semi-implicit cross-lingual CoT with progressively compressible reasoning tokens. |
| 2024 | Training Large Language Models to Reason in a Continuous Latent Space (Coconut) | COLM 2025 | [📄](https://openreview.net/forum?id=Itxz7S4Ip3) | [📦](https://github.com/facebookresearch/coconut) | `method`, `hidden-state`, `autoregressive`, `compression` | Uses hidden states as continuous thoughts instead of explicit CoT. |
| 2024 | Compressed Chain of Thought | arXiv | [📄](https://arxiv.org/abs/2412.13171) | — | `method`, `hidden-state`, `autoregressive`, `compression` | Compresses explicit CoT into dense reasoning states. |
| 2024 | Hidden Chain-of-Thought Decoding | arXiv | [📄](https://arxiv.org/abs/2409.08561) | — | `method`, `hidden-state`, `autoregressive`, `compression` | Decodes with hidden CoT instead of explicit rationale tokens. |
| 2024 | Let's Think Dot by Dot: Hidden Computation in Transformer Language Models | COLM 2024 | [📄](https://arxiv.org/abs/2404.15758) | [📦](https://github.com/JacobPfau/fillerTokens) | `method`, `hidden-state`, `autoregressive`, `routing` | Filler tokens provide extra computation steps without explicit semantic CoT. |
| 2024 | From Explicit CoT to Implicit CoT: Learning to Internalize CoT Step by Step (ICoT-SI) | arXiv | [📄](https://arxiv.org/abs/2405.14838) | [📦](https://github.com/da03/Internalize_CoT_Step_by_Step) | `method`, `hidden-state`, `autoregressive`, `compression` | Curriculum removes explicit CoT tokens and internalizes steps into hidden states. |
| 2024 | Latent Space Chain-of-Embedding Enables Output-free LLM Self-Evaluation | ICLR 2025 | [📄](https://openreview.net/forum?id=jxo70B9fQo) | [📦](https://github.com/Alsace08/Chain-of-Embedding) | `method`, `soft-readout`, `autoregressive`, `concept-embedding` | Embedding-chain self-evaluation without generating explicit reasoning text. |
| 2024 | Large Concept Models | arXiv | [📄](https://arxiv.org/abs/2412.08821) | — | `method`, `soft-readout`, `autoregressive`, `embodied`, `concept-embedding` | Sentence/concept embeddings as high-level soft semantic reasoning carriers. |
| 2024 | Multimodal Latent Language Modeling with Next-Token Diffusion | arXiv | [📄](https://arxiv.org/abs/2412.08635) | — | `method`, `soft-readout`, `autoregressive`, `embodied`, `concept-embedding` | Continuous latent vectors with diffusion readout for unified multimodal modeling. |
| 2023 | Implicit Chain of Thought Reasoning via Knowledge Distillation | arXiv | [📄](https://arxiv.org/abs/2311.01460) | [📦](https://github.com/da03/implicit_chain_of_thought/) | `method`, `hidden-state`, `autoregressive`, `compression`, `distillation` | Emulator distills explicit CoT hidden states into an implicit-reasoning student. |

[Back](#bookmarks)

## Overthinking Reduction

| Year | Title | Venue | Paper | Code/Data | Tags | Note |
| ---- | ----- | ----- | :---: | :-------: | ---- | ---- |
| 2026 | SwiReasoning: Switch-Thinking in Latent and Explicit for Pareto-Superior Reasoning LLMs | ICLR 2026 | [📄](https://openreview.net/forum?id=t33kMzEAg8) | [📦](https://github.com/sdc17/SwiReasoning) | `method`, `hidden-state`, `autoregressive`, `routing` | Training-free switching between explicit CoT and latent reasoning to curb overthinking. |

[Back](#bookmarks)

## Early Stopping & Adaptive Exit

Adaptive depth, pondering, and test-time latent compute with budget control.

| Year | Title | Venue | Paper | Code/Data | Tags | Note |
| ---- | ----- | ----- | :---: | :-------: | ---- | ---- |
| 2026 | LoopFormer: Elastic-Depth Looped Transformers for Latent Reasoning via Shortcut Modulation | ICLR 2026 | [📄](https://openreview.net/forum?id=RzYXb5YWBs) | — | `method`, `hidden-state`, `depth-recurrence` | Time/step-conditioned loops with budget-tunable elastic-depth latent reasoning. |
| 2026 | Depth-Recurrent Attention Mixtures (Dreamer) | arXiv | [📄](https://arxiv.org/abs/2601.21582) | — | `method`, `hidden-state`, `depth-recurrence` | Depth-recurrent attention mixtures scale latent reasoning under a fixed token budget. |
| 2026 | Parallel Test-Time Scaling for Latent Reasoning Models | ACL 2026 | [📄](https://arxiv.org/abs/2510.07745) | [📦](https://github.com/YRYangang/LatentTTS) | `method`, `hidden-state`, `parallel`, `test-time` | Parallel sampling and aggregation for latent reasoning at inference time. |
| 2025 | SpiralThinker: Latent Reasoning through Text–Latent Interleaving | ACL 2026 Findings | [📄](https://openreview.net/forum?id=ZbYQ91Zw0t) | — | `method`, `hidden-state`, `depth-recurrence` | Iteratively refines latent states interleaved with text reasoning. |
| 2025 | PonderLM-2: Pretraining LLM with Latent Thoughts in Continuous Space | arXiv | [📄](https://arxiv.org/abs/2509.23184) | — | `method`, `hidden-state`, `depth-recurrence` | Emits continuous latent thoughts before each output token during pretraining. |
| 2025 | Think-at-Hard: Selective Latent Iterations to Improve Reasoning LLMs | arXiv | [📄](https://arxiv.org/abs/2511.08577) | [📦](https://github.com/thu-nics/TaH) | `method`, `hidden-state`, `depth-recurrence` | Triggers extra latent iterations only on hard tokens for efficient test-time depth. |
| 2025 | Learning to Ponder: Adaptive Reasoning in Latent Space (FR-Ponder) | arXiv | [📄](https://arxiv.org/abs/2509.24238) | — | `method`, `hidden-state`, `depth-recurrence` | Lightweight controller adapts test-time latent depth per instance without backbone changes. |
| 2025 | Latent Thinking Optimization (LTO) | arXiv | [📄](https://arxiv.org/abs/2509.26314) | — | `method`, `hidden-state`, `parallel`, `test-time` | Optimizes latent thinking trajectories at test time using a latent-space classifier. |
| 2025 | LatentEvolve | arXiv | [📄](https://arxiv.org/abs/2509.24771) | [📦](https://github.com/jins7/LatentEvolve) | `method`, `hidden-state`, `parallel`, `test-time` | Test-time latent self-evolution for reasoning refinement. |
| 2025 | Thinking on the Fly | ICLR 2026 | [📄](https://openreview.net/forum?id=r1WEQzkCQv) | [📦](https://github.com/ltpo2025/LTPO) | `method`, `hidden-state`, `parallel`, `test-time` | Policy optimization over latent thoughts at inference time. |
| 2025 | System-1.5 Reasoning: Traversal in Language and Latent Spaces with Dynamic Shortcuts | arXiv | [📄](https://arxiv.org/abs/2505.18962) | — | `method`, `hidden-state`, `depth-recurrence` | Dynamic shortcuts reuse hidden states across steps to allocate compute efficiently. |
| 2025 | Skip a Layer or Loop It? Test-Time Depth Adaptation of Pretrained LLMs | arXiv | [📄](https://arxiv.org/abs/2507.07996) | — | `method`, `hidden-state`, `depth-recurrence` | Test-time layer looping/skipping adapts effective depth under a compute budget. |
| 2025 | The 4th Dimension for Scaling Model Size | arXiv | [📄](https://arxiv.org/abs/2506.18233) | — | `method`, `hidden-state`, `depth-recurrence` | Recurrent depth as a fourth scaling dimension for latent reasoning. |
| 2025 | Mixture-of-Recursions | arXiv | [📄](https://arxiv.org/abs/2507.10524) | — | `method`, `hidden-state`, `depth-recurrence` | Token-level dynamic recursive depth for adaptive internal thinking. |
| 2025 | Hierarchical Reasoning Model | arXiv | [📄](https://arxiv.org/abs/2506.21734) | [📦](https://github.com/sapientinc/HRM) | `method`, `hidden-state`, `depth-recurrence` | Hierarchical recursive subproblem solving in latent space. |
| 2025 | Scaling Latent Reasoning via Looped Language Models | arXiv | [📄](https://arxiv.org/abs/2510.25741) | — | `method`, `hidden-state`, `depth-recurrence` | Looped language models scale latent reasoning through depth recurrence. |
| 2025 | Pretraining Language Models to Ponder in Continuous Space | ICLR 2026 | [📄](https://openreview.net/forum?id=UrM4MNRYZm) | — | `method`, `hidden-state`, `depth-recurrence` | Pondering in continuous space via iterative depth refinement. |
| 2025 | Reasoning with Latent Thoughts: On the Power of Looped Transformers | ICLR 2025 | [📄](https://openreview.net/forum?id=din0lGfZFd) | — | `method`, `hidden-state`, `depth-recurrence` | Looped transformers deepen thinking through layer recurrence. |
| 2025 | Inner Thinking Transformer | arXiv | [📄](https://arxiv.org/abs/2502.13842) | — | `method`, `hidden-state`, `depth-recurrence` | Dynamically expands internal thinking depth per token. |
| 2025 | Loop-Aligned Reasoning (RELAY) | arXiv | [📄](https://arxiv.org/abs/2502.08482) | [📦](https://github.com/qifanyu/RELAY) | `method`, `hidden-state`, `depth-recurrence` | Aligns autoregressive CoT supervision to looped internal reasoning. |
| 2025 | Scaling up Test-Time Compute with Latent Reasoning: A Recurrent Depth Approach | NeurIPS 2025 | [📄](https://proceedings.neurips.cc/paper_files/paper/2025/file/3b01972cf31e6fa0fe29e4b8b5c2a0a1-Paper-Conference.pdf) | [📦](https://github.com/seal-rg/recurrent-pretraining) | `method`, `hidden-state`, `depth-recurrence` | Recurrent depth allocates extra test-time compute in latent space. |
| 2025 | SoftCoT++ | arXiv | [📄](https://arxiv.org/abs/2505.11484) | — | `method`, `soft-readout`, `parallel`, `compression` | Parallel soft-trajectory refinement for test-time latent scaling. |
| 2025 | Seek in the Dark | arXiv | [📄](https://arxiv.org/abs/2505.13308) | [📦](https://github.com/bigai-nlco/LatentSeek) | `method`, `hidden-state`, `parallel`, `test-time` | Instance-level policy gradients search latent space at inference time. |
| 2024 | Language Models are Hidden Reasoners (LaTRO) | arXiv | [📄](https://arxiv.org/abs/2411.04282) | — | `method`, `hidden-state`, `parallel`, `test-time` | Treats reasoning as latent posterior optimization at test time. |
| 2024 | Think before you speak: Training Language Models With Pause Tokens | ICLR 2024 | [📄](https://openreview.net/forum?id=ph04CRkPdC) | — | `method`, `hidden-state`, `depth-recurrence` | Pause tokens delay readout to buy extra hidden-layer computation. |
| 2024 | Thinking Tokens for Language Modeling | arXiv | [📄](https://arxiv.org/abs/2405.08644) | — | `method`, `hidden-state`, `depth-recurrence` | Inserts thinking tokens to obtain more latent update steps in RNN LMs. |
| 2023 | CoTFormer | ICLR 2025 | [📄](https://openreview.net/forum?id=8wAL9SmUk8) | — | `method`, `hidden-state`, `depth-recurrence` | Budget-adaptive internal thinking via depth refinement. |

[Back](#bookmarks)

## Token / KV / Memory Optimization

| Year | Title | Venue | Paper | Code/Data | Tags | Note |
| ---- | ----- | ----- | :---: | :-------: | ---- | ---- |
| 2026 | The Silent Thought | ICML 2026 | [📄](https://arxiv.org/abs/2603.17837) | — | `method`, `hidden-state`, `memory-kv`, `audio` | Recurrent latent thinking while listening in audio-language models. |
| 2026 | Latent-DARM: Bridging Discrete Diffusion and Autoregressive Models for Reasoning | ICLR 2026 Workshop | [📄](https://openreview.net/forum?id=5y0tSg0dTf) | — | `method`, `hidden-state`, `memory-kv` | Latent interface connects a diffusion planner to an autoregressive executor. |
| 2025 | Identity Bridge: Enabling Implicit Reasoning via Shared Latent Memory | arXiv | [📄](https://arxiv.org/abs/2509.24653) | — | `method`, `hidden-state`, `memory-kv` | Shared latent memory supports efficient implicit multi-step reasoning. |
| 2025 | Latent Collaboration in Multi-Agent Systems | ICML 2026 | [📄](https://icml.cc/virtual/2026/poster/61180) | [📦](https://github.com/Gen-Verse/LatentMAS) | `method`, `hidden-state`, `memory-kv`, `embodied` | Agents share latent working memory for efficient collaboration. |
| 2025 | MeSH: Memory-as-State-Highways | ICLR 2026 | [📄](https://openreview.net/forum?id=IhTrFvY7p3) | — | `method`, `hidden-state`, `memory-kv` | Persistent memory highways carry evolving intermediate reasoning state. |
| 2025 | KaVa | ICLR 2026 | [📄](https://openreview.net/forum?id=ePrhcLbtGv) | — | `method`, `hidden-state`, `memory-kv` | Compressed KV trajectories supervise latent reasoning. |
| 2025 | Towards General Continuous Memory for Vision-Language Models (CoMEM) | arXiv | [📄](https://arxiv.org/abs/2505.17670) | — | `method`, `hidden-state`, `memory-kv`, `vlm` | Compresses multimodal knowledge into few continuous embeddings for efficient VLM reasoning. |
| 2024 | Deliberation in Latent Space via Differentiable Cache Augmentation | arXiv | [📄](https://arxiv.org/abs/2412.17747) | — | `method`, `hidden-state`, `memory-kv` | Injects latent computation directly into KV/cache. |
| 2022 | Memorizing Transformers | NeurIPS 2022 | [📄](https://arxiv.org/abs/2203.08913) | — | `method`, `hidden-state`, `memory-kv` | External kNN memory stores persistent intermediate states. |
| 2021 | Going Beyond Linear Transformers with Recurrent Fast Weight Programmers | NeurIPS 2021 | [📄](https://openreview.net/forum?id=ot2ORiBqTa1) | — | `method`, `hidden-state`, `memory-kv` | Recurrence plus fast weights for efficient state evolution. |
| 2021 | Linear Transformers Are Secretly Fast Weight Programmers | arXiv | [📄](https://arxiv.org/abs/2102.11174) | — | `method`, `hidden-state`, `memory-kv` | Interprets linear attention as fast-weight latent state programming. |
| 2020 | Compressive Transformers | arXiv | [📄](https://arxiv.org/abs/1911.05507) | — | `method`, `hidden-state`, `memory-kv` | Compresses past states into memory for long-horizon latent context. |
| 2019 | Transformer-XL | ACL 2019 | [📄](https://aclanthology.org/P19-1285/) | [📦](https://github.com/kimiyoung/transformer-xl) | `method`, `hidden-state`, `memory-kv` | Segment recurrence enables persistent latent state across long contexts. |
| 2016 | Using Fast Weights to Attend to the Recent Past | NeurIPS 2016 | [📄](https://papers.nips.cc/paper/6573-using-fast-weights-to-attend-to-the-recent-past) | — | `method`, `hidden-state`, `memory-kv` | Fast weights as classic dynamic latent memory for efficient recurrence. |
| 2023 | Adapting Language Models to Compress Contexts (AutoCompressor) | EMNLP 2023 | [📄](https://aclanthology.org/2023.emnlp-main.232/) | — | `method`, `hidden-state`, `memory-kv` | Compresses long context into summary vectors used as latent reasoning memory. |

[Back](#bookmarks)

## Distillation & Small Reasoning Models

| Year | Title | Venue | Paper | Code/Data | Tags | Note |
| ---- | ----- | ----- | :---: | :-------: | ---- | ---- |
| 2024 | Quiet-STaR: Language Models Can Teach Themselves to Think Before Speaking | COLM 2024 | [📄](https://arxiv.org/abs/2403.09629) | [📦](https://github.com/ezelikman/quiet-star) | `method`, `hidden-state`, `parallel`, `test-time` | Self-generates internal rationales and reinforces helpful latent thoughts without explicit CoT at inference. |

[Back](#bookmarks)

## Efficient Multimodal Reasoning

Implicit or latent reasoning across vision, video, audio, and embodied settings.

| Year | Title | Venue | Paper | Code/Data | Tags | Note |
| ---- | ----- | ----- | :---: | :-------: | ---- | ---- |
| 2026 | OneLatent | arXiv | [📄](https://arxiv.org/abs/2602.13738) | — | `method`, `modality-latent`, `autoregressive`, `vlm`, `visual-latent` | Single-token visual latent compression for efficient multimodal reasoning. |
| 2026 | Render-of-Thought | ACL 2026 | [📄](https://openreview.net/forum?id=8uPWvXS9sG) | [📦](https://github.com/TencentBAC/RoT) | `method`, `modality-latent`, `autoregressive`, `vlm`, `visual-latent` | Renders text CoT into images to enter visual latent reasoning space. |
| 2026 | ImgCoT | arXiv | [📄](https://arxiv.org/abs/2601.22730) | — | `method`, `modality-latent`, `autoregressive`, `vlm`, `visual-latent` | Compresses long CoT into compact visual tokens. |
| 2026 | ReGuLaR | arXiv | [📄](https://arxiv.org/abs/2601.23184) | [📦](https://github.com/FanmengWang/ReGuLaR) | `method`, `modality-latent`, `parallel`, `vlm`, `embodied-latent` | Variational latent reasoning with rendered-CoT supervision. |
| 2026 | Thinking with Images as Continuous Actions | arXiv | [📄](https://arxiv.org/abs/2602.23959) | — | `method`, `modality-latent`, `autoregressive`, `vlm`, `embodied-latent` | Continuous coordinate actions serve as visual intermediate reasoning states. |
| 2026 | Latent Reasoning VLA (LaRA-VLA) | ICML 2026 | [📄](https://arxiv.org/abs/2602.01166) | — | `method`, `modality-latent`, `autoregressive`, `embodied`, `embodied-latent` | Curriculum from explicit multimodal CoT to continuous latent reasoning for VLA. |
| 2026 | LaST₀: Latent Spatio-Temporal Chain-of-Thought for Robotic VLA | arXiv | [📄](https://arxiv.org/abs/2601.05248) | — | `method`, `modality-latent`, `autoregressive`, `embodied`, `embodied-latent` | Latent spatio-temporal CoT trajectories for efficient robotic planning. |
| 2026 | CLAP | arXiv | [📄](https://arxiv.org/abs/2601.04061) | — | `method`, `modality-latent`, `autoregressive`, `embodied`, `embodied-latent` | Contrastive latent actions align video and robot actions for efficient embodied reasoning. |
| 2025 | Sketch-in-Latents: Eliciting Unified Reasoning in MLLMs (SkiLa) | arXiv | [📄](https://arxiv.org/abs/2512.16584) | — | `method`, `modality-latent`, `autoregressive`, `vlm`, `visual-latent` | Alternates text thoughts and latent sketch tokens with semantic reconstruction. |
| 2025 | Latent Chain-of-Thought World Modeling for Autonomous Driving (LCDrive) | CVPR 2026 | [📄](https://arxiv.org/abs/2512.10226) | — | `method`, `modality-latent`, `autoregressive`, `embodied`, `embodied-latent` | Interleaves action proposals and latent world-model tokens for efficient driving rollout. |
| 2025 | Think with 3D: Geometric Imagination Grounded Spatial Reasoning (3DThinker) | CVPR 2026 | [📄](https://arxiv.org/abs/2510.18632) | — | `method`, `modality-latent`, `depth-recurrence`, `vlm`, `spatiotemporal-latent` | Online 3D geometric latent imagination for spatial reasoning from limited views. |
| 2025 | VL-JEPA | arXiv | [📄](https://arxiv.org/abs/2512.10942) | — | `method`, `modality-latent`, `autoregressive`, `vlm`, `visual-latent` | Predicts continuous text embeddings instead of discrete tokens for efficient VL reasoning. |
| 2025 | Monet | CVPR 2026 | [📄](https://arxiv.org/abs/2511.21395) | [📦](https://github.com/NOVAglow646/Monet) | `method`, `modality-latent`, `autoregressive`, `vlm`, `visual-latent` | Reasons directly in latent visual space with VLPO. |
| 2025 | Chain-of-Visual-Thought (CoVT) | arXiv | [📄](https://arxiv.org/abs/2511.19418) | [📦](https://github.com/ymqian151/Chain-of-Visual-Thought) | `method`, `modality-latent`, `autoregressive`, `vlm`, `visual-latent` | Continuous visual tokens carry intermediate multimodal reasoning. |
| 2025 | CoCoVa | arXiv | [📄](https://arxiv.org/abs/2511.02360) | — | `method`, `modality-latent`, `depth-recurrence`, `vlm`, `spatiotemporal-latent` | Latent Q-Former iteratively fuses vision and text for efficient spatio-temporal reasoning. |
| 2025 | Latent Sketchpad | arXiv | [📄](https://arxiv.org/abs/2510.24514) | [📦](https://github.com/Huanyu-Zhang/LatentSketchpad) | `method`, `modality-latent`, `autoregressive`, `vlm`, `visual-latent` | Internal visual sketches act as a latent workspace for reasoning. |
| 2025 | Latent Chain-of-Thought for Visual Reasoning (LaCoT) | NeurIPS 2025 | [📄](https://openreview.net/forum?id=0i8ClSr3kQ) | [📦](https://github.com/heliossun/LaCoT) | `method`, `modality-latent`, `parallel`, `vlm`, `embodied-latent` | Posterior inference learns visual latent rationales without long explicit CoT. |
| 2025 | Reasoning in the Dark | arXiv | [📄](https://arxiv.org/abs/2510.12603) | [📦](https://github.com/FYYDCC/IVT-LR) | `method`, `modality-latent`, `autoregressive`, `vlm`, `visual-latent` | Each step carries coupled latent text and latent vision for efficient multimodal thinking. |
| 2025 | Latent Visual Reasoning (LVR) | arXiv | [📄](https://arxiv.org/abs/2509.24251) | [📦](https://github.com/bangzhengli/LVR) | `method`, `modality-latent`, `autoregressive`, `vlm`, `visual-latent` | Generates reconstructible visual tokens as latent reasoning workspace. |
| 2025 | Multimodal Chain of Continuous Thought (MCoCOT) | arXiv | [📄](https://arxiv.org/abs/2508.12587) | — | `method`, `modality-latent`, `autoregressive`, `vlm`, `visual-latent` | Continuous vision-language thought chain in latent space. |
| 2025 | villa-X | arXiv | [📄](https://arxiv.org/abs/2507.23682) | — | `method`, `modality-latent`, `autoregressive`, `embodied`, `embodied-latent` | Unifies vision-language-latent-action planning for efficient embodied reasoning. |
| 2025 | V-JEPA 2 | arXiv | [📄](https://arxiv.org/abs/2506.09985) | [📦](https://github.com/facebookresearch/jepa) | `method`, `modality-latent`, `depth-recurrence`, `video`, `spatiotemporal-latent` | Video world model with latent predictive representations for planning-efficient reasoning. |
| 2025 | Machine Mental Imagery | arXiv | [📄](https://arxiv.org/abs/2506.17218) | [📦](https://github.com/UMass-Embodied-AGI/Mirage) | `method`, `modality-latent`, `autoregressive`, `vlm`, `visual-latent` | Latent visual tokens serve as internal mental imagery for reasoning. |
| 2025 | SSR: Rationale-Guided Spatial Reasoning | NeurIPS 2025 | [📄](https://openreview.net/forum?id=SOc0tHCewe) | [📦](https://yliu-cs.github.io/SSR/) | `method`, `modality-latent`, `autoregressive`, `vlm`, `visual-latent` | Distills spatial rationales into compact latent embeddings for efficient VLM reasoning. |
| 2025 | Efficient Reasoning with Hidden Thinking (Heima) | ICML 2026 | [📄](https://arxiv.org/abs/2501.19201) | [📦](https://github.com/shawnricecake/Heima) | `method`, `modality-latent`, `autoregressive`, `vlm`, `visual-latent` | Compresses CoT into thinking tokens with encode-decode reconstruction in MLLMs. |
| 2025 | Latent Action Pretraining Through World Modeling | arXiv | [📄](https://arxiv.org/abs/2509.18428) | — | `method`, `modality-latent`, `memory-kv`, `embodied`, `embodied-latent` | World-model constraints learn efficient latent action representations. |
| 2024 | Latent Action Pretraining from Videos | ICLR 2025 | [📄](https://openreview.net/forum?id=VYOe2eBQeh) | [📦](https://github.com/LatentActionPretraining/LAPA) | `method`, `modality-latent`, `memory-kv`, `embodied`, `embodied-latent` | Latent action tokens as compact intermediate states for embodied reasoning. |
| 2024 | Video Representation Learning with Joint-Embedding Predictive Architectures | arXiv | [📄](https://arxiv.org/abs/2412.10925) | — | `method`, `modality-latent`, `depth-recurrence`, `video`, `spatiotemporal-latent` | JEPA latent targets encode video dynamics for efficient predictive reasoning. |
| 2019 | Dream to Control | ICLR 2020 | [📄](https://openreview.net/forum?id=S1lOTC4tDS) | [📦](https://github.com/google-research/dreamer) | `method`, `modality-latent`, `parallel`, `embodied`, `embodied-latent` | Optimizes policies inside latent imagination for sample-efficient control reasoning. |
| 2018 | Learning Latent Dynamics for Planning from Pixels (PlaNet) | ICML 2019 | [📄](https://arxiv.org/abs/1811.04551) | — | `method`, `modality-latent`, `parallel`, `embodied`, `embodied-latent` | Plans in learned latent dynamics for efficient visual reasoning and control. |

[Back](#bookmarks)

## Efficiency Benchmarks

Analysis and theory of whether implicit/latent reasoning is faithful, efficient, and reliable.

| Year | Title | Venue | Paper | Code/Data | Tags | Note |
| ---- | ----- | ----- | :---: | :-------: | ---- | ---- |
| 2026 | Large Reasoning Models Are (Not Yet) Multilingual Latent Reasoners | ACL 2026 Findings | [📄](https://arxiv.org/abs/2601.02996) | [📦](https://github.com/cisnlp/multilingual-latent-reasoner) | `analysis`, `hidden-state`, `autoregressive`, `behavioral` | Diagnoses uneven multilingual behavior in latent reasoning pathways. |
| 2026 | Dynamics Within Latent Chain-of-Thought: An Empirical Study of Causal Structure | ICML 2026 | [📄](https://proceedings.mlr.press/v306/li26a.html) | [📦](https://github.com/J1mL1/causal-latent-cot) | `analysis`, `hidden-state`, `depth-recurrence`, `causal` | Step-wise causal interventions on Coconut and CODI reveal cross-step latent structure. |
| 2026 | Do Latent-CoT Models Think Step-by-Step? | arXiv | [📄](https://arxiv.org/abs/2602.00449) | [📦](https://github.com/jialiang19/latent-cot-thinking) | `analysis`, `hidden-state`, `autoregressive`, `probing` | Probes whether CODI truly encodes and uses sequential intermediate states. |
| 2026 | Capabilities and Fundamental Limits of Latent Chain-of-Thought | arXiv | [📄](https://arxiv.org/abs/2602.01148) | — | `theory`, `soft-readout`, `parallel` | Formal limits of latent CoT on exploratory versus computational tasks. |
| 2026 | The Theoretical Benefits and Limitations of Latent Chain-of-Thought Reasoning | ICLR 2026 | [📄](https://openreview.net/forum?id=q7Nhu2Fw11) | — | `theory`, `soft-readout`, `parallel` | Theory unifying exploration benefits and fidelity limits of latent CoT. |
| 2026 | How Do Latent Reasoning Methods Perform Under Weak and Strong Supervision | arXiv | [📄](https://arxiv.org/abs/2602.22441) | — | `analysis`, `hidden-state`, `autoregressive`, `behavioral` | Behavioral diagnosis of shortcut trade-offs in Coconut/CODI-style methods. |
| 2026 | Emergence of Superposition in Chain of Continuous Thought | ICLR 2026 | [📄](https://openreview.net/forum?id=lsJwX9Jf5u) | — | `theory`, `soft-readout`, `parallel` | Training dynamics explain superposition in continuous implicit CoT. |
| 2026 | LLMs Are Single-Threaded Reasoners: Soft Thinking Mechanism | ICLR 2026 | [📄](https://openreview.net/forum?id=ASLuOoP78o) | — | `analysis`, `soft-readout`, `autoregressive`, `behavioral` | Shows soft thinking behaves as greedy single-threaded reasoning despite parallel design. |
| 2025 | Do Latent Tokens Think? A Causal and Adversarial Analysis of Chain-of-Continuous-Thought | arXiv | [📄](https://arxiv.org/abs/2512.21711) | — | `analysis`, `hidden-state`, `parallel`, `causal` | Causal/adversarial study finds latent tokens can act as placeholders with shortcut risk. |
| 2025 | A Formal Comparison Between Chain of Thought and Latent Thought | ICML 2026 | [📄](https://arxiv.org/abs/2509.25239) | [📦](https://github.com/kevin671/cot-vs-loop) | `theory`, `hidden-state`, `parallel` | Formalizes compute and parallelism differences between explicit and latent thought. |
| 2025 | Reasoning by Superposition: A Theoretical Perspective on Chain of Continuous Thought | NeurIPS 2025 | [📄](https://proceedings.neurips.cc/paper_files/paper/2025/file/72c363c2a573ca2128bd176d3317696b-Paper-Conference.pdf) | — | `theory`, `soft-readout`, `parallel` | Theoretical account of parallel exploration via superposition in continuous CoT. |
| 2025 | Do Language Models Use Their Depth Efficiently? | ICML 2025 | [📄](https://proceedings.mlr.press/v267/csordas25a.html) | — | `analysis`, `hidden-state`, `depth-recurrence`, `behavioral` | Diagnoses inefficient depth usage relevant to latent depth-based reasoning. |
| 2025 | Uncovering Latent Chain of Thought Vectors in Large Language Models | ICLR 2025 Workshop | [📄](https://iclr.cc/virtual/2025/33087) | — | `analysis`, `hidden-state`, `autoregressive`, `probing` | Decodes latent CoT vectors to test what implicit states encode. |
| 2025 | Think-to-Talk or Talk-to-Think? Multi-Step Arithmetic Timing | arXiv | [📄](https://arxiv.org/abs/2412.01113) | — | `analysis`, `hidden-state`, `autoregressive`, `probing` | Probes when implicit arithmetic reasoning happens relative to answer generation. |
| 2025 | A Little Depth Goes a Long Way: Expressive Power of Log-Depth Transformers | ICLR 2025 | [📄](https://openreview.net/forum?id=7cMzTpbJHC) | — | `theory`, `hidden-state`, `depth-recurrence` | Argues vertical depth bottlenecks explicit CoT steps and motivates latent depth methods. |
| 2025 | Implicit Reasoning in Transformers Is Reasoning through Shortcuts | ICLR 2025 | [📄](https://openreview.net/forum?id=7RJT6w3kKc) | — | `analysis`, `hidden-state`, `depth-recurrence`, `behavioral` | Shows implicit reasoning can rely on shortcuts rather than faithful intermediate computation. |
| 2024 | Do LLMs Really Think Step-by-step In Implicit Reasoning? | arXiv | [📄](https://arxiv.org/abs/2411.15862) | [📦](https://github.com/yuyijiong/if_step_by_step_implicit_CoT) | `analysis`, `hidden-state`, `depth-recurrence`, `probing` | Linear probes reveal trained implicit CoT encodes steps; prompted implicit CoT does not. |
| 2024 | Can Language Models Learn to Skip Steps? | ICLR 2024 | [📄](https://openreview.net/forum?id=w4AnTVxAO9) | — | `analysis`, `hidden-state`, `autoregressive`, `probing` | Probes whether models internalize or skip intermediate reasoning steps. |
| 2024 | Do Large Language Models Latently Perform Multi-Hop Reasoning? | ACL 2024 | [📄](https://doi.org/10.18653/v1/2024.acl-long.550) | — | `analysis`, `hidden-state`, `depth-recurrence`, `probing` | Probing evidence for multi-hop reasoning in latent states. |

[Back](#bookmarks)
