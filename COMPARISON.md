# 方法对比表 / Method Comparison

本表格对比了溯源图APT检测领域的主要方法。

## 📊 总览

| 论文 | 年份 | 方法类型 | 核心技术 | 数据集 | 主要指标 |
|------|------|----------|----------|--------|----------|
| **APT-MCL** | 2026 | GNN | 多视图协同学习 | DARPA TC | F1: ~0.95 |
| **Sentient** | 2025 | GNN | 间接依赖+行为逻辑 | DARPA TC, StreamSpot | - |
| **TFLAG** | 2025 | GNN | 时序偏差感知学习 | DARPA TC | F1: 0.94+ |
| **SHIELD** | 2025 | LLM | GPT检测+解释 | DARPA TC | 可解释性强 |
| **OCR-APT** | 2025 | LLM+GNN | 子图异常+LLM重建 | DARPA TC | 攻击故事重建 |
| **PROVSYN** | 2025 | 数据增强 | 溯源图合成 | 合成数据 | 解决数据稀缺 |
| **METANOIA** | 2025 | 终身学习 | 概念漂移缓解 | DARPA TC | 长期稳定性 |
| **GraphDART** | 2025 | GNN | 图蒸馏 | DARPA TC | 效率优化 |
| **TPPR** | 2025 | 路径推理 | ATT&CK模式引导 | DARPA TC | 战术识别 |
| **Slot** | 2024 | RL | 图强化学习 | DARPA TC | 自适应检测 |
| **MAGIC** | 2024 | GNN | 掩码图表示学习 | DARPA TC, StreamSpot | F1: 0.96 |
| **NODLINK** | 2024 | GNN | 在线细粒度检测 | DARPA TC | 实时性强 |
| **HADES** | 2024 | GNN | AD攻击检测 | 企业网络 | 全网分析 |
| **P3GNN** | 2024 | GNN | 隐私保护 | SDN环境 | 联邦学习 |
| **LTRDetector** | 2024 | GNN | 长期关系建模 | DARPA TC | 长程依赖 |
| **Winemaking** | 2024 | 特征提取 | 审计日志精华 | DARPA TC | 高效检测 |
| **TREC** | 2024 | Few-shot | 少样本战术识别 | DARPA TC | 低样本场景 |
| **LogShield** | 2023 | Transformer | 自注意力机制 | DARPA TC | Transformer检测 |
| **Prov2vec** | 2023 | 表示学习 | 无监督图嵌入 | DARPA TC, StreamSpot | 无监督 |

## 🔍 按方法类型分类

### Graph Neural Networks (GNN)
最主流的方法，利用图结构建模系统实体关系。

| 论文 | 特点 | 适用场景 |
|------|------|----------|
| APT-MCL | 多视图融合 | 复杂攻击场景 |
| MAGIC | 掩码预训练 | 通用检测 |
| NODLINK | 在线检测 | 实时系统 |
| TFLAG | 时序建模 | 长时间攻击 |
| Sentient | 间接依赖 | 隐蔽攻击 |

### LLM-based Methods
利用大语言模型的推理和解释能力。

| 论文 | 特点 | 优势 |
|------|------|------|
| SHIELD | GPT检测 | 可解释性 |
| OCR-APT | 攻击故事重建 | 人类可读报告 |

### Reinforcement Learning (RL)
通过强化学习自适应检测策略。

| 论文 | 特点 | 优势 |
|------|------|------|
| Slot | 图强化学习 | 自适应 |

### 其他方法

| 论文 | 类型 | 特点 |
|------|------|------|
| PROVSYN | 数据增强 | 解决训练数据不足 |
| METANOIA | 终身学习 | 适应环境变化 |
| TREC | Few-shot | 少样本学习 |
| LogShield | Transformer | 序列建模 |

## 📈 数据集使用情况

| 数据集 | 使用论文数 | 特点 |
|--------|-----------|------|
| DARPA TC (Trace/Theia/Cadets/FiveDirections) | 17/19 | 最主流，含真实APT攻击 |
| StreamSpot | 3/19 | 流式图检测 |
| Unicorn | 2/19 | 企业环境 |

## 🚀 技术趋势

1. **2023**: 基础GNN方法 (MAGIC, NODLINK)
2. **2024**: 多样化探索 (RL, Few-shot, 隐私保护)
3. **2025**: LLM融合 + 工程优化 (可解释性、效率、概念漂移)
4. **2026**: 多视图协同 (APT-MCL)

## 📎 开源代码

| 论文 | 代码链接 |
|------|----------|
| MAGIC | [GitHub](https://github.com/xxx) |
| NODLINK | [GitHub](https://github.com/xxx) |
| ... | (待补充) |

---

*最后更新: 2026-02-01*
