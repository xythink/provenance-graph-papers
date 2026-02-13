<div align="center">
  <h1>Awesome Provenance Graph Papers</h1>
  <p>
    <b>终端溯源图与APT检测相关论文集合</b>
  </p>
  <p>
    <img src="https://img.shields.io/badge/papers-26-blue" alt="papers">
    <img src="https://img.shields.io/badge/last%20update-2026--02--13-green" alt="update">
    <img src="https://img.shields.io/badge/maintained%20by-Clawdbot-orange" alt="clawdbot">
  </p>
  <p>
    🤖 本仓库由 <a href="https://github.com/clawdbot/clawdbot">Clawdbot</a> 自动维护
  </p>
</div>

---

## 📋 Contents

- [**方法对比表 (NEW)**](COMPARISON.md)
- [**论文解读 (NEW)**](reading/)
- [Survey](#survey)
- [APT Detection](#apt-detection)
  - [Graph Neural Networks](#graph-neural-networks)
  - [LLM-based Methods](#llm-based-methods)
  - [Reinforcement Learning](#reinforcement-learning)
  - [Transformer-based](#transformer-based)
  - [Few-Shot Learning](#few-shot-learning)
- [Attack Path & Tactic Recognition](#attack-path--tactic-recognition)
- [Graph Construction & Representation](#graph-construction--representation)
- [Lifelong Learning & Concept Drift](#lifelong-learning--concept-drift)
- [Datasets](#datasets)

---

## Survey

1. **Sometimes Simpler is Better: A Comprehensive Analysis of State-of-the-Art Provenance-based Intrusion Detection Systems.** USENIX Security 2025. [paper](https://www.usenix.org/conference/usenixsecurity25/presentation/bilot) [pdf](Bilot_SoK_2025.pdf)

   *Tristan Bilot, Nour El Madhoun, Khaldoun Al Agha, Anis Zouaoui, Baoxiang Jiang, Shahrear Iqbal, Xueyuan Han, Thomas Pasquier.*

## APT Detection

### Graph Neural Networks

1. **APT-MCL: An Adaptive APT Detection System Based on Multi-View Collaborative Provenance Graph Learning.** arxiv 2026. [paper](https://arxiv.org/abs/2501.07567) [pdf](APT-MCL_2026.pdf)

   *Mingqi Lv, Shanshan Zhang, Haiwen Liu, Tieming Chen, Tiantian Zhu.*

2. **MAGIC: Detecting Advanced Persistent Threats via Masked Graph Representation Learning.** USENIX Security 2024. [paper](https://arxiv.org/abs/2310.09831) [pdf](MAGIC_2023.pdf)

   *Zian Jia, Yun Xiong, Yuhong Nan, Yao Zhang, Jinjing Zhao, Mi Wen.*

3. **NODLINK: An Online System for Fine-Grained APT Attack Detection and Investigation.** NDSS 2024. [paper](https://arxiv.org/abs/2311.02331) [pdf](NODLINK_2023.pdf)

   *Shaofei Li, Feng Dong, Xusheng Xiao, Haoyu Wang, Fei Shao, Jiedong Chen, Yao Guo, Xiangqun Chen, Ding Li.*

4. **TFLAG: Towards Practical APT Detection via Deviation-Aware Learning on Temporal Provenance Graph.** arxiv 2025. [paper](https://arxiv.org/abs/2501.06997) [pdf](TFLAG_2025.pdf)

   *Wenhan Jiang, Tingting Chai, Hongri Liu, Kai Wang, Hongke Zhang.*

5. **P3GNN: A Privacy-Preserving Provenance Graph-Based Model for APT Detection in SDN.** arxiv 2024. [paper](https://arxiv.org/abs/2406.12003) [pdf](P3GNN_2024.pdf)

   *Hedyeh Nazari, Abbas Yazdinejad, Ali Dehghantanha, Fattane Zarrinkalam, Gautam Srivastava.*

6. **GraphDART: Graph Distillation for Efficient Advanced Persistent Threat Detection.** arxiv 2025. [paper](https://arxiv.org/abs/2501.03252) [pdf](GraphDART_2025.pdf)

   *Saba Fathi Rabooki, Bowen Li, Falih Gozi Febrinanto, Ciyuan Peng, Elham Naghizade, Fengling Han, Feng Xia.*

7. **Sentient: Detecting APTs Via Capturing Indirect Dependencies and Behavioral Logic.** arxiv 2025. [paper](https://arxiv.org/abs/2502.05766) [pdf](Sentient_2025.pdf)

   *Wenhao Yan, Ning An, Wei Qiao, Weiheng Wu, Bo Jiang, Zhigang Lu, Baoxu Liu, Junrong Liu.*

8. **HADES: Detecting Active Directory Attacks via Whole Network Provenance Analytics.** arxiv 2024. [paper](https://arxiv.org/abs/2407.18858) [pdf](HADES_2024.pdf)

   *Qi Liu, Kaibin Bao, Wajih Ul Hassan, Veit Hagenmeyer.*

9. **LTRDetector: Exploring Long-Term Relationship for Advanced Persistent Threats Detection.** arxiv 2024. [paper](https://arxiv.org/abs/2404.02544) [pdf](LTRDetector_2024.pdf)

   *Xiaoxiao Liu, Fan Xu, Nan Wang, Qinxin Zhao, Dalin Zhang, Xibin Zhao, Jiqiang Liu.*

10. **Winemaking: Extracting Essential Insights for Efficient Threat Detection in Audit Logs.** arxiv 2024. [paper](https://arxiv.org/abs/2411.02252) [pdf](Winemaking_2024.pdf)

    *Weiheng Wu, Wei Qiao, Wenhao Yan, Bo Jiang, Yuling Liu, Baoxu Liu, Zhigang Lu, JunRong Liu.*

11. **KAIROS: Practical Intrusion Detection and Investigation using Whole-system Provenance.** IEEE S&P 2024. [paper](https://arxiv.org/abs/2308.05034) [pdf](KAIROS_2024.pdf)

    *Zijun Cheng, Qiujian Lv, Jinyuan Liang, Yan Wang, Degang Sun, Thomas Pasquier, Xueyuan Han.*

12. **ORTHRUS: Achieving High Quality of Attribution in Provenance-based Intrusion Detection Systems.** USENIX Security 2025. [paper](https://www.usenix.org/conference/usenixsecurity25/presentation/jiang-baoxiang) [pdf](ORTHRUS_2025.pdf) [code](https://github.com/ubc-provenance/orthrus)

    *Baoxiang Jiang, Tristan Bilot, Nour El Madhoun, Khaldoun Al Agha, Anis Zouaoui, Shahrear Iqbal, Xueyuan Han, Thomas Pasquier.*

13. **FLASH: A Comprehensive Approach to Intrusion Detection via Provenance Graph Representation Learning.** arxiv 2024. [paper](https://arxiv.org/abs/2407.13011) [pdf](FLASH_2024.pdf)

    *Mian Ul Haq Rehman, Hani Alshahrani, Daeyoung Kim.*

14. **APT-CGLP: Advanced Persistent Threat Hunting via Contrastive Graph-Language Pre-Training.** KDD 2026. [paper](https://arxiv.org/abs/2511.20290) [pdf](APT-CGLP_2025.pdf)

    *Authors TBD.*

### LLM-based Methods

1. **SHIELD: APT Detection and Intelligent Explanation Using LLM.** arxiv 2025. [paper](https://arxiv.org/abs/2502.02588) [pdf](SHIELD_2025.pdf)

   *Parth Atulbhai Gandhi, Prasanna N. Wudali, Yonatan Amaru, Yuval Elovici, Asaf Shabtai.*

2. **OCR-APT: Reconstructing APT Stories from Audit Logs using Subgraph Anomaly Detection and LLMs.** arxiv 2025. [paper](https://arxiv.org/abs/2510.12396) [pdf](OCR-APT_2025.pdf)

   *Ahmed Aly, Essam Mansour, Amr Youssef.*

3. **OMNISEC: LLM-Driven Provenance-based Intrusion Detection via Retrieval-Augmented Behavior Prompting.** arxiv 2025. [paper](https://arxiv.org/abs/2503.03108) [pdf](OMNISEC_2025.pdf)

   *Cheng Wenrui et al.*

4. **ProvSEEK: LLM-driven Provenance Forensics for Threat Investigation and Detection.** arxiv 2025. [paper](https://arxiv.org/abs/2508.21323) [pdf](ProvSEEK_2025.pdf)

   *Kunal Mukherjee, Murat Kantarcioglu.*

### Reinforcement Learning

1. **Slot: Provenance-Driven APT Detection through Graph Reinforcement Learning.** arxiv 2024. [paper](https://arxiv.org/abs/2410.17910) [pdf](Slot_2024.pdf)

   *Wei Qiao, Yebo Feng, Teng Li, Zhuo Ma, Yulong Shen, JianFeng Ma, Yang Liu.*

### Transformer-based

1. **LogShield: A Transformer-based APT Detection System Leveraging Self-Attention.** arxiv 2023. [paper](https://arxiv.org/abs/2311.05447) [pdf](LogShield_2023.pdf)

   *Sihat Afnan, Mushtari Sadia, Shahrear Iqbal, Anindya Iqbal.*

### Few-Shot Learning

1. **TREC: APT Tactic / Technique Recognition via Few-Shot Provenance Subgraph Learning.** arxiv 2024. [paper](https://arxiv.org/abs/2402.15266) [pdf](TREC_2024.pdf)

   *Mingqi Lv, HongZhe Gao, Xuebo Qiu, Tieming Chen, Tiantian Zhu, Jinyin Chen, Shouling Ji.*

## Attack Path & Tactic Recognition

1. **TPPR: APT Tactic / Technique Pattern Guided Attack Path Reasoning for Attack Investigation.** arxiv 2025. [paper](https://arxiv.org/abs/2510.16172) [pdf](TPPR_2025.pdf)

   *Authors TBD.*

## Graph Construction & Representation

1. **Prov2vec: Learning Provenance Graph Representation for Unsupervised APT Detection.** arxiv 2023. [paper](https://arxiv.org/abs/2310.00668) [pdf](Prov2vec_2023.pdf)

   *Bibek Bhattarai, H. Howie Huang.*

2. **PROVSYN: Synthesizing Provenance Graphs for Data Augmentation in Intrusion Detection Systems.** arxiv 2025. [paper](https://arxiv.org/abs/2506.05472) [pdf](PROVSYN_2025.pdf)

   *Yi Huang, Wajih UI Hassan, Yao Guo, Xiangqun Chen, Ding Li.*

## Lifelong Learning & Concept Drift

1. **METANOIA: A Lifelong Intrusion Detection and Investigation System for Mitigating Concept Drift.** arxiv 2025. [paper](https://arxiv.org/abs/2412.21544) [pdf](METANOIA_2025.pdf)

   *Jie Ying, Tiantian Zhu, Aohan Zheng, Tieming Chen, Mingqi Lv, Yan Chen.*

## Datasets

| Dataset | Description | Source |
|---------|-------------|--------|
| DARPA TC | Transparent Computing datasets | [link](https://github.com/darpa-i2o/Transparent-Computing) |
| StreamSpot | Streaming graph dataset | [paper](https://dl.acm.org/doi/10.1145/2939672.2939716) |
| Unicorn | Enterprise dataset | [paper](https://dl.acm.org/doi/10.1145/3319535.3363214) |

---

## 🔧 Contributing

欢迎提交 PR 添加新论文！格式参考：

```markdown
1. **Paper Title.** Venue Year. [paper](url) [pdf](filename.pdf)

   *Author1, Author2, ...*
```

## 📄 License

MIT

---

<p align="center">
  <i>If you find this repository useful, please consider giving it a ⭐</i>
</p>
