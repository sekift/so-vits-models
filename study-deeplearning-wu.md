# 一、ChatGPT Prompt Engineering for Developers 

# 给开发者看的ChatGPT提示语工程

Prompting

practices 

build

base LLMs and instruction-tuned LLMs

## Base LLMs

Unicorn-> magical forest

 the capital of France->France's largest city

## Instruction-tuned LLMs

 the capital of France->Paris

RLHF reinforcement learning from human feedback

Example:Something about Alan Turing

## **Prompting Principles**

- **Principle 1: Write clear and specific instructions**
- **Principle 2: Give the model time to “think”**

## Issue 1: The text is too long 

- Limit the number of words/sentences/characters.

## Issue 2. Text focuses on the wrong details

- Ask it to focus on the aspects that are relevant to the intended audience.

## **Issue 3. Description needs a table of dimensions**

- Ask it to extract information and organize it in a table.

## **Text to summarize**

- Summaries include topics that are not related to the topic of focus.

## Try "extract" instead of "summarize"

## Inferring 推理

multiple tasks

topic

## Transforming 翻译

## Expanding 扩展，续写

## Chatbot 聊天机器人

# 二、Building Systems with the ChatGPT API

# 利用ChatGPT接口创建自己的系统

问题要：公开公平公正

## How LLMs work？

Prompt

supervised learning

input-output ：context-completion

next word

prompting lollipop 拆分

system, user, and assistant 

System

User

Assistant

temperature 

tokens use calculate - API key

traditional supervised machine learning workflow：six months or a year to build

ChatGPT ：build in minutes or hours

## Classification

delimiter ：hashtags #

## Moderation

是否违反策略

OpenAI Moderation API

Avoid prompt injection：

1.delimiters and clear instructions

2.use additional prompt

string replace function

## 推理

可以算数

## Chain and task

complex tasks : simpler subtasks

chaining multiple prompts

Workflow

helper functions

string format - JSON - list

 text embeddings

## **Check outputs**

moderation API

latency ，additional call ， additional tokens

## Evaluation

多个步骤 如果有合适的答案应及早终结

Few-shot

one-shot

extra junk

summarize articles

good answer or not

different dimensions

BLEU score：bilingual evaluation understudy，即：双语互译质量评估辅助工具。专业的就是好。s

deal (expert) human written

evals framework

# 三、LangChain for LLM Application Development

# LangChain在LLM应用中的用途

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=YmI1ZGJjZjViMTVlMGU3YWJlNzhhZDM2ZGVhNGVlOGVfUXVIZE43UTZXdm5zUEYyZFV6V0FzTDRZNnF6eGVrWXBfVG9rZW46SW1xTmJ3c3Bnb3Nqckl4dWpHdWNsZW9objZYXzE2OTg3MTgyMjI6MTY5ODcyMTgyMl9WNA)

## Introduction

building LLM applications

composition and modularity

## models, prompts, and parsers

- Direct API calls to OpenAI
- API calls through LangChain:
  - Prompts
  - Models
  - Output parsers

Type - text

Prompt templates

Output Parsers ： JSON JSON方便结构化、解析数据

## Memory

History

ConversationBufferMemory

ConversationBufferWindowMemory

Context

​    verbose=False

ConversationTokenBufferMemory

ConversationSummaryMemory：从简

Memory & database

## Chains

- LLMChain
- Sequential Chains
  - SimpleSequentialChain
  - SequentialChain
- Router Chain

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=OTFjYjg3YTZkODRmMGVkZjk0ZTBlOThjNGNkMWM2YzdfMm1vMkFFT0xOSU9lOW82UHV2SkFPc1ZtN25lazVuMFRfVG9rZW46U3dramJMOXBMb212WUl4ZEg5NGNrZzZwblFkXzE2OTg3MTgyMjI6MTY5ODcyMTgyMl9WNA)

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=NzQyYTcyN2NmZGY3YjFhNjRiMmMyZDU1ZTQ2MWY4MzJfMnJJaTRWTHRuNWxKZFB3RVVaU0g0Q1pEbUtZUUN6azZfVG9rZW46WnVjemI5YUhPb0hvU2J4SVRWaGN3cDJZbkdmXzE2OTg3MTgyMjI6MTY5ODcyMTgyMl9WNA)

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=NzJmZWJkNmJjNjE1YzVjODJjZTRlZGI4NGYyNDFlNjFfeFdvVlVXNnVHN05lSWhWTEthRGF3SUtwY2tscWFmZjFfVG9rZW46R2JuSGJBeUdwb1Bwc3V4bnZLM2NqN0t6bkFiXzE2OTg3MTgyMjI6MTY5ODcyMTgyMl9WNA)

## Question And Answer

Embeddings vector

