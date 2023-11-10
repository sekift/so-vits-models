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

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=MjQ5MWQxMDE0ZWE2ZjRlZWE3NGJiOWUyZWY3MjNkOWNfeEJwUHFvVlVNU09NVGFnMHZnRWtIaDRNd1Y3Y0pjUWNfVG9rZW46SzdMVmI5SU9yb0NzUHV4MHV4MWNnRERDbkdoXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=NjhkZDIwYzg1OGE0MTNjOTZlMDUyYzJiOGYzMmZmZDVfZ0diU2Y4Z0FlT3VhQkx2VzVpSXlwa3VJVmJVSGZ4MzVfVG9rZW46QUFSZ2J6ZHFLb1hsNWl4Y3VRRWNIZEJ4bkZ6XzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

Bind

Fallbacks

## **OpenAI** **Function Calling In LangChain**

Pydantic - JSON validation

Linux Expression Syntax

## **Tagging and Extraction Using** **OpenAI** **functions**

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=ZDQ0MTMxZjRhNjk3MTE4OGEyZWViZjMyOWUzNDRjMjFfRGlva0Qwdzd5blYwRDI0cmhGNnlRbjRVc3k3WmhwSEZfVG9rZW46QlAyUGJybGxab25iNnl4NENZV2NVanNXbjBoXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=MjkyMGYwZGM2MTY4OTdlN2NjYWQ1ZTJhNjk1ZWIxODhfcTlTVUJ6Tmd5Yzk0bTF0NlVMSUJ4UmNBeTdqalRiRERfVG9rZW46VVdIdWIxeVZ4b2Q5Mnl4cGFJamNrM3dHbnNlXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

标签 - 抽取

Extraction is similar to tagging, but used for extracting multiple pieces of information.

目的都是JSON parser

## Tools and Routing

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=ZGQxMDU5MTcyNjFlMDMyZmFkZjE2ODM5MDFiMTNlNDZfYUdGQkZKckVBZ015VWF0bjdMMVJ5dGFFWHBrWWRRbzBfVG9rZW46TzY3TGJhd01qb1Yycm14ZnZJRGNpN0RwbjBkXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

Tools ： search、math、call api

Routing就是Multi Tools的ifelse

OpenAIFunctionsAgentOutputParser

## **Conversational agent**

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=ZTA0Zjc0OGZjYzFjN2ZlZDcwODFmN2FlM2JiYmE3NGZfeUZvMnZPMDNzTlF4RUdGZlZzbUhLYlNVMWdpM21MUFVfVG9rZW46TUJFOGI2ajBLb3c2YkF4UnVOM2NqUllGbmxnXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

AgentExecutor

ConversationBufferMemory

chatbot

# 六、Finetuning Large Language Models

# 微调大模型

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=MzZlNjRmZDRkMWE5NWViYTJhZDg0NDRkMTIyNTRjNTlfcTBMUFplaWF0cEk5bGpYcmJpbnJVaHp6SGpZSTFDbTZfVG9rZW46VWN5WmJmU01Rb05IWXh4TjA3QmM5UVlvbkVuXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

## Why finetune？

meta-llama BasicModelRunner

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=YjIxMGM2NGQ0NmRiYjQxYThiZjQ5ZDgwYjM3OWJkNmFfVkZtVHN1ejlVMUVtbFVHeWxjN0lVc1BJTk9vNWY4aDdfVG9rZW46RHY5emJzcmwxb2k3S2N4VjMzS2M3NTRFbnFlXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=YjNjMGE5MTY3YmYyNjZiOTY3OTJhYTNjYTVmNzNiMjdfY1dhUFFLNDlBZlcwOVB4Q2w5cjFQYzBWRHBlTllCdEFfVG9rZW46V3JCRWJ5b2xwb2JTbTZ4b3pKSWNqQ0xIbldlXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

Pytorch

Huggingface

meta-Llama VS ChatGPT

## Where finetuning fits in

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=YjJhOWU3ODJhYTU3NjFkM2JlZjJhMTIxOWRmOTg1MjhfbUYxMHpuZFBOaTdMZHRDTjYxN2pXeDhFUXJvUWhEUTNfVG9rZW46VGxYQWJBZ3JYbzlhQTN4R25WcmN0Q2lkbjdKXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=ZWZiMmRhNGMwZDlhMWVlNWQ0NTY4ZGVmNjkxZTczYjFfdkt3cjFnbnpiRUlSUXlLdHFmS0RhdUwwa1NPYzhSMVRfVG9rZW46SXI3eWJtd0xab0VTeGR4dUFhNWNIYU9GbkNjXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

