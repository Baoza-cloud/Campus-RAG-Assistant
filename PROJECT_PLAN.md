# Enterprise-LLM-RAG-Assistant Project Plan


# 1. 项目背景

随着大语言模型（LLM）的快速发展，模型具有强大的文本理解和生成能力。

但是，通用大模型仍然存在：

- 知识更新困难
- 无法访问企业私有数据
- 容易产生幻觉（Hallucination）

等问题。

本项目结合 RAG（Retrieval-Augmented Generation）
和 LoRA（Low-Rank Adaptation）技术，
构建一个企业级智能知识库问答系统。


---

# 2. 项目目标

实现一个完整的大模型应用系统：

用户问题

↓

问题向量化

↓

知识库检索

↓

相关文档召回

↓

Rerank排序

↓

Prompt构造

↓

LLM生成答案

↓

LoRA优化模型


系统最终支持：

- 企业文档问答
- 私有知识检索
- 来源引用
- 降低模型幻觉


---

# 3. 系统架构


## 数据层

企业PDF、Word、Markdown文档


↓

## 文档处理层

- 文档解析
- 文本清洗
- Chunk切分


↓

## Embedding层

文本转换为向量


↓

## Retrieval层

- FAISS向量检索
- BM25关键词检索
- Rerank排序


↓

## Generation层

大语言模型生成回答


↓

## Fine-tuning层

LoRA监督微调


↓

## Evaluation层

评估系统效果



---

# 4. 技术栈


## Programming

Python


## Deep Learning

PyTorch


## LLM

- Qwen
- Transformers


## RAG

- LangChain
- FAISS
- BGE Embedding


## Fine-tuning

- PEFT
- LoRA


## Deployment

Streamlit



---

# 5. 开发阶段


## Phase 1 基础RAG

完成：

- PDF读取
- 文本切分
- Embedding
- FAISS检索
- LLM回答


## Phase 2 RAG优化

增加：

- Hybrid Search
- BM25
- Rerank
- Prompt优化


## Phase 3 LoRA微调

完成：

- 构造instruction数据
- Qwen LoRA训练
- 微调模型测试


## Phase 4 部署和评估

完成：

- Web Demo
- 检索评估
- 生成评估


---

# 6. 当前进度

[x] GitHub项目创建

[x] 项目结构设计

[x] README完善

[x] 项目名称修改

[ ] 数据收集

[ ] PDF解析

[ ] RAG基础系统

[ ] Rerank优化

[ ] LoRA微调

[ ] 部署Demo
