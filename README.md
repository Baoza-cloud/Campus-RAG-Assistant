# Enterprise-LLM-RAG-Assistant


## 1. 项目简介

本项目旨在构建一个企业级大语言模型知识库问答系统。

针对大语言模型存在的以下问题：

- 知识更新困难
- 无法直接访问企业私有数据
- 容易产生幻觉（Hallucination）

本项目结合：

- RAG（Retrieval-Augmented Generation，检索增强生成）
- Embedding向量检索
- FAISS向量数据库
- LoRA参数高效微调

实现一个基于企业文档知识库的智能问答系统。

---

## 2. 项目目标

实现一个完整的大模型应用流程：

用户问题

↓

问题理解

↓

知识库检索

↓

相关文档召回

↓

大语言模型生成答案

↓

返回带来源的回答


最终实现：

- 企业文档问答
- 私有知识库检索
- 降低模型幻觉
- 支持知识动态更新


---

## 3. 技术路线


原始企业文档

↓

PDF/文本解析

↓

文本清洗

↓

Chunk切分

↓

Embedding向量化

↓

FAISS建立索引

↓

Retriever检索

↓

Prompt构造

↓

LLM生成

↓

LoRA微调优化


---

## 4. 技术栈


### 编程语言

Python


### 深度学习框架

PyTorch


### 大模型相关

- Transformers
- Qwen
- PEFT(LoRA)


### RAG相关

- LangChain
- FAISS
- BGE Embedding


### 部署

- Streamlit


---

## 5. 项目开发阶段


### Phase 1：基础RAG系统

完成：

- PDF文档读取
- 文本切分
- Embedding
- 向量数据库
- 相似度检索
- LLM回答


### Phase 2：RAG优化

增加：

- Hybrid Search
- BM25检索
- Rerank模型
- Prompt优化


### Phase 3：模型微调

使用：

LoRA + SFT

优化模型对于特定领域问题的回答能力。


### Phase 4：系统评估与部署

包括：

- 检索效果评估
- 回答质量评估
- Web Demo


---

## 6. 项目结构

```text
Enterprise-LLM-RAG-Assistant

├── data
├── src
├── retrieval
├── finetuning
├── evaluation
├── deployment
├── scripts
└── docs