## Instruction finetuning

## Data preparation

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=NWFkMjlkMjZlMWFjODNhOWM1Zjg3MjhiNmNlMjZiMGJfYTg3cVJHeTdTZnNpaDBnTHVucWVOTHFnRjNxVjlXWWFfVG9rZW46S0U1ZmJPRXNzb2IxRFB4MEI3amN0NDhVbnlmXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

Tokenizing data

transformers - AutoTokenizer

Tokenize

Padding and truncation

Prepare instruction dataset

Tokenize the instruction dataset

Prepare test/train splits

## Training process

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=NDYwY2I5ZmE5YzFlNzgwMWYwMDAwODg3YTJjNzc1YTZfbGY5d2daazloMGlTMXJKYUZsVzFQNXdvVGhqNXVWVFhfVG9rZW46Q0IxSGJHZlh3b0pLOTN4TlpYeGNqdXMybnhiXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

1. Choose the base model.
2. Load data.
3. Train it. Returns a model ID, dashboard, and playground interface.

## Evaluation  and iteration

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=NTRjYTM5ZmVkNzY4Y2VmZWQ3MTUxYmM4YzIyZDQwODZfRlZwRGtyYW5qdEE4TEVxMGJ2bEFDOXZ1STZ4c1Jwb09fVG9rZW46S3pJZ2J4b2psb29MYVR4dm1sTGNoT0tTbkZNXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

Setup a really basic evaluation function

Evaluate all the data

Try the ARC benchmark

## Consideration on getting started now

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=ODFmNWY4NWJmM2VmMTRlYWQyYTFjYmMyZmY2ZTIxYzJfb2V6R0lnNEJlVlMyd016SWdaV1haUFFpNHFwSzF2V0NfVG9rZW46UkdwdmI0Ykppb3U2d1Z4cldJOGNVdGlFbmRMXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=OGQwMTFmYzc0MTIyMjcxNjYzNTU1OWNkOGFkZjI5NDZfVElnZlNwQnQxZkdmWUs5QmpZQWRSRGRHMzBzYzhPSnhfVG9rZW46Uk15a2IwY1Vvb1hya0t4U3Rrd2NuSmU5bnRiXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=ZmQ3NzQzZTNiYmNhNWJjYjkwNjE5NzI5MmVhNGVlMzNfOEc4M1B6MVF6aWFkeDhvcWIzNUhuVk5GZ1NpY2VVUmZfVG9rZW46WTJQOWI2R0Fsb05TdEV4SlJtTmNIS0NibkoyXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

# 七、Large Language Models on semantic search

# 大模型在语义搜索中的应用

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=MGIxNDZjM2E0MWRkMDY0MDI0MzRlZjExOTljZTdiNzVfNDk5eGREenV1UGNWQVdwaUZneTlCVjdpTmpZWFJ1d1pfVG9rZW46VlhJNmJJaWpwb1d3aHZ4T3hGaWNMVWxYbm9iXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

## Keyword Search

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=MjVmNTBlM2I3MWJhYmQzZmYxMWQ3Y2Q5NTJjNjAyNDlfWm1WTGlZZG9NOWl5M3N4R2hENnIzUjFqMlNMRUFtVWhfVG9rZW46TTRpVWI4Zmkyb3E1cVF4QUZxNGNQQUhYbjhmXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

## Embeddings

Word Embeddings

Sentence Embeddings

Article Embeddings

## Dense Retrieval

Vector Database for semantic Search

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=NDkyMWQwYzI5OWVkMmJjZGM1NmExMDYxMjFmODAwY2ZfRGRMRUNpYXZoekhOMEtDQ090Vm1MNDhVUzY0TVI3N1pfVG9rZW46WWlWWWI1dkpib1dGb1d4UmcwcWNsS0xQbm1mXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

## Rerank

Dense Retrieval

Improving Keyword Search with ReRank

## Generating Answer

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=YTA3MmRmOTg5ZjczMjg0ZGU1NGU2ODY1Nzc4MGVjMjFfOGw4eE9WNjVmenREOGRwa3pYcWlLaFRLMGNKNnJCZU5fVG9rZW46UGw3bmJPVXlZbzNlNER4QkxGR2N1YTU4bldnXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

