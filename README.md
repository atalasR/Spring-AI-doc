# Spring-AI-doc
Spring AI中文文档

# Introduction
# 介绍

The Spring AI project aims to streamline the development of applications that incorporate artificial intelligence functionality without unnecessary complexity.  
Spring AI的目标是简化集成人工智能功能的应用程序的开发，避免不必要的复杂性。

The project draws inspiration from notable Python projects, such as LangChain and LlamaIndex, but Spring AI is not a direct port of those projects. The project was founded with the belief that the next wave of Generative AI applications will not be only for Python developers but will be ubiquitous across many programming languages.  
这个项目从著名的Python项目（如LangChain和LlamaIndex）中汲取灵感，但是Spring AI不是直接移植这些项目。这个项目的创立是伴随着这样的信念：下一波生成式AI应用程序不仅仅是为Python开发者而设计，而是将遍布许多编程语言。


<b>Note:</b>Spring AI addresses the fundamental challenge of AI integration: Connecting your enterprise Data and APIs with AI Models.  
注意：Spring AI解决了AI的集成的本质问题：将企业数据和API与AI模型连接起来。

![Spring AI](./images/Spring%20AI%20struct.png)

Spring AI provides abstractions that serve as the foundation for developing AI applications. These abstractions have multiple implementations, enabling easy component swapping with minimal code changes.  
Spring AI提供了抽象层，这样抽象层作为开发AI应用程序的基础。这些抽象层有多种实现方式，可以通过最小的代码更改轻松交换组件。

Spring AI provides the following features:   
SpringAI提供了以下功能：
- Portable API support across AI providers for Chat, text-to-image, and Embedding models. Both synchronous and streaming API options are supported. Access to model-specific features is also available.   
- 支持跨AI提供者的便携式API，适用与聊天、文本到图像和嵌入式模型。同步和流式API都支持。还可以访问模型的特定功能。
- Support for all major [AI Model providers](https://docs.spring.io/spring-ai/reference/api/index.html) such as Anthropic, OpenAI, Microsoft, Amazon, Google, and Ollama. Supported model types include:
- 支持所有主要的AI模型提供者，例如Anthropic, OpenAI, Microsoft, Amazon, Google, and Ollama. 支持的模型类型包括：
  - Chat Completion
  - Embedding
  - Text to Image
  - Audio Transcription
  - Text to Speech
  - Moderation
- Structured Outputs - Mapping of AI Model output to POJOs.
- 结构化的输出 - AI模型输出映射到POJO。
- Support for all major Vector Database providers such as Apache Cassandra, Azure Cosmos DB, Azure Vector Search, Chroma, Elasticsearch, GemFire, MariaDB, Milvus, MongoDB Atlas, Neo4j, OpenSearch, Oracle, PostgreSQL/PGVector, PineCone, Qdrant, Redis, SAP Hana, Typesense and Weaviate.
- 支持所有主要的向量数据库提供者，例如Apache Cassandra, Azure Cosmos DB, Azure Vector Search, Chroma, Elasticsearch, GemFire, MariaDB, Milvus, MongoDB Atlas, Neo4j, OpenSearch, Oracle, PostgreSQL/PGVector, PineCone, Qdrant, Redis, SAP Hana, Typesense和Weaviate。
- Portable API across Vector Store providers, including a novel SQL-like metadata filter API.
- 跨向量存储提供商的可移植API，包含一个新颖的类似SQL的元数据过滤API。
- Tools/Function Calling - Permits the model to request the execution of client-side tools and functions, thereby accessing necessary real-time information as required and taking action.
- 工具/函数调用 - 允许模型请求执行客户端的工具和函数，从而按需访问必要的实时信息并采取行动。
- Observability - Provides insights into AI-related operations.
- 可观察性 - 提供了深入AI相关操作的洞察。
- Document ingestion ETL framework for Data Engineering.
- 用于数据工程的文档摄入ETL框架
- AI Model Evaluation - Utilities to help evaluate generated content and protect against hallucinated response.
- AI模型评估 - 这个工具帮助评估生成的内容并防止幻觉响应。
- Spring Boot Auto Configuration and Starters for AI Models and Vector Stores.
- 用于AI模型和向量存储的Spring Boot自动配置和启动器。
- ChatClient API - Fluent API for communicating with AI Chat Models, idiomatically similar to the WebClient and RestClient APIs.
- ChatClient API - AI聊天模型流畅的API，其习惯用法类似于WebClient和RestClient API.
- Advisors API - Encapsulates recurring Generative AI patterns, transforms data sent to and from Language Models (LLMs), and provides portability across various models and use cases.
- Advisors API - 封装重复出现的生成式AI模式，转换往返于语言模型的数据，并提供跨各种模型和用例的可移植性。
- Support for Chat Conversation Memory and Retrieval Augmented Generation (RAG).
- 支持聊天对话记忆和检索增强生成（RAG）。

This feature set lets you implement common use cases, such as “Q&A over your documentation” or “Chat with your documentation.”   
这个功能集合让你实现常见的用户案例，例如“关于你的文档的问答”或“与你的文档聊天”。   

The [concepts section](https://docs.spring.io/spring-ai/reference/concepts.html) provides a high-level overview of AI concepts and their representation in Spring AI.   
[概念章节](./AI%20Concepts.md)提供了一个AI概念和它们在Spring AI中的表示的高级概述。

The Getting Started section shows you how to create your first AI application. Subsequent sections delve into each component and common use cases with a code-focused approach.   
入门章节给你展示了如何创建你的第一个AI应用。随后的章节以代码为中心的方式深入探讨每个组件和常见的使用案例。













