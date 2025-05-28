# virtual-digital-person

 收集各种有关虚拟数字人的模型、应用；生成视频的模型。



## 1 应用

|      | 名称                                               | 功能                        | 论文 | Github | 使用情况                                                     |
| ---- | -------------------------------------------------- | --------------------------- | ---- | ------ | ------------------------------------------------------------ |
| 1    | [数字人口播](https://studio.d-id.com/)             | studio.d-id，虚拟数字人播报 |      |        | 无需翻墙，直接可用，免费20分钟                               |
| 2    | https://app.heygen.com/                            | 黑根，虚拟人                |      |        | 需翻墙，可以用邮箱无需注册，[教程](https://zhuanlan.zhihu.com/p/666671104) |
| 3    | https://zenvideo.qq.com/                           | 腾讯智影                    |      |        | 腾讯出的AI数字人，邀请3天体验                                |
| 4    | https://pixverse.ai/                               | pixverse                    |      |        | 无需翻墙，AI视频制作                                         |
| 5    | https://www.deepbrain.io/                          | deepbrain                   |      |        | 国外的站，访问慢                                             |
| 6    | https://lumen5.com/                                | lumen5                      |      |        | 免费试用，需注册                                             |
| 7    | https://github.com/nateraw/stable-diffusion-videos | SDV                         |      |        | 以SD为基础的，可以在Colab使用，一般要40G的GPU                |
| 8    | https://makeavideo.studio/                         | Make-A-Video                |      |        | 一张图片生成视频，天马行空                                   |
| 9    | https://www.synthesia.io/                          | synthesia                   |      |        | 需翻墙                                                       |
| 10   | Topaz Video AI v6.0.2                              | AI视频修复                  |      |        | 可用，只有下载模型，CPU适用                                  |

## 2 Sora存在的问题[20240229]

1.突变的问题：存在突然的画面转换，sora无法连接

2.物理过渡：存在不符合物理世界的过渡

3.不能理解概念：通病

## 3 Sora必读论文

|      | 题目                                                         | 作者                                                        | 简介                                                         | 论文                                               | 年份 |
| ---- | ------------------------------------------------------------ | ----------------------------------------------------------- | ------------------------------------------------------------ | -------------------------------------------------- | ---- |
| 1    | Unsupervised learning of video representations using lstms.  | Srivastava, Nitish, Elman Mansimov, and Ruslan Salakhudinov | 提出了一种基于 LSTM 的视频表示学习模型                       | https://arxiv.org/abs/1502.04681                   | 2015 |
| 2    | Recurrent environment simulators.                            | Chiappa, Silvia, et al.                                     | 本文介绍了一种模拟动作条件动态的方法，并证明了它能够适应不同的环境，从Atari游戏到3D赛车环境和迷宫。 | https://arxiv.org/abs/1704.02254                   | 2017 |
| 3    | World models                                                 | Ha, David, and Jürgen Schmidhuber                           | 本文探讨了构建生成型神经网络模型来模拟流行的强化学习环境     | https://arxiv.org/abs/1803.10122                   | 2018 |
| 4    | Generating videos with scene dynamics.                       | Vondrick, Carl, Hamed Pirsiavash, and Antonio Torralba      | 我们提出了一种具有跨距时态推理架构的生成敌对网络。           | https://arxiv.org/abs/1609.02612                   | 2016 |
| 5    | Mocogan: Decomposing motion and content for video generation. | Tulyakov, Sergey, et al.                                    | 提出了一种名为 MoCoGAN 的视频生成模型，该模型能够将视觉信号分为内容和运动两部分。 | https://arxiv.org/abs/1707.04993                   | 2018 |
| 6    | Adversarial video generation on complex datasets             | Clark, Aidan, Jeff Donahue, and Karen Simonyan              | 通过引入一个能够捕捉大型视频数据集复杂性的 GAN，解决自然视频建模的挑战问题 | https://arxiv.org/abs/1907.06571                   | 2019 |
| 7    | Generating long videos of dynamic scenes.                    | Brooks, Tim, et al.                                         | 提出了一个视频生成模型,该模型能够准确地处理对象运动、镜头变换和未来内容的出现。 | https://arxiv.org/abs/2206.03429                   | 2022 |
| 8    | Videogpt: Video generation using vq-vae and transformers.    | Yan, Wilson, et al.                                         | 提出了视频格式:一个基于可变概率生成模型的框架。视频格式使用VQ VAE来学习原始视频的实时隐藏映射。 | https://arxiv.org/abs/2104.10157                   | 2021 |
| 9    | Nüwa: Visual synthesis pre-training for neural visual world creation. | Wu, Chenfei, et al.                                         | 介绍了一种名为NÜWA的统一的多模态预训练模型，该模型能够为各种视觉合成任务生成新的或操纵现有的视觉数据（即图像和视频）。 | https://doi.org/10.1007/978-3-031-19787-1_41       | 2022 |
| 10   | Imagen video: High definition video generation with diffusion models | Ho, Jonathan, et al.                                        | 图森视频是一个基于视频传播模型的文本到视频生成系统。         | https://arxiv.org/abs/2210.02303                   | 2022 |
| 11   | Align your latents: High-resolution video synthesis with latent diffusion models. | Blattmann, Andreas, et al.                                  | 研究了潜在传播模型(LDM)在高分辨率视频生成中的应用。          | https://arxiv.org/abs/2304.08818                   | 2023 |
| 12   | Photorealistic video generation with diffusion models.       | Gupta, Agrim, et al.                                        | 本文介绍了基于扩散模型的照片级视频生成方法W.A.L.T。          | https://arxiv.org/abs/2312.06662                   | 2023 |
| 13   | Attention is all you need.                                   | Vaswani, Ashish, et al.                                     | 介绍了作者们在Twitter上进行政治实体态度检测的研究，使用预训练模型解决了Twitter内容短小、动态变化和偏离标准散文句子结构的问题。 | https://arxiv.org/abs/1706.03762                   | 2017 |
| 14   | Language models are few-shot learners.                       | Brown, Tom, et al.                                          | 我们证明了扩展语言模型可以提高许多NLP任务和评估任务的准确性。 | https://arxiv.org/abs/2005.14165                   | 2020 |
| 15   | An image is worth 16x16 words: Transformers for image recognition at scale. | Dosovitskiy, Alexey, et al.                                 | 文章的贡献主要在于证明纯Transformer可以直接应用于图像分类任务。 | https://arxiv.org/abs/2010.11929                   | 2020 |
| 16   | Vivit: A video vision transformer.                           | Arnab, Anurag, et al.                                       | 本文介绍了纯Transformer模型在图像和视频分类中的应用，讨论了Vision Transformer（ViT）处理二维图像和将视频令牌化的策略。 | https://arxiv.org/abs/2103.15691                   | 2021 |
| 17   | Masked autoencoders are scalable vision learners.            | He, Kaiming, et al.                                         | 我们提出了一种隐马尔可夫解码算法,它将输入图像的随机补丁伪装成隐藏的补丁。 | https://arxiv.org/abs/2111.06377                   | 2022 |
| 18   | Patch n'Pack: NaViT, a Vision Transformer for any Aspect Ratio and Resolution. | Dehghani, Mostafa, et al.                                   | 介绍了一种名为NaViT（Native Resolution ViT）的新模型，这是一种用于任意分辨率和宽高比的视觉Transformer | https://arxiv.org/abs/2307.06304                   | 2023 |
| 19   | High-resolution image synthesis with latent diffusion models. | Rombach, Robin, et al.                                      | 本文的重点工作是提出了一种利用先前训练好的自编码器的潜在空间进行训练的扩散模型，称作“潜在扩散模型”。 | https://arxiv.org/abs/2112.10752                   | 2022 |
| 20   | Auto-encoding variational bayes.                             | Kingma, Diederik P., and Max Welling.                       | 我们介绍了一种随机变量推理和学习算法,该算法可扩展到大量数据集,并且即使在令人不寒而栗的条件下也能很好地工作 | https://arxiv.org/abs/1312.6114                    | 2013 |
| 21   | Deep unsupervised learning using nonequilibrium thermodynamics. | Sohl-Dickstein, Jascha, et al.                              | 我们开发了一种算法,该算法可同时实现两种健壮性和可处理性。    | https://arxiv.org/abs/1503.03585                   | 2015 |
| 22   | Denoising diffusion probabilistic models.                    | Ho, Jonathan, Ajay Jain, and Pieter Abbeel.                 | 提出了一种新的基于传播概率模型的图像生成方法,这是一种潜在变量的近似模型,受到不平衡热磁场的影响。 | https://arxiv.org/abs/2006.11239                   | 2020 |
| 23   | Improved denoising diffusion probabilistic models.           | Nichol, Alexander Quinn, and Prafulla Dhariwal.             | 提出了一些简单的修改，使得去噪扩散概率模型（DDPMs）可以同时具备较高的采样质量和较竞争的对数似然性能。 | https://arxiv.org/abs/2102.09672                   | 2021 |
| 24   | Diffusion Models Beat GANs on Image Synthesis.               | Dhariwal, Prafulla, and Alexander Quinn Nichol.             | 这篇文章的主旨是评估不同生成模型的性能，包括 GANs、likelihood-based models (如 Flows 和 VAEs) 和 diffusion models，以确定它们在生成高质量图像方面的优劣。 | https://arxiv.org/abs/2105.05233                   | 2021 |
| 25   | Elucidating the design space of diffusion-based generative models. | Karras, Tero, et al.                                        | Diffusion-based generative models have emerged as a powerful new  framework for neural image synthesis, in both unconditional and  conditional settings. | https://arxiv.org/abs/2206.00364                   | 2022 |
| 26   | Scalable diffusion models with transformers.                 | Peebles, William, and Saining Xie.                          | 描述了一种基于变换器的传播模型的新类。                       | https://arxiv.org/abs/2212.09748                   | 2023 |
| 27   | Generative pretraining from pixels.                          | Chen, Mark, et al.                                          | 基于自然语言无监督表示学习技术的改进,我们研究了像素对图的有用表示。 | https://academic.microsoft.com/paper/3034445277    | 2020 |
| 28   | Zero-shot text-to-image generation.                          | Ramesh, Aditya, et al.                                      | 描述了一种基于变换器的简单方法,该方法基于一种变换器,该变换模型生成文本和图标作为单一的数据流。 | https://arxiv.org/abs/2102.12092                   | 2021 |
| 29   | Scaling autoregressive models for content-rich text-to-image generation. | Yu, Jiahui, et al.                                          | 提出了一种新的图像转换文本到图像(单独)模型,该模型生成高精度图像,并支持跨语言文本和世界知识的深度合成。 | https://arxiv.org/abs/2206.10789                   | 2022 |
| 30   | Improving image generation with better captions.             | Betker, James, et al.                                       | 论文研究了如何通过更好的描述生成图像来改善图像生成。         | [PDF](https://cdn.openai.com/papers/dall-e-3. pdf) | 2023 |
| 31   | Hierarchical text-conditional image generation with clip latents. | Ramesh, Aditya, et al.                                      | 使用 unCLIP 模型进行文本条件图像生成。                       | https://arxiv.org/abs/2204.06125                   | 2022 |
| 32   | Sdedit: Guided image synthesis and editing with stochastic differential equations. | Meng, Chenlin, et al.                                       | 提出了一种新的图像编辑和合成框架,基于最近使用随机多路径公式生成的生成模型。 | https://arxiv.org/abs/2108.01073                   | 2021 |
|      |                                                              |                                                             |                                                              |                                                    |      |