Vector database

处理document，先返回最合适的部分，再用gpt返回答案。

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=NjIyYmRhYzNkM2YxMGQyYmUzYjAxZDAwOTM4YmJkOWRfOHd3RXZkSU1RNFNaeldsZGdrcVQ5WThKTTZ2NGd3Z3JfVG9rZW46V0dwMWJONGFsb2ZyYU94dGxzcGN3dTd2bnFkXzE2OTg3MTgyMjI6MTY5ODcyMTgyMl9WNA)

## Evaluation

- Example generation
- Manual evaluation (and debuging)
- LLM-assisted evaluation
- LangChain evaluation platform

## Agents

- Using built in LangChain tools: DuckDuckGo search and Wikipedia
- Defining your own tools

Do some complex task

# 四、LangChain Chat with Your Data

## 通过LangChain与你的数据对话

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=ZTE5YWU4MDU4NDc0MjBjMTc1MGE5ZWQyYTc5YjQyNjlfRERBbEczZENCZzFpWmdENkxxeVFENlJTb1RLazRkS1JfVG9rZW46QkJlTmJzRkVPb1FVTW94VXJNNWNPZEh4bkpJXzE2OTg3MTgyMjI6MTY5ODcyMTgyMl9WNA)

## Document Loading

80+

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=MjY2OTM1OTE2MzIzYmJjOTM4NDVkMTMwZWMxY2E0NWZfaWhyem9zM2M5RHVUWkZsekRNVlRTSkpwNk04UjlMTk5fVG9rZW46WHRNcGJFZml5b0lUNDZ4eFoxUmM5V3J3bjBiXzE2OTg3MTgyMjI6MTY5ODcyMTgyMl9WNA)

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=YzNjNzE3YmFkMWFlMTM0ZjlhMGFlMWZhN2U0Y2M1YTBfVFZmSkJoMTVuNmt5UjZ6SDZUUXR3WmFlOW11T3d5eHBfVG9rZW46TDhTQWJVOGNlbzZpcUV4S1F0a2M0c08xblFmXzE2OTg3MTgyMjI6MTY5ODcyMTgyMl9WNA)

### Document Splitting

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=YjM1M2YyMjdkNzQxZjE2YmI0N2Y5OWMwNWJlMTcyMzdfM2xzZ1h1d2dtM0trbnpwa3Rjb0VFWjhxTlVoMXpodk1fVG9rZW46SjZIOWJVWGlYb1pwYUp4azZJcmN0ekFIbjR0XzE2OTg3MTgyMjI6MTY5ODcyMTgyMl9WNA)

RecursiveCharacterTextSplitter

TokenTextSplitter

MarkdownHeaderTextSplitter

## Vectorstores and Embeddings

retrieval augmented generation (RAG)

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=NDhhM2Y4MTk2OWFmY2MyZWYwMDM2NjUxMzQyYzY2MjBfTUtKOWtOQUJCbkhPMDdVaFRuWGtjTGxkVHNoMG50SEZfVG9rZW46Q1MwZmJIaXdTb2lYVFd4NDFla2NYT2d0bmZJXzE2OTg3MTgyMjI6MTY5ODcyMTgyMl9WNA)

Vectorstores

Similarity Search

Failure modes

## Retrieval

Maximum marginal relevance

working with metadata

compression：LLMChainExtractor

## Question Answering

RetrievalQA Chain

LangChain plus platform

1. Map_reduce chain
2. Refine chain
3. Map_rerank chain

## Chat

Memory

ConversationalRetrievalChain

# 五、Functions, Tools and Agents with LangChain

# LangChain中的函数、工具和代理功能

## OpenAI Function Calling

- LLM's don't always produce the same results. The results you see in this notebook may differ from the results you see in the video.
- Notebooks results are temporary. Download the notebooks to your local machine if you wish to save your results.

## LangChain Expression Language (LCEL)

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=YTMyZjBlNDlkYTY5MmIxMzk1OTI1NzFkYjdmMTEyYjNfZnhPa0ZoaVRIQXFadDc0U3ZNT0pNb0JUNWx0OHFMTzFfVG9rZW46SzdMVmI5SU9yb0NzUHV4MHV4MWNnRERDbkdoXzE2OTg3MTgyMjI6MTY5ODcyMTgyMl9WNA)

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=MmIwODljNDRjNjU3YzY0OTE2MzBjNjA0YWY2NmZhYzBfVlVnamJDRHU4eDBMTjk1SmZTY1NDTVVKS29aajNaWmlfVG9rZW46QUFSZ2J6ZHFLb1hsNWl4Y3VRRWNIZEJ4bkZ6XzE2OTg3MTgyMjI6MTY5ODcyMTgyMl9WNA)

Bind