# 八、Building Generative AI Applications with Gradio

# 使用Gradio构建生成式AI应用

## NLP Tasks Interface

Here we are using an [Inference Endpoint](https://huggingface.co/inference-endpoints) for the `shleifer/distilbart-cnn-12-6`, a 306M parameter distilled model from `facebook/bart-large-cnn`.

summarization

demo.launch(share=True)

Title - description

We are using this [Inference Endpoint](https://huggingface.co/inference-endpoints) for `dslim/bert-base-NER`, a 108M parameter fine-tuned BART model on the NER task.

Named entity

gr.close_all() 、 demo.close()

## Image captioning app

Here we'll be using an [Inference Endpoint](https://huggingface.co/inference-endpoints) for `Salesforce/blip-image-captioning-base` a 14M parameter captioning model.

Image-to-text

图像转文字描述

## Image generation app

Here we are going to run `runwayml/stable-diffusion-v1-5` using the `🧨 diffusers` library.

text-to-image

生成图像

## **`gr.Blocks()`**

```Java
with gr.Blocks() as demo:
    gr.Markdown("# Image Generation with Stable Diffusion")
    with gr.Row():
        with gr.Column(scale=4):
            prompt = gr.Textbox(label="Your prompt") #Give prompt some real estate
        with gr.Column(scale=1, min_width=50):
            btn = gr.Button("Submit") #Submit button side by side!
    with gr.Accordion("Advanced options", open=False): #Let's hide the advanced options!
            negative_prompt = gr.Textbox(label="Negative prompt")
            with gr.Row():
                with gr.Column():
                    steps = gr.Slider(label="Inference Steps", minimum=1, maximum=100, value=25,
                      info="In many steps will the denoiser denoise the image?")
                    guidance = gr.Slider(label="Guidance Scale", minimum=1, maximum=20, value=7,
                      info="Controls how much the text prompt influences the result")
                with gr.Column():
                    width = gr.Slider(label="Width", minimum=64, maximum=512, step=64, value=512)
                    height = gr.Slider(label="Height", minimum=64, maximum=512, step=64, value=512)
    output = gr.Image(label="Result") #Move the output up too
            
    btn.click(fn=generate, inputs=[prompt,negative_prompt,steps,guidance,width,height], outputs=[output])

gr.close_all()
demo.launch(share=True, server_port=int(os.environ['PORT4']))
```

## Describe and generate game

Image-text-image

## Chat with any LLM

Here we'll be using an [Inference Endpoint](https://huggingface.co/inference-endpoints) for `falcon-40b-instruct` , one of best ranking open source LLM on the [🤗 Open LLM Leaderboard](https://huggingface.co/spaces/HuggingFaceH4/open_llm_leaderboard).

To run it locally, one can use the [Transformers library](https://huggingface.co/docs/transformers/index) or the [text-generation-inference](https://github.com/huggingface/text-generation-inference)

## **`gr.Chatbot()`**

Adding other advanced features

# 九、Evaluating and Debugging Generative AI

# 生成式AI的评估与调试

## Instrument W&B

wandb

## Training a diffusion models

- Logging of the training loss and metrics
- Sampling from the model during training and uploading the samples to W&B
- Saving the model checkpoints to W&B

**Setup DDPM noise scheduler and sampler (same as in the Diffusion course).****[¶](https://s172-31-11-251p27213.lab-aws-production.deeplearning.ai/notebooks/02_diffusion_training_starter.ipynb#Setup-DDPM-noise-scheduler-and-sampler-(same-as-in-the-Diffusion-course).)**

- perturb_input: Adds noise to the input image at the corresponding timestep on the schedule
- sample_ddpm_context: Generate images using the DDPM sampler, we will use this function during training to sample from the model regularly and see how our training is progressing

## Evaluating diffusion models

- We are going to compare the samples from DDPM and DDIM samplers
- Visualize mixing samples with conditional diffusion models

wandb.init

## **LLM** **Evaluation and Tracing with W&B**

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=MDRmMzM1OWFiOWRjZjVlYWE2ZDI5OWMxOWIxNzhiOWNfQUpvTWhBWldyM3BBMnJkdHphYnU2cmdYUE5oSEp3T29fVG9rZW46WFlSaGJmN29hb1ZyTjd4UFlmQ2N5V2RUbnhiXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=MjFmZWRlMzIyMzdmNWU4YzVlZDEwYzYyMTBkMTVhNmRfTWZ2T25BVjBaRDZXb3dWY0RVMDZvRFNhRkhnWGZLdEdfVG9rZW46UnByc2JzNDQ5b3pRMWh4bENPU2NMdnU1bmJjXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

## Funeturing a language model

Let's see how to finetune a language model to generate character backstories using HuggingFace Trainer with wandb integration. We'll use a tiny language model (`TinyStories-33M`) due to resource constraints, but the lessons you learn here should be applicable to large models too!

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=NmYwMzZiMmEyNjEwODQ0NWJiNjFmNzk1Nzg0NGEyYTJfS1l1N29DaFVmM1BKYWJFS2ZIS25uVXpvaWhxQjIyR2tfVG9rZW46Qm56QWJQaUlnb0VKRDZ4aHdqa2NFb1pqbmRoXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

**Preparing data**

**Training**

LLM's don't always generate the same results. Your generated characters and backstories may differ from the video.

# 十、How diffusion models work？

# 迁移模型的工作原理

## Intuition

直觉

Noise

## Sampling

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=ZTcwNWIyNDJmMTQ5NmEwN2JiZTUxOTI4MjMyNTkyOGNfeWtFUUw0NHlYWjkwVTdsVW5ibVdOMFFHN1RCY1ZqeTlfVG9rZW46RGw0bWJ4UUFOb0JIbFp4TlZGT2NicHlqbkllXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

## Neural Network

UNet

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=YjljODU5NTI3ZWY3ODZiMjFjNWU4MDhlMzViZmJkOGNfOEQydVRMVUtHRGIxRmlSOEZYd1paMVA1ZXRSTWVxZFlfVG9rZW46RXNiOWJ6Ynl1b3R4R014bnVqdGNRZTQ5bnpoXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

## Training

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=ZDg3MjZmNWRmZTBiMmNhMjRmOGVlZDkzODhjMWU1NTFfbHpXSHlRcmJrcExobEVQMFFCU3Z4WGg1YjJPSHQ4RlBfVG9rZW46QmNwRGJHVmMwbzRqTVV4eXAwdmNXcFl0bkRlXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=ODEzNDZiMTY5MzVhYTY0MWI5ZmZhMmRiMjRkZWZiNTBfZFl4ajBBVFRjVjYwVEF4U0l0TjczT1IzdjhGelRVZlBfVG9rZW46QWFlTGI5b3Vrb3ZCRE94V0FPYmNOQnpDbmNkXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

Epoch

## Controlling

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=ODJiMTYyZjc5ZTBlYTgxZjYwMGNkMmJiMTM4ZGFhMzhfa3ZwcWRvV0RZMUJtSHo0UFJMRDkyMEx2R2sxeXc0M2xfVG9rZW46RGxjQ2JPalNLb1pQN294bTJHSWNzSVNubnVlXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

# **Acknowledgments**

Sprites by ElvGames, [FrootsnVeggies](https://zrghr.itch.io/froots-and-veggies-culinary-pixels) and [kyrise](https://kyrise.itch.io/) This code is modified from, https://github.com/cloneofsimo/minDiffusion Diffusion model is based on [Denoising Diffusion Probabilistic Models](https://arxiv.org/abs/2006.11239) and [Denoising Diffusion Implicit Models](https://arxiv.org/abs/2010.02502)

## Speeding up

DDPM

DDIM

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=N2ViOWM5ZjYyNDZlYWY5Mzg4NzUxMDg3ZmI0MGM4MTZfZUN1QzdBUEpzbUhaN2Q4N3NQV25CV3VKdWxlRFBCQkxfVG9rZW46SVNHYWJ4c3B5bzBYWlN4RXBYU2NtWGtJbnJjXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

DDIM faster than DDPM

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=ZTNmYTI1OGU1MWFmN2Y0MjUwNDk2ODg0MTRkOGY4YmRfcGpTSlduWndKSVJNYW9zeVF5aXF5UkR2ZVFja0VjSjlfVG9rZW46WGYyT2I5Q2FJbzQ5WFh4V2FjemM3MVEzbnFjXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

# 十一、Pair Programming of Large Language Model

# 大语言模型的结对编程

结对编程是一种软件开发方法，两个程序员坐在一起共同完成一个任务。其中一个程序员负责编写代码，另一个程序员则负责审查和提供反馈。这种方法可以提高代码质量、减少错误、增强团队协作能力等。

在结对编程中，两个程序员通常会使用一个共享的计算机，并使用一些工具来同步他们的工作。例如，他们可以使用版本控制系统来管理代码，并使用实时通信工具来交流想法和解决问题。

使用的模型是PaLM

## Getting Started

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=YTc4NzM5NjIyNDdmZmViNmRkNGMxNmM4N2E3OTljZDJfNE9FZ0lYa3ZXZU9EZDFoWWNLSDhUaGdsaVBYSTl0cENfVG9rZW46TU9NTmJRUkhXb010WUh4QnZIZGNaMjZmbkRoXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

- The `@retry` decorator helps you to retry the API call if it fails.
- We set the temperature to 0.0 so that the model returns the same output (completion) if given the same input (the prompt).

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=YzUwYWY1Yzc4MDNiOTgxMTI0ZTVlMTVlMDg1MDNhNzRfaTF5ZWJ3QjNaMzRSVWpidUxSVkIwd2hDTXg3Q1RiSk9fVG9rZW46WjNKU2JCUURFb3MxNnB4MzlhNmMxbjNnbkRlXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

## Using a string template

Set the MakerSuite API key with the provided helper function.

#### **Prompt template**

1. priming: getting the LLM ready for the type of task you'll ask it to do.
2. question: the specific task.
3. decorator: how to provide or format the output.

#### **Observe how the decorator affects the output****[¶](https://s172-31-15-12p30464.lab-aws-production.deeplearning.ai/notebooks/L2-template.ipynb#Observe-how-the-decorator-affects-the-output)**

- In other non-coding prompt engineering tasks, it's common to use "chain-of-thought prompting" by asking the model to work through the task "step by step".
- For certain tasks like generating code, you may want to experiment with other wording that would make sense if you were asking a developer the same question.

prompt_template = """

{priming}

{question}

{decorator}

Your solution:

"""

## Pair programming scenarios

结对编程方案

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=NjY0Yzg5YWQyNDhmOTY3YTVjZTdhYjdjYjUzMGYxZDRfRDU3OUQ3MU0xNkplcjczTGNheVVnTExVSlgwc1lPMVFfVG9rZW46TngyS2JrZGk2bzZjMXh4dFRub2NLZmp5bmlkXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

### **Scenario 1: Improve existing code**

- An LLM can help you rewrite your code in the way that's recommended for that particular language.
- You can ask an LLM to rewrite your Python code in a way that is more 'Pythonic".

 Ask for multiple ways of rewriting your code

Paste markdown into a markdown cell

Ask the model to recommend one of the methods as most 'Pythonic'

### **Scenario 2: Simplify code**

- Ask the LLM to perform a code review.
- Note that adding/removing newline characters may affect the LLM completion that gets output by the LLM.

### **Scenario 3: Write test cases**

- It may help to specify that you want the LLM to output "in code" to encourage it to write unit tests instead of just returning test cases in English.

### **Scenario 4: Make code more efficient**

- Improve runtime by potentially avoiding inefficient methods (such as ones that use recursion when not needed).

### Scenario 5: Debug your code

## Technical Debt

技术债务

"Technical Debt"这个词是软件开发中的一个术语，最早由软件工程师比尔·麦康奈尔（Bill McConnell）在1992年提出。它用来描述在软件开发过程中，由于时间、成本或其他资源的限制，而做出的妥协或牺牲，这些妥协或牺牲可能会在未来导致额外的工作或问题。

# 十二、Understanding and applying text embedding

## 理解和使用文本嵌入

## Getting started with text embeddings

Vertex AI

- The returned object is a list with a single `TextEmbedding` object.
- The `TextEmbedding.values` field stores the embeddings in a Python list.

#### **Similarity**

- Calculate the similarity between two sentences as a number between 0 and 1.
- Try out your own sentences and check if the similarity calculations match your intuition.

cosine_similarity

#### **From word to sentence embeddings**

- One possible way to calculate sentence embeddings from word embeddings is to take the average of the word embeddings.
- This ignores word order and context, so two sentences with different meanings, but the same set of words will end up with the same sentence embedding.
- These sentence embeddings account for word order and context.
- Verify that the sentence embeddings are not the same.

## Understanding text embedding

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=MWNhMTkzNDNkOWVkNjA1NDcyYWMzNmRkN2Y2NDlmOWVfNlVpdnpLWUhrNndIM3QyQkFYV29NV21tRkJhbWFXUlpfVG9rZW46RkRuTWJaN1Bab2pqSjN4RDJDc2NReGpCbkxnXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=ODk3NGViZWNkNDU5NzNjMjhkMGYwMDcwMjM5MzJmNWRfSjNVdGJvNjdwUmtzdkJBYXlEdGlVZ05heTJVSFlUZDNfVG9rZW46TzhqQmJ2M0tib2NzOTd4a0J4SGN5VnN5bkxkXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

Mix embedding ： text +picture

## Visualizing embeddings

- We'll use principal component analysis (PCA).
- You can learn more about PCA in [this video](https://www.coursera.org/learn/unsupervised-learning-recommenders-reinforcement-learning/lecture/73zWO/reducing-the-number-of-features-optional) from the Machine Learning Specialization.
- The `cosine_similarity` function expects a 2D array, which is why we'll wrap each embedding list inside another list.
- You can verify that sentence 1 and 2 have a higher similarity compared to sentence 1 and 4, even though sentence 1 and 4 both have the words "desert" and "plant".

## Applications of Embeddings

#### **Load** **Stack Overflow** **questions and answers from** **BigQuery**

- BigQuery is Google Cloud's serverless data warehouse.
- We'll get the first 500 posts (questions and answers) for each programming language: Python, HTML, R, and CSS.
- You can reuse the above code to run your own queries if you are using Google Cloud's BigQuery service.
- In this classroom, if you run into any issues, you can load the same data from a csv file.

#### **Generate text embeddings****[¶](https://s172-31-11-251p23786.lab-aws-production.deeplearning.ai/notebooks/L4-applications-of-embeddings.ipynb#Generate-text-embeddings)**

- To generate embeddings for a dataset of texts, we'll need to group the sentences together in batches and send batches of texts to the model.
- The API currently can take batches of up to 5 pieces of text per API call.

#### **Get embeddings on a batch of data****[¶](https://s172-31-11-251p23786.lab-aws-production.deeplearning.ai/notebooks/L4-applications-of-embeddings.ipynb#Get-embeddings-on-a-batch-of-data)**

- This helper function calls `model.get_embeddings()` on the batch of data, and returns a list containing the embeddings for each text in that batch.

#### **Load the data from file****[¶](https://s172-31-11-251p23786.lab-aws-production.deeplearning.ai/notebooks/L4-applications-of-embeddings.ipynb#Load-the-data-from-file)**

- We'll load the stack overflow questions, answers, and category labels (Python, HTML, R, CSS) from a .csv file.
- We'll load the embeddings of the questions (which we've precomputed with batched calls to `model.get_embeddings()`), from a pickle file.

### **Anomaly /** **Outlier** **detection****[¶](https://s172-31-11-251p23786.lab-aws-production.deeplearning.ai/notebooks/L4-applications-of-embeddings.ipynb#Anomaly-/-Outlier-detection)**

- We can add an anomalous piece of text and check if the outlier (anomaly) detection algorithm (Isolation Forest) can identify it as an outlier (anomaly), based on its embedding.

### **Classification**

- Train a random forest model to classify the category of a Stack Overflow question (as either Python, R, HTML or CSS).

## Text generation with vertex AI

#### **Classify and elaborate**

- For more predictability of the language model's response, you can also ask the language model to choose among a list of answers and then elaborate on its answer.

**Adjusting Creativity/Randomness**

- You can control the behavior of the language model's decoding strategy by adjusting the temperature, top-k, and top-n parameters.
- For tasks for which you want the model to consistently output the same result for the same input, (such as classification or information extraction), set temperature to zero.
- For tasks where you desire more creativity, such as brainstorming, summarization, choose a higher temperature (up to 1).

Softmax =one/all

temperature

top_k

top_p

## Building a QA system using semantic search

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=Nzk5N2ZhMGY2N2IwZDlmYTUxMDQ5Njg0NGM2ZWI1MzNfU0pEeXNnVE9WMlJveWFkc1JlM2dWZHI5WEFTbDZsNmhfVG9rZW46VzNFNWJRQkNJb1ViT094dGJUaGNwUWtnbk5sXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

# 十三、How Business Thinkers Can Start Building AI Plugins With Semantic Kernel

Microsoft

# 商业思考者如何开始用语义内核构建AI插件

## Semantic kernel is like your AI cooking kitchen

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=NmViNjViY2ZhMjE0M2JlYWUwY2JjM2RjNWNhYzZkNGVfM3BoU3BDa1dmWEN1TDY2SXo2Q3lLNHNpQmlpbmZXNjNfVG9rZW46SVlqc2JyMDdSb0FYRFV4ZXdmTmNRekFNbjhkXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=ZTNmZGM4MGU2ZmEyM2VjMTZmZDY5YjNkZTMyMDI0ZTFfOTJiYVpQQUFCNXBFSzhOUWZZSlRxNW1nN0IwOW8zblJfVG9rZW46TXRYN2JwNFA5bzdOajl4VU5JaGNtUlN2bmZiXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

## **Cooking up flavorful SWOTs with the kernel**

SWOTs可以被用于分析其内部和外部环境的优势（Strengths）、弱点（Weaknesses）、机会（Opportunities）和威胁（Threats）。

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=MjIxMGI3MjdkOTM5OGNiNjIwNTliNzllNjc2MGE0NTVfYThBMmNxeWpWTTZKNmdxdzYyWEJFeGNoZHVndW1TV0JfVG9rZW46Vzd4dWJxT0xkb0tVYTh4WnFZSWNnWXgwblljXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

## **Organizing the tools you make for later reuse**

1. Grow the existing business
2. Save money and time
3. Add completely new business
4. Prepare for the unknown

## Frozen dinner the design thinking meal

Inventory:

1. Kernel
2. Semantic (and Native) functions -- you can do a lot with these
3. BusinessThinking plugin --> SWOTs in ways you could never imagine
4. DesignThinking plugin ... Here you are

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=MTc5Mjg0YWJlNTE5MTE5ODUxMmUxNzFkM2UzY2VlNDFfcE5CVEtUQWEyOGVKRnZuNlJZb3lUekhVT3p0SnRVV2hfVG9rZW46TWtSYmI1OFlob1lwekR4OXBxTWMyb200blFoXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

## **Don’t forget to save the generated drippings, or “the gravy”**

Inventory:

1. Kernel
2. Semantic (and Native) functions -- you can do a lot with these
3. BusinessThinking plugin --> SWOTs in ways you could never imagine
4. DesignThinking plugin --> you did that. Congrats

... next up ... you did all that COMPLETION

![img](https://aamtech-data.feishu.cn/space/api/box/stream/download/asynccode/?code=ODc0ZmI0MDhjZDRlMWY2MWViYjMyMzFlN2Y2N2YwZjZfN3NNTEpKSEI4STZXZldMQ2pKR05ma1pwRjRKcXp6MllfVG9rZW46UkxNY2I2U1Rnb2NLMk54UktocmNWMEtJbkJiXzE2OTk1Nzk4NDc6MTY5OTU4MzQ0N19WNA)

You have now accessed both the COMPLETION and SIMILARITY engines.

##  **A kitchen that responds to your “I’m hungry” is more than feasible**

Inventory:

1. Kernel
2. Semantic (and Native) functions -- you can do a lot with these
3. BusinessThinking plugin --> SWOTs in ways you could never imagine
4. DesignThinking plugin --> you did that. Congrats
5. Use the similarity engine to your heart's content 🧲
6. THE BIG ONE!!!!!

 The next two cells will *sometimes return an error*. The LLM response is variable and at times can't be successfully parsed by the planner or the LLM will make up new functions. If this happens, try resetting the jupyter notebook kernel and running it again.

There are a variety of limitations to using the planner in August of 2023 in terms of number of tokens required and model preference that we can expect to slowly vanish over time. For simple tasks, this Planner-based approach is unusually powerful. It takes full advantage of both COMPLETION and SIMILARITY in a truly magical way.

## There's a Fully-Outfitted professional-grade kitchen ready for you

https://github.com/microsoft/chat-copilot

The backend server demonstrates how to connect to a variety of resources like auth, vector dbs, telemetry, content safety, PDF import, and even OCR.