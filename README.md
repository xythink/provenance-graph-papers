<div align="center">
  <h1>📊 Awesome Provenance Graph Papers</h1>
  <p>
    <b>A curated collection of provenance graph & APT detection papers</b>
  </p>
  <p>
    <img src="https://img.shields.io/badge/papers-32-blue" alt="papers">
    <img src="https://img.shields.io/badge/last%20update-2026--03--30-green" alt="update">
    <img src="https://img.shields.io/badge/maintained%20by-OpenClaw-orange" alt="openclaw">
    <img src="https://img.shields.io/github/stars/xythink/provenance-graph-papers?style=social" alt="stars">
  </p>
  <p>
    🤖 本仓库由 <a href="https://github.com/openclaw/openclaw">OpenClaw</a> AI 助手自动维护<br>
    📬 欢迎 PR 补充论文 · ⭐ Star 支持一下
  </p>
</div>

---

## 📋 Table of Contents

- [📈 Research Trends](#-research-trends)
- [📊 Method Comparison](COMPARISON.md)
- [📖 Paper Reading Notes](reading/)
- [Survey](#survey)
- [APT Detection](#apt-detection)
  - [Graph Neural Networks](#graph-neural-networks)
  - [LLM-based Methods](#llm-based-methods)
  - [Reinforcement Learning](#reinforcement-learning)
  - [Transformer-based](#transformer-based)
  - [Few-Shot Learning](#few-shot-learning)
  - [Rule-based / Adaptive](#rule-based--adaptive)
- [Attack Path & Tactic Recognition](#attack-path--tactic-recognition)
- [Graph Construction & Representation](#graph-construction--representation)
- [Lifelong Learning & Concept Drift](#lifelong-learning--concept-drift)
- [Datasets & Benchmarks](#datasets--benchmarks)
- [Open Source Code](#open-source-code)

---

## 📈 Research Trends

```
2023  ████░░░░░░░░░░░░  4 papers   基础 GNN (MAGIC, NODLINK, Prov2vec, LogShield)
2024  ██████░░░░░░░░░░  8 papers   多样化 (RL, Few-shot, 隐私保护, 顶会 KAIROS@S&P)
2025  ████████████████ 17 papers   LLM 爆发 + 顶会丰收 (Slot@CCS, OCR-APT@CCS, CAPTAIN@NDSS)
2026  ██████░░░░░░░░░░  3 papers   图-语言预训练 (APT-CGLP@KDD) + LLM 语义 (Semantic-Aware)
```

**Key observations:**
- 🔥 **2025 是 LLM+溯源图元年** — OMNISEC, ProvSEEK, SHIELD, OCR-APT, APT-LLM 五篇 LLM 方法同年出现
- 📊 **DARPA TC 仍是主流 benchmark** — 28/32 篇论文使用
- 🏆 **顶会认可度持续上升** — KAIROS (S&P'24), MAGIC (USENIX Sec'24), CAPTAIN (NDSS'25), Slot & OCR-APT (CCS'25), ORTHRUS (USENIX Sec'25), APT-CGLP (KDD'26)
- 📝 **首个全面 SoK + 统一框架** — Bilot et al. SoK (USENIX Sec'25) + PIDSMaker 开源框架

---

## Survey

| Paper | Venue | PDF | Highlights |
|-------|-------|-----|------------|
| **Sometimes Simpler is Better: A Comprehensive Analysis of State-of-the-Art PIDS** | USENIX Sec'25 | [pdf](Bilot_SoK_2025.pdf) | 首个全面 PIDS SoK，系统对比所有主流方法 |

---

## APT Detection

### Graph Neural Networks

| # | Paper | Venue | Links | Key Technique |
|---|-------|-------|-------|---------------|
| 1 | **KAIROS**: Practical Intrusion Detection and Investigation using Whole-system Provenance | S&P'24 | [arxiv](https://arxiv.org/abs/2308.05034) · [pdf](KAIROS_2024.pdf) | 时序因果 GNN encoder-decoder |
| 2 | **MAGIC**: Detecting APTs via Masked Graph Representation Learning | USENIX Sec'24 | [arxiv](https://arxiv.org/abs/2310.09831) · [pdf](MAGIC_2023.pdf) · [code](https://github.com/FDUDSDE/MAGIC) | 掩码图自编码器，自监督 |
| 3 | **ORTHRUS**: Achieving High Quality of Attribution in Provenance-based IDS | USENIX Sec'25 | [paper](https://www.usenix.org/conference/usenixsecurity25/presentation/jiang-baoxiang) · [pdf](ORTHRUS_2025.pdf) · [code](https://github.com/ubc-provenance/orthrus) | 节点级高质量归因 |
| 4 | **APT-MCL**: Adaptive APT Detection via Multi-View Collaborative Provenance Graph Learning | arXiv'26 | [arxiv](https://arxiv.org/abs/2601.08328) · [pdf](APT-MCL_2026.pdf) | 多视图协同学习 |
| 5 | **APT-CGLP**: APT Hunting via Contrastive Graph-Language Pre-Training | KDD'26 | [arxiv](https://arxiv.org/abs/2511.20290) · [pdf](APT-CGLP_2025.pdf) | 对比图-语言预训练 |
| 6 | **NODLINK**: An Online System for Fine-Grained APT Attack Detection | NDSS'24 | [arxiv](https://arxiv.org/abs/2311.02331) · [pdf](NODLINK_2023.pdf) | 在线细粒度检测 |
| 7 | **FLASH**: A Comprehensive Approach to Intrusion Detection via Provenance Graph Representation Learning | arXiv'24 | [paper](https://ieeexplore.ieee.org/document/10646725/) · [pdf](FLASH_2024.pdf) | 综合图表示学习 |
| 8 | **TFLAG**: Towards Practical APT Detection via Deviation-Aware Learning on Temporal Provenance Graph | arXiv'25 | [arxiv](https://arxiv.org/abs/2501.06997) · [pdf](TFLAG_2025.pdf) | 时序偏差感知 |
| 9 | **Sentient**: Detecting APTs Via Capturing Indirect Dependencies and Behavioral Logic | arXiv'25 | [arxiv](https://arxiv.org/abs/2502.06521) · [pdf](Sentient_2025.pdf) | 间接依赖+行为逻辑 |
| 10 | **GraphDART**: Graph Distillation for Efficient APT Detection | arXiv'25 | [arxiv](https://arxiv.org/abs/2501.02796) · [pdf](GraphDART_2025.pdf) | 图蒸馏，效率优化 |
| 11 | **HADES**: Detecting Active Directory Attacks via Whole Network Provenance Analytics | arXiv'24 | [arxiv](https://arxiv.org/abs/2407.18858) · [pdf](HADES_2024.pdf) | AD 攻击全网分析 |
| 12 | **LTRDetector**: Exploring Long-Term Relationship for APT Detection | arXiv'24 | [arxiv](https://arxiv.org/abs/2404.03162) · [pdf](LTRDetector_2024.pdf) | 长期关系建模 |
| 13 | **P3GNN**: A Privacy-Preserving Provenance Graph-Based Model for APT Detection in SDN | arXiv'24 | [arxiv](https://arxiv.org/abs/2406.12003) · [pdf](P3GNN_2024.pdf) | 隐私保护联邦学习 |
| 14 | **Winemaking**: Extracting Essential Insights for Efficient Threat Detection in Audit Logs | arXiv'24 | [arxiv](https://arxiv.org/abs/2411.02775) · [pdf](Winemaking_2024.pdf) | 审计日志精华提取 |
| 15 | **CONTINUUM**: Detecting APT Attacks through Spatial-Temporal Graph Neural Networks | arXiv'25 | [arxiv](https://arxiv.org/abs/2501.02981) | 时空 GNN 自编码器 + 联邦学习 |

### LLM-based Methods

| # | Paper | Venue | Links | Key Technique |
|---|-------|-------|-------|---------------|
| 1 | **OMNISEC**: LLM-Driven Provenance-based IDS via Retrieval-Augmented Behavior Prompting | arXiv'25 | [arxiv](https://arxiv.org/abs/2503.03108) · [pdf](OMNISEC_2025.pdf) | LLM + RAG 异常判断 + 攻击图重建 |
| 2 | **ProvSEEK**: LLM-driven Provenance Forensics for Threat Investigation | arXiv'25 | [arxiv](https://arxiv.org/abs/2508.21323) · [pdf](ProvSEEK_2025.pdf) | LLM Agent 迭代 CoT 取证 |
| 3 | **SHIELD**: APT Detection and Intelligent Explanation Using LLM | arXiv'25 | [arxiv](https://arxiv.org/abs/2502.02342) · [pdf](SHIELD_2025.pdf) | GPT 检测 + 可解释性 |
| 4 | **OCR-APT**: Reconstructing APT Stories from Audit Logs using Subgraph Anomaly Detection and LLMs | CCS'25 | [arxiv](https://arxiv.org/abs/2510.15188) · [pdf](OCR-APT_2025.pdf) | 子图异常 + LLM 攻击故事重建 |
| 5 | **APT-LLM**: Embedding-Based Anomaly Detection of Cyber APTs Using Large Language Models | arXiv'25 | [arxiv](https://arxiv.org/abs/2502.09385) | LLM 嵌入 + 自编码器异常检测 |
| 6 | **Knowledge Transfer from LLMs to Provenance Analysis**: A Semantic-Augmented Method for APT Detection | arXiv'25 | [arxiv](https://arxiv.org/abs/2503.18316) | LLM 知识迁移到溯源图分析 |
| 7 | **Semantic-Aware APT Detection** Using Autoencoders on LLM-Encoded System Logs | arXiv'26 | [arxiv](https://arxiv.org/abs/2602.00204) | LLM 编码日志 + 自编码器 |

### Reinforcement Learning

| # | Paper | Venue | Links | Key Technique |
|---|-------|-------|-------|---------------|
| 1 | **Slot**: Provenance-Driven APT Detection through Graph Reinforcement Learning | CCS'25 | [arxiv](https://arxiv.org/abs/2410.17910) · [pdf](Slot_2024.pdf) | 图强化学习自适应检测 |

### Transformer-based

| # | Paper | Venue | Links | Key Technique |
|---|-------|-------|-------|---------------|
| 1 | **LogShield**: A Transformer-based APT Detection System Leveraging Self-Attention | arXiv'23 | [arxiv](https://arxiv.org/abs/2311.05733) · [pdf](LogShield_2023.pdf) | 自注意力序列建模 |

### Few-Shot Learning

| # | Paper | Venue | Links | Key Technique |
|---|-------|-------|-------|---------------|
| 1 | **TREC**: APT Tactic/Technique Recognition via Few-Shot Provenance Subgraph Learning | arXiv'24 | [arxiv](https://arxiv.org/abs/2402.15147) · [pdf](TREC_2024.pdf) | 少样本战术识别 |

### Rule-based / Adaptive

| # | Paper | Venue | Links | Key Technique |
|---|-------|-------|-------|---------------|
| 1 | **CAPTAIN**: Incorporating Gradients to Rules for Lightweight, Adaptive Provenance-based Intrusion Detection | NDSS'25 | [arxiv](https://arxiv.org/abs/2404.14720) · [code](https://github.com/LexusWang/CAPTAIN) | 梯度优化规则，自适应轻量 PIDS |

---

## Attack Path & Tactic Recognition

| # | Paper | Venue | Links | Key Technique |
|---|-------|-------|-------|---------------|
| 1 | **TPPR**: APT Tactic/Technique Pattern Guided Attack Path Reasoning | arXiv'25 | [arxiv](https://arxiv.org/abs/2510.22191) · [pdf](TPPR_2025.pdf) | ATT&CK 模式引导路径推理 |

---

## Graph Construction & Representation

| # | Paper | Venue | Links | Key Technique |
|---|-------|-------|-------|---------------|
| 1 | **Prov2vec**: Learning Provenance Graph Representation for Unsupervised APT Detection | arXiv'23 | [arxiv](https://arxiv.org/abs/2310.00843) · [pdf](Prov2vec_2023.pdf) | 无监督图嵌入 |
| 2 | **PROVSYN**: Synthesizing Provenance Graphs for Data Augmentation in IDS | arXiv'25 | [arxiv](https://arxiv.org/abs/2506.06226) · [pdf](PROVSYN_2025.pdf) | 溯源图合成增强 |

---

## Lifelong Learning & Concept Drift

| # | Paper | Venue | Links | Key Technique |
|---|-------|-------|-------|---------------|
| 1 | **METANOIA**: A Lifelong IDS for Mitigating Concept Drift | arXiv'25 | [arxiv](https://arxiv.org/abs/2501.00438) · [pdf](METANOIA_2025.pdf) | 终身学习适应环境变化 |

---

## Datasets & Benchmarks

| Dataset | Description | Source | Used by |
|---------|-------------|--------|---------|
| **DARPA TC** | Transparent Computing — 最主流的 APT 检测 benchmark (Trace/Theia/Cadets/FiveDirections) | [GitHub](https://github.com/darpa-i2o/Transparent-Computing) | 28/32 papers |
| **StreamSpot** | 流式异构信息流图 | [paper](https://dl.acm.org/doi/10.1145/2939672.2939716) | 3/32 papers |
| **Unicorn** | 企业级端点数据集 | [paper](https://dl.acm.org/doi/10.1145/3319535.3363214) | 2/32 papers |

### Frameworks & Tools

| Paper | Venue | Links | Description |
|-------|-------|-------|-------------|
| **PIDSMaker**: Building and Evaluating Provenance-based Intrusion Detection Systems | USENIX Sec'25 | [arxiv](https://arxiv.org/abs/2601.22983) · [code](https://github.com/ubc-provenance/PIDSMaker) | 开源 PIDS 统一评估框架，集成 8 个系统 |

---

## Open Source Code

| Paper | Code | Stars |
|-------|------|-------|
| MAGIC | [FDUDSDE/MAGIC](https://github.com/FDUDSDE/MAGIC) | ![](https://img.shields.io/github/stars/FDUDSDE/MAGIC?style=social) |
| ORTHRUS | [ubc-provenance/orthrus](https://github.com/ubc-provenance/orthrus) | ![](https://img.shields.io/github/stars/ubc-provenance/orthrus?style=social) |
| PIDSMaker | [ubc-provenance/PIDSMaker](https://github.com/ubc-provenance/PIDSMaker) | ![](https://img.shields.io/github/stars/ubc-provenance/PIDSMaker?style=social) |
| CAPTAIN | [LexusWang/CAPTAIN](https://github.com/LexusWang/CAPTAIN) | ![](https://img.shields.io/github/stars/LexusWang/CAPTAIN?style=social) |
| DARPA TC | [darpa-i2o/Transparent-Computing](https://github.com/darpa-i2o/Transparent-Computing) | ![](https://img.shields.io/github/stars/darpa-i2o/Transparent-Computing?style=social) |

> 📢 如果你知道其他论文的开源代码，欢迎 PR 补充！

---

## 🔧 Contributing

欢迎提交 PR 添加新论文！格式参考：

```markdown
| # | **Paper Title**: Description | Venue | [arxiv](url) · [pdf](file.pdf) | Key technique |
```

**提交规范：**
1. PDF 文件命名：`PaperName_Year.pdf`
2. 按年份倒序排列（新的在前）
3. 注明发表会议或 arXiv

---

## 📄 License

MIT

---

<p align="center">
  <b>If you find this repository useful, please consider giving it a ⭐</b><br>
  <sub>Maintained with ❤️ by <a href="https://github.com/openclaw/openclaw">OpenClaw</a></sub>
</p>
