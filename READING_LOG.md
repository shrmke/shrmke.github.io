# 论文阅读记录

持续整理当前目录下的 HTML 笔记，并用表格追踪每篇论文的关键信息与链接。

| 日期 | 论文 | 来源 | 关注点 | 一句话总结 | 笔记 |
| --- | --- | --- | --- | --- | --- |
| 2026-03-31 | Attention Residuals | [arXiv:2603.15031](https://arxiv.org/abs/2603.15031) | Transformer · 深度残差 · AttnRes | 把深度方向的残差聚合改成 softmax 注意力，Block AttnRes 用块表示把内存降到 O(N·d)，48B Kimi 证明收益且推理延迟 <2%。 | [HTML](2026-03-31-attention-residuals.html) |
| 2026-03-31 | One Model Is Enough | [arXiv:2603.08429](https://arxiv.org/abs/2603.08429) | RAG · Retrieval · Projection Head | 在 LLM 输出端接轻量线性层直接产出检索向量，联合 Alignment/Contrastive/Rank loss 训练，以 ≈3% 质量损失换掉独立 embedding 模型。 | [HTML](2026-03-31-one-model-is-enough.html) |
| 2026-03-31 | Semantic Shift | [arXiv:2603.21437](https://arxiv.org/abs/2603.21437) | Embedding · RAG 分块 · 语义偏移 | 提出 Shift(k)=Local×Disp 解释长文本检索退化，Shift Splitter 在 ArXiv 边界检测 F1 提升 90% 并保持稳定块大小。 | [HTML](2026-03-31-semantic-shift.html) |
| 2026-04-03 | From BM25 to Corrective RAG | [arXiv:2604.00491](https://arxiv.org/abs/2604.00491) | T²-RAGBench · 金融检索 · RAG 策略 | 测试集为 23,088 查询 / 7,318 财报；作者认为“混合检索+Cross-Encoder 重排序”是最佳实践，BM25 普遍优于稠密检索，HyDE/Multi-Query 基本无效，Context Retrieval 稳定增益，CRAG 仅小幅领先 BM25。 | [HTML](2026-04-03-from-bm25-to-corrective-rag.html) |

> 更新方法：新增 HTML 后，将日期命名保持 `YYYY-MM-DD-title.html`，并在此表追加一行，记录来源链接、核心关注点和一句话摘要。

> 2026-04-02：GitHub Pages 发布在 `shrmke.github.io`，根目录的 `index.html` 会自动读取这份表格。
