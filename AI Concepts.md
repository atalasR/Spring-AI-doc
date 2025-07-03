# AI Concepts
This section describes core concepts that Spring AI uses. We recommend reading it closely to understand the ideas behind how Spring AI is implemented.   
这个章节描述Spring AI使用的核心概念。我们建议你仔细地阅读它，以理解Spring AI实现背后的思想。


## Models
## 模型
AI models are algorithms designed to process and generate information, often mimicking human cognitive functions. By learning patterns and insights from large datasets, these models can make predictions, text, images, or other outputs, enhancing various applications across industries.   
人工智能模型是被设计用于处理和生成信息的算法，通常模仿人类的认知功能。通过从大量的数据集中学习模式和简洁，这些模型可以进行预测、生成文本、生成图片或其他的输出，从而增强跨行业的各种应用。

There are many different types of AI models, each suited for a specific use case. While ChatGPT and its generative AI capabilities have captivated users through text input and output, many models and companies offer diverse inputs and outputs. Before ChatGPT, many people were fascinated by text-to-image generation models such as Midjourney and Stable Diffusion.   
这里有很多不同类型的AI模型，每个模型都适合特定的用例。尽管ChatGPT和它的生成式AI通过文本输入和输出吸引了用户，但许多模型和公司提供了多样化的输入和输出。在ChatGPT之前，许多人被文本到图像生成模型如Midjourney和Stable Diffusion所吸引。

The following table categorizes several models based on their input and output types:   
下面的表格根据它们的输入和输出类型对几个模型进行了分类：
![spring-ai-concepts-model-types](./images/spring-ai-concepts-model-types.jpg)

Spring AI currently supports models that process input and output as language, image, and audio. The last row in the previous table, which accepts text as input and outputs numbers, is more commonly known as embedding text and represents the internal data structures used in an AI model. Spring AI has support for embeddings to enable more advanced use cases.   
Spring AI目前支持处理输入输出为自然语言，图片和声音的模型。在上面表格的最后一行，它接收文本作为输入并输出数字，通常被称为嵌入文本（embedding text）它代表了被用于一个AI模型的内部数据结构。Spring AI支持嵌入（embeddings）以启用更高级的用例。

What sets models like GPT apart is their pre-trained nature, as indicated by the "P" in GPT—Chat Generative Pre-trained Transformer. This pre-training feature transforms AI into a general developer tool that does not require an extensive machine learning or model training background.   
使像GPT这样的模型与从不同的是它们预训练的特性，正如在GPT中的"P"所指示的-聊天生成预训练Transformer。这种预训练特性将 AI 转化为不需要广泛机器学习或模型训练背景的通用开发者工具。


## Prompts
## 提示词
Prompts serve as the foundation for the language-based inputs that guide an AI model to produce specific outputs. For those familiar with ChatGPT, a prompt might seem like merely the text entered into a dialog box that is sent to the API. However, it encompasses much more than that. In many AI Models, the text for the prompt is not just a simple string.   
提示词作为基于语言的的输入基础，这些输入指导AI模型产生特定的输出。对于那些熟悉ChatGPT的人来说，一个提示词似乎看起来仅仅像文本输入到一个对话框中并发给API。然而，它包含的东西远远不止这些。在许多AI模型中，提示词的文本不仅仅是一个简单的字符串。


ChatGPT’s API has multiple text inputs within a prompt, with each text input being assigned a role. For example, there is the system role, which tells the model how to behave and sets the context for the interaction. There is also the user role, which is typically the input from the user.   
ChatGPT的API在一个提示词中有多个文本输入，每一个文本输入都被分配一个角色。例如，这里有一个系统角色，它告诉模型如何行为并为交互设置上下文。这里还一个用户角色，它通常是来自用户的输入。

Crafting effective prompts is both an art and a science. ChatGPT was designed for human conversations. This is quite a departure from using something like SQL to "ask a question". One must communicate with the AI model akin to conversing with another person.